# Mission Statement

## Goals

We want to make single cell data analysis as accesible as possible. This means

* Keeping data open, prioritizing interoperable data formats over serialized objects
* Diversity, we believe in removing barriers to participation in research, including economic factors and institutional culture. Our tools will have the most impact if they are developed by and for a diverse community.
* Transparency, we do our work as openly as possible and welcome our community to join in the decision making process
* Simplicity – Invent as little as possible and work with standard pydata types. Our users already have to be experts in multiple-fields. Lets not raise the bar for usage higher.

## Abstract

Scanpy and accessory packages for single-cell data analysis in Python have seen a strong and steady increase in interest since its first publication.
The ecosystem has outgrown a single package and modality, so we've formed a new organization, the **`scverse`**, to handle this.

The `scverse` is a community-based ecosystem of tools with users and developers across many organizations.
For the ecosystem to be useful and grow, it’s essential that the core analytic tools are well made and continue to be maintained. Frequently, tools are made by small groups within individual labs, and can quickly fall into disrepair once a grad student leaves. To some extent, this is unavoidable and is the nature of academic code. For commonly used, important tools this needs to be avoided.

The scverse constitutes an environment of tools which is deliberately not unified under a single package, but instead a consortium of core analytic tools with shared maintanance resposibilities.
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

The scverse heavily benefits from a variety of people contributing code via different channels. The channels used at the moment are:

* Pull requests on scverse core or ecosytem packages: These can be used to fix bugs that are experienced during a workflow or to contribute functionalities. 
* Feedback/ bug reporting through issues and the community forum.
* Creating and sharing tutorial content, either through written documentation or in person workshops.
* Contributing and maintaining documentation, making it easier for people to use or understand available tools.
* Participation in community forums, by helping new users or participating in discussions.
* Ecosystem packages: Development of tools and analyses which interact with core packages, work with AnnData or MuData objects, or further what can be done with single cell data in Python.

As a community, we try to incentivise code contributions through the following mechanisms:

* Pull requests: New workflows or methods can be contributed to the existing packages as extra functionalities in a pull request. These functionalities can be documented as being advised to be cited separately from the target repository if they are referenced in a scientific publication. Examples that were contributed to Scanpy are documented here: https://scanpy.readthedocs.io/en/docsearch/external/index.html. 
* Promotion of ecosystem packages: These packages can and are cited separately from Scanpy and can therefore further the developers academic careers.  Secondly, these packages are advertised on [scverse.org](), thus increasing the user base that is reached with the new package.
* Core engagement in the community is acknowledged as contribution mentions on the website, which may certify the engagement in this community. Moreover, we can attribute contributions in our Twitter accounts to make this readily available for your career development.
