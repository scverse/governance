# Abstract

The purpose of this document is to formalize the governance process used by the `scverse` project, to clarify how decisions are made and how the various groups within our community interact.

As a whole, we are a consensus-based community project.
However, any subproject within the scverse can have their own governance system as long as they do not conflict with the rules set out here.
Anyone with an interest in the project can join the community, contribute to the project design, and participate in the decision making process.
This document describes how that participation takes place, how to find consensus, and how deadlocks are resolved.

# Roles And Responsibilities

## The Community

The scverse community consists of anyone using or working with the project in any way.

## Contributors

A community member can become a contributor by interacting directly with the project in concrete ways, such as:

- proposing, discussing, or reviewing a change to the code, documentation, or specification via a GitHub pull request to any https://github.com/scverse repository;
- reporting a GitHub issue to any https://github.com/scverse repository;
- discussing examples or usage issues on any of our discussion platforms

among other possibilities.
Any community member can become a contributor, and all are encouraged to do so.
By contributing to the project, community members can directly help to shape its future.

All community members are required to adhere by our [code of conduct](https://scverse.org/about/code_of_conduct/).
Potential contributors are encouraged to read the [Contributing Guide](https://scanpy.readthedocs.io/en/stable/dev/index.html).

A community member becomes a contributor when the following criteria are met:

- At least two core team members support their addition
- The new member has supported the project several times, either through code or otherwise

### Project developers

Individual projects within scverse have a lot of freedom in deciding how their projects are developed.
This includes who gets commit rights to their projects.

## Core team

The core team are community members that have demonstrated continued commitment to the project through ongoing contributions.
They have shown they can be trusted to maintain scverse with care.
Team members appear as organization members on the scverse [GitHub organization](https://github.com/orgs/scverse/people) and are on our [@scverse/core](https://github.com/orgs/scverse/teams/core) GitHub team.

There are sub-roles within the core team depending on the kinds covering different kinds of contributions and responsibilities.

### Core developers

Core developers are members of the core team who have made significant code contributions to `scverse`.
They are granted additional rights so they can more easily carry on with their `scverse` related activities.
These rights include: merging approved pull requests, voting for and against contested pull-requests, and being involved in deciding major changes to the API.
Core developers are on our [@scverse/core-devs](https://github.com/orgs/scverse/teams/core-devs) GitHub team.

All core packages must have at least one core developer as a maintainer.
New core developers can be nominated by any existing core developer.
While there is no hard-and-fast rule about who can be nominated, ideally, they should have:

- Been part of the community for a significant amount of time
- Contributed significant changes of their own
- Contributed to the discussion and review of others' work
- Collaborated in a way befitting our community values

After nomination admission will be decided by two-thirds majority vote on a private mailing list by the core team.

Primary maintainers of new core packages, who are not already core developers, will be invited to join.

## Steering Council

The Steering Council (SC) members are core team members who have additional responsibilities to ensure the smooth running of the project.
SC members are expected to participate in strategic planning, approve changes to the governance model, and make decisions about funding granted to `scverse` itself (funding to community members is theirs to pursue and manage). Changes that impact the full project require analysis informed by extensive experience with both the project and the larger ecosystem.
When the core team (including the SC members) fails to reach a consensus in a reasonable timeframe, the SC is the entity that resolves the issue.

Members of the steering council also have the "owner" role within the [scverse GitHub organization](https://github.com/scverse/)
and are ultimately responsible for managing the [scverse](https://github.com/scverse) GitHub account, the [@scverse](https://twitter.com/scverse_team)
twitter account, the [scverse website](https://scverse.org), and other similar scverse-owned resources.

The steering council is currently fixed in size to three members.
This number will be increased as our community grows and diversifies, but will always be an odd number to ensure a simple majority vote outcome is always possible.
The initial steering council of the `scverse` consists of

- [Isaac Virshup](https://github.com/ivirshup)
- [Danila Bredikhin](https://github.com/gtca)
- [Lukas Heumos](https://github.com/Zethson)

The SC membership is revisited every January.
SC members who do not actively engage with the SC duties are expected to resign.
New members are added by nomination by a core developer.
Nominees should have demonstrated long-term, continued commitment to the project and its mission and values.
A nomination will result in discussion that cannot take more than a month and then admission to the SC by consensus.
During that time deadlocked votes of the SC will be postponed until the new member has joined and another vote can be held.

The `scverse` steering council may be contacted at `steering-council@scverse.org`, or via the [@scverse/steering-council](https://github.com/orgs/scverse/teams/steering-council) GitHub team.

## Management committee

The management committee consists of PIs that support the development of scverse core projects. Members of the management committee are expected to secure funding and allocate resources to the continuous development of one or more core projects.

PIs supervising the development of new core packages, who are not already part of the management committee, will be invited to join.

## Scientific advisory board

The scientific advisory boards consists of highly experienced scientists devoted to research in single cell omics analysis. In an annual meeting, the scientific advisory boards assesses the progress of scverse and suggests priorities for the next year based on the latests developments in the field.

Members of the scientific advisory boards are nominated by the core team.

## NumFOCUS subcommittee

The core team will maintain a subcommittee to manage its interactions with NumFOCUS.

- The NumFOCUS Subcommittee is comprised of at least 5 persons who manage project funding that comes through NumFOCUS. It is expected that these funds will be spent in a manner that is consistent with the non-profit mission of NumFOCUS and the direction of the Project as determined by the Core Team.
- This Subcommittee shall NOT make decisions about the direction, scope or technical direction of the Project.

_The role of NumFOCUS subcomittee is modelled after [numpy](https://numpy.org/devdocs/dev/governance/governance.html#numfocus-subcommittee)_

# Decision Making Process

Decisions about the future of the project are made through discussion with members of the community.
All non-sensitive project management discussion takes place on the issue trackers of the https://github.com/scverse repositories, in public channels of our chat, or on the forums.
Occasionally, sensitive discussion may occur via a private message.

Decisions should be made in accordance with the mission and values of the scverse project.

scverse uses a “consensus seeking” process for making decisions.
The group tries to find a resolution that has no open objections among relevant core team members.
Core members are expected to distinguish between fundamental objections to a proposal and minor perceived flaws that they can live with, and not hold up the decision-making process for the latter.
If no option can be found without objections, the decision is escalated to the SC, which will itself use consensus seeking to come to a resolution.
In the unlikely event that there is still a deadlock, the proposal will move forward if it has the support of a simple majority of the SC.

If an objection is raised on a lazy consensus, the proposer can appeal to the community and core developers and the change can be approved or rejected by escalating to the SC.
