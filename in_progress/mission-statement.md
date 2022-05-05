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

scverse is a consortium of tools with users and developers across the world. To sustain the utility and growth of the ecosystem, it’s essential the core analytic tools are robust and well-maintained. This entails consistent support and improvement of tools beyond what's possible in the conventional single-lab academic setting.

Tools within `scverse` are deliberately not unified under a single package, and instead form a consortium of core analytic tools with shared maintenance responsibilities.
We define "core tools" as those which facilitate sharing data through common formats, or provide foundational support for single cell datatypes (e.g. modality-specific IO, toolkits) and analyses. 
These tools are placed under shared maintenance in the `scverse` GitHub organization.

We are committed to keeping this community open.
`scverse` core tools are expected to interface with and be supplemented by other tools in the ecosystem.
However, development of core packages is not restricted – contributions to the core packages are welcomed and publicly acknowledged.

This document lays out our vision and processes around the project.
It may serve as an entry point for third parties into the structure of the scverse environment.

## User engagement

`scverse` provides a set of high quality infrastructure and analysis packages for single cell data.```
These packages provide are well documented, tested, and provide broad functionality.
All of these packages work with standardized data structures which use common python numeric types and have interchange-friendly on-disk formats.
Beyond these standard packages, users have access to cutting-edge and alternative analysis methods through the large ecosystem of packages built around these core tools.

Beyond the purely technical, we support our users through:

* clear documentation of code and usage of tutorial notebooks,
* participation in development through issues and pull requests,
* community forums, such as our Discourse, Zulip, and Twitter account, and
* workshops at which we teach analysis workflows based on the `scverse` ecosystem

## Developer engagement

Apart from a collection of analysis tools, `scverse` aims to support the development of new approaches to analyze and work with single cell data.
We believe that progress in this field can't be silo'd to a few groups.

We support the development of third party tools by:

* Providing stable APIs to build on top of
* Providing standardized and well supported data structure to pass around data
* Making sure all contributions are recognized in our change logs and documentation
* Promoting 3rd party packages that rely on scverse via our websites and social media feeds.
* Establishing open communication channels for
  * Discussion and collaboration between developers
  * A common forum for user support and engagement
