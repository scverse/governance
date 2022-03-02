# Mission Statement

## Goals

We want to make single cell omics data analysis as accessible as possible. This means

* Interoperability -- we focus on developing open, standardized, and interchangeable file formats and keep our data openly accessible. 
* Diversity -- we believe in removing barriers to participation in research, including economic factors and institutional culture. Our tools will have the most impact if they are developed by and for a diverse community.
* Transparency -- we do our work as openly as possible and welcome our community to join the decision making process.
* Simplicity -- invent as little as possible and work with standard pydata types. We strive for easy-to-use interfaces that reduce mental overhead.

## Abstract

The growing adoption of Python for single-cell omics data analysis has been catalyzed by [Scanpy](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1382-0) and [AnnData](https://anndata.readthedocs.io/en/latest/). 
Around this infrastructure an ecosystem of packages has been contributed by various developers and institutions — extending single-cell analysis to different modalities and addressing challenges at the cutting-edge of single-cell research.
To further nurture the growth of this ecosystem, we've formed a new organization -- **`scverse`**.

scverse is a consortium of tools with users and developers across the world. To sustain the utility and growth of the ecosystem, it’s essential the core analytic tools are robust and well-maintained. This entails consistently support and improvement tools beyond what's possible in the conventional single-lab academic setting.

Tools within `scverse` are deliberately not unified under a single package, and instead form a consortium of core analytic tools with shared maintenance responsibilities.
Tools within this environment that are considered "core" for sharing data between tools or are required for fundamental analyses of single cell datatypes are placed under shared maintainance in the `scverse` github organization.

Workflows in this environment are heterogeneous and this core can be supplemented with analysis specific accessory packages.
This document lays out our vision and processes around the project's community in a transparent and accessible way.
We are committed to keeping this community open to third-party contributions and usage and are committed to acknowledging contributions.
This white paper may serve as an entry point for third parties into the structure of the scverse environment.

## User engagement

The ecosystem centred on `scverse` core packages consists of python packages which are documented on readthedocs and commonly accompanied by scientific publications.
Its primary purpose is to allow users to generalise workflows to their own data analysis settings.
We promote user engagement via the following mechanisms:

* Clear documentation of code and usage of tutorial notebooks.
* Participation in development though issues and pull requests.
* Community forums, such as our Discourse and Twitter account. scverse environment-centric workshops at which scverse workflows are taught and hackathons at which functionalities are contributed. We share event dates and resources within the environment to increase impact and to exploit synergies.

## Developer engagement

Scverse heavily benefits from a variety of people contributing code via different channels. The channels used at the moment are:

* Pull requests on scverse core or ecosystem packages: These can be used to fix bugs that are experienced during a workflow or to contribute functionalities. 
* Feedback/bug reporting through issues and the community forum.
* Creating and sharing tutorial content, either through written documentation or in person workshops.
* Contributing and maintaining documentation, making it easier for people to use or understand available tools.
* Participation in community forums, by helping new users or participating in discussions.
* Ecosystem packages: Development of tools and analyses which interact with core packages, work with AnnData or MuData objects, or further what can be done with single cell data in Python.

As a community, we try to incentivise code contributions through the following mechanisms:

* Pull requests: New workflows or methods can be contributed to the existing packages as extra functionalities in a pull request. These functionalities can be documented as being advised to be cited separately from the target repository if they are referenced in a scientific publication. Examples that were contributed to Scanpy are documented here: https://scanpy.readthedocs.io/en/docsearch/external/index.html. 
* Promotion of ecosystem packages: These packages can and are cited separately from Scanpy and can therefore further the developers academic careers.  Secondly, these packages are advertised on [scverse.org](), thus increasing the user base that is reached with the new package.
* Core engagement in the community is acknowledged as contribution mentions on the website, which may certify the engagement in this community. Moreover, we can attribute contributions in our Twitter accounts to make this readily available for your career development.