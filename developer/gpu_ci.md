# GPU CI

## Goal

We want to ensure that all scverse packages with GPU support test all relevant functions via CI.

## Setup

The current setup has several components:

1. A setup on [cirun](https://cirun.io) that activates self-hosted Github Actions Runners that we specify.
2. An AWS Account that is connected to cirun which provides the GPU instances and machine images.
3. Configuration files on the target Github repostitory for cirun and Github actions.

### cirun

We use [cirun](https://cirun.io) to connect the whole setup.
cirun is responsible for selecting the specified machine image, spinning up the machine through Github actions and tearing it down.
Fundamentally, it allows us to easily use self-hosted (through AWS) runners from Github Actions with custom images.
Please visit the [cirun documentation](https://docs.cirun.io/) for an introduction and more information.

To enable GPU CI via cirun two things need to be done.

1. The cirun account needs to be connected to the cloud provider (AWS, GCP, Azure, ...).
   Instructions can be found here: https://docs.cirun.io/cloud/aws.
   We're using the Helmholtz AWS Account for this purpose.
   Currently, Isaac, Phil and Lukas have access to this AWS account.
2. The repository needs to be activated on cirun. 
   Currently, we're using Lukas' setup who is happy to activate repositories on request.

### Configuration files

#### `.cirun.yml`

cirun looks for a `.cirun.yml` configuration file in the root of a repository.
The configuration file is [documented here](https://docs.cirun.io/reference/yaml).
Ensure that the cloud is set to AWS and that the correct workflow file path is specified.
The configuration file further specifies the instance type and machine image.
All available instance types can be found here: https://aws.amazon.com/ec2/instance-types/g4/.
We're currently using `g4dn.xlarge` which is the smallest available GPU instance.
The current machine image that we're using is https://aws.amazon.com/marketplace/pp/prodview-7ikjtg3um26wq?applicationId=AWS-EC2-Console which corresponds to the image id `ami-067a4ba2816407ee9`.
Any image Ami ID can be found by clicking "continue to subscribe" on the machine image page.

Please have a look at this [.cirun.yml example configuration adapted from AnnData](https://github.com/scverse/anndata/blob/main/.cirun.yml)

```yaml
runners:
  - name: aws-gpu-runner
    cloud: aws
    instance_type: g4dn.xlarge
    machine_image: ami-067a4ba2816407ee9
    region: eu-north-1
    preemptible: false
    workflow: .github/workflows/test-gpu.yml
    labels:
      - cirun-aws-gpu
```

#### Github Actions workflow yml

Create a Github Actions workflow configuration that matches the specified name in the `.cirun.yml` configuration file.
Specify the `runs-on` as `runs-on: "cirun-aws-gpu--${{ github.run_id }}"`.
To minimize costs, we only trigger this workflow if the label `run-gpu-ci` is specified, and we cancel any workflows if they are in progress.
Dependencies are managed with `mamba` which makes it easier to install packages with GPU support.
Moreover, we only test functions that are marked with `@pytest.mark.gpu`. See below for more detail.

Please have a look at this [ test-gpu.yml example configuration adapted from AnnData](https://github.com/scverse/anndata/blob/main/.github/workflows/test-gpu.yml).

```yaml
name: AWS GPU

on:
  push:
    branches: [main]
  pull_request:
    types:
      - labeled
      - opened
      - synchronize

# Cancel the job if new commits are pushed
concurrency:
  group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
  cancel-in-progress: true

jobs:
  test:
    name: GPU Tests
    if: ${{ github.event_name == 'push' || contains(github.event.pull_request.labels.*.name, 'run-gpu-ci') }}
    runs-on: "cirun-aws-gpu--${{ github.run_id }}"
    defaults:
      run:
        shell: bash -el {0}
    steps:
      - uses: actions/checkout@v3
        with:
          fetch-depth: 0

      - name: Nvidia SMI sanity check
        run: nvidia-smi

      - uses: mamba-org/setup-micromamba@v1
        with:
          micromamba-version: "1.3.1-0"
          environment-name: anndata-gpu-ci
          create-args: >-
            python=3.10
            cupy
            pytest
            pytest-cov
            pytest-xdist
          init-shell: >-
            bash
          generate-run-shell: false

      - name: Install AnnData
        run: pip install .[dev,test,gpu]

      - name: Run test
        run: pytest -m gpu --cov --cov-report=xml --cov-context=test -n 4

      - uses: codecov/codecov-action@v3
        with:
          flags: gpu-tests
```

#### Pytest

TODO Isaac & Phil

#### Custom machine images

We are looking into custom machine images. This may be documented at a later point.
For a starting point https://docs.cirun.io/custom-images/cloud-custom-images#aws-building-custom-images-with-user-modification may be useful.
