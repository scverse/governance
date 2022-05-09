# Mission Statement

## Goals

We want to make analysis tools for omics data in the life sciences as accessible as possible. This means:

* Interoperability -- we focus on developing open, standardized, and efficient file formats to encourage data sharing and re-use.
* Diversity -- we believe in removing barriers to participation in research, including economic factors and institutional culture. Our tools will have the most impact if they are developed by and for a diverse community.
* Transparency -- we do our work as openly as possible and welcome our community to join the decision making process.
* Simplicity -- invent as little as possible and work with standard pydata types. We strive for easy-to-use interfaces that reduce mental overhead.
* Efficiency -- our tools should require as little computational resources as possible. This makes analysis of large datasets more accessible, and makes cutting edge research possible.

## Abstract

The growing adoption of Python for single-cell omics data analysis has been catalyzed by [Scanpy](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-017-1382-0) and [AnnData](https://anndata.readthedocs.io/en/latest/). 
Around this infrastructure an ecosystem of packages has been created by various developers and institutions — extending single-cell analysis to different modalities and addressing challenges at the cutting-edge of single-cell research. We believe that progress in this field can't be silo'd to a few groups. To further nurture the growth of this ecosystem, we've formed a new organization -- **`scverse`**.

`scverse` is a consortium of tools with users and developers across the world. To sustain the utility and growth of the ecosystem, it’s essential that the core analytic tools are robust and well-maintained. This entails consistent support and improvement of tools beyond what's possible in the conventional single-lab academic setting.

`scverse` provides high quality infrastructure for analysis of single cell omics data. These *core* tools are well documented, tested, and provide broad functionality. They work with standardized data structures which use common Python numeric types and have interchange-friendly on-disk formats.

We define *core* tools as those which facilitate sharing data through common formats, or provide foundational support for single cell datatypes (e.g. modality-specific IO, toolkits) and analyses. 
These tools are placed under shared maintenance and development in the `scverse` GitHub organization.

`scverse` *core* tools are expected to interface with and be supplemented by other tools in the ecosystem. `scverse` strives for synergy and interoperability with the ecosystem of packages built around these *core* tools, to ultimately provide users to cutting-edge and varied selection of analysis methods.

## User engagement

We are community-driven and committed to keeping the `scverse` community open. We strive to actively foster a community where everyone is and feels welcomed, and where there are no barriers to contributions in any form. We welcome newcomers and pledge to build an environment where they can grow as contributors, developers and community members. Together with technical and development support, we also support our users through:

* Clear documentation of code and usage via docs and tutorials.
* Participation in development through issues and pull requests.
* Community forums, such as our Discourse, Zulip, and Twitter.
* Workshops at which we teach analysis workflows based on the `scverse` ecosystem.

## Developer engagement

Tools within `scverse` are deliberately not unified under a single package, and instead form a consortium of *core* analytic tools with shared maintenance responsibilities. `scverse` aims to support the development of new approaches to analyze and work with single cell data. However, development of *core* packages is not restricted – contributions to the *core* packages are welcomed and publicly acknowledged.
We support the development of third party tools by:

* Providing stable APIs to build on top of.
* Providing standardized and well supported data structure to pass around data.
* Making sure all contributions are recognized in our change logs and documentation.
* Promoting 3rd party packages that rely on `scverse` via our websites and social media feeds.
* Establishing open communication channels for:
  * Discussion and collaboration between developers.
  * A common forum for user support and engagement.
