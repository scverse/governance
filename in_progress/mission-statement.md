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
We define "core tools" as those which facilitate sharing data through common formats, or provide foundational support for single cell datatypes (e.g. modality specific IO, toolkits) and analyses. 
These tools are placed under shared maintenance in the `scverse` GitHub organization.

We are committed to keeping this community open.
`scverse` core tools are expected to interface and be supplemented by other tools in the ecosystem.
However, development of core packages is not restricted – contributions to the core packages are welcomed and publicly acknowledged.

This document lays out our vision and processes around the project.
It may serve as an entry point for third parties into the structure of the scverse environment.

## User engagement


`scverse` provides a set of high quality core packages for performing analysis on single cell data.
These packages provide are well documented, tested, and provide broad functionality.
All of these packages work with standardized data structures which use common python numeric types and have interchange friendly on-disk formats.
Beyond these standard packages, users have access to cutting-edge and alternative analysis methods through the large ecosystem of packages built around these core tools.

* clear documentation of code and usage of tutorial notebooks,
* participation in development through issues and pull requests,
* community forums, such as our Discourse, Zulip, and Twitter account, and
* workshops at which we teach analysis workflows based on the `scverse` ecosystem

## Developer engagement

Community contributions are instrumental to scverse. Apart from direct contributions of code through pull-requests to scverse core or ecosystem packages, we emphasize the importance of

* providing feedback and reporting bugs through the community forum and the packages' issue trackers,
* creating and sharing tutorial content, either through written documentation or in-person workshops,
* contributing and maintaining documentation, making it easier for people to use or understand available tools,
* participation in community forums, by helping new users or participating in discussions on what opportunities or challenges lie ahead for scverse, and
* developing ecosystem packages, that interact with scverse core packages and data-structures and further what can be done with single-cell data in Python.


As a community, we try to incentivise code contributions through the following mechanisms:

* Pull requests: New workflows or methods can be contributed to the existing packages as extra functionalities in a pull request. These functionalities can be documented as being advised to be cited separately from the target repository if they are referenced in a scientific publication. Examples that were contributed to Scanpy are documented here: https://scanpy.readthedocs.io/en/docsearch/external/index.html. 
* Promotion of ecosystem packages: These packages can and are cited separately from Scanpy and can therefore further the developers academic careers.  Secondly, these packages are advertised on [scverse.org](), thus increasing the user base that is reached with the new package.
* Core engagement in the community is acknowledged as contribution mentions on the website, which may certify the engagement in this community. Moreover, we can attribute contributions in our Twitter accounts to make this readily available for your career development.
