# Abstract

The purpose of this document is to formalize the governance process used by the `scverse` project, to clarify how decisions are made and how the various elements of our community interact.

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

All community members are required to adhere by our code of conduct (**TODO: add link**).
Potential contributors are encouraged to read the Contributing Guide (**TODO: add link**).

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
The core team meets on a regular basis and reviews propsals as described in the section [Descision Making Process](#decision-making-process). 

Core team members may resign from the project at any time, or lose their vote if a proposal to that effect is passed as outlined in the [Descision Making Process](#decision-making-process) section of this page.
A proposal to remove someone’s vote may not contain any other business.
Each person must be the subject of a separate proposal.
The person in question has the right to vote on the proposal to remove their vote.

There are sub-roles within the core team depending on the kinds covering different kinds of contributions and responsibilities.

### Core developers

Core developers are members of the core team who have made signifigant code contributions to `scverse`.
They are granted additional rights so they can more easily carry on with their `scverse` related activities.
These rights include: merging approved pull requests, voting for and against contested pull-requests, and being involved in deciding major changes to the API.
Core developers are on our [@scverse/core-devs](https://github.com/orgs/scverse/teams/core-devs) GitHub team (**TODO**).
Core developers are expected to review code contributions while adhering to the [core developer guide](CORE_DEV_GUIDE.md) (**TODO**).

All core packages must have at least one core developer as a maintainer.
New core developers can be nominated by any existing core developer. 
While there is no hard-and-fast rule about who can be nominated, ideally, they should have: 

* Been part of the community for a significant amount of time
* Contributed significant changes of their own
* Contributed to the discussion and review of others' work
* Collaborated in a way befitting our community values

After nomination admission will be decided by two-thirds majority vote on a private mailing list by the core team.

Primary maintainers of new core packages, who are not already core developers, will be invited to join.

## Steering Council

The Steering Council (SC) members are core team members who have additional responsibilities to ensure the smooth running of the project.
SC members are expected to participate in strategic planning, approve changes to the governance model, and make decisions about funding granted to `scverse` itself.
(Funding to community members is theirs to pursue and manage). 
The purpose of the SC is to ensure smooth progress from the big-picture perspective.
Changes that impact the full project require analysis informed by long experience with both the project and the larger ecosystem.
When the core team (including the SC members) fails to reach such a consensus in a reasonable timeframe, the SC is the entity that resolves the issue.

Members of the steering council also have the "owner" role within the [scverse GitHub organization](https://github.com/scverse/)
and are ultimately responsible for managing the [scverse](https://github.com/scverse) GitHub account, the [@scverse](https://twitter.com/scanpy_team)
twitter account, the [scverse website](https://scverse.org), and other similar scverse-owned resources.

The steering council is currently fixed in size to three members.
This number will be increased as our community grows and diversifies, but will always be an odd number to ensure a simple majority vote outcome is always possible. 
The initial steering council of the `scverse` consists of

* [Isaac Virshup](https://github.com/ivirshup)
* [Danila Bredikhin](https://github.com/gtca)
* [Lukas Heumos](https://github.com/Zethson)

The SC membership is revisited every January.
SC members who do not actively engage with the SC duties are expected to resign.
New members are added by nomination by a core developer.
Nominees should have demonstrated long-term, continued commitment to the project and its mission and values.
A nomination will result in discussion that cannot take more than a month and then admission to the SC by consensus.
During that time deadlocked votes of the SC will be postponed until the new member has joined and another vote can be held.

The `scverse` steering council may be contacted at `steering-council@scverse.org`, or via the [@scverse/steering-council](https://github.com/orgs/scverse/teams/steering-council) GitHub team.

# Decision Making Process

This project uses [Martha’s Rules](https://journals.sagepub.com/doi/10.1177/088610998600100206) as described in the [blog post by Greg Wilson](https://third-bit.com/files/2020/08/marthas/) for making decisions. 
The first section below describes these rules; the second lists voting members of the project and explains how to become one, while the third lists decisions made to date.

## Making Decisions

Decisions about the future of the project are made through discussion with members of the community.
All non-sensitive project management discussion takes place on the issue trackers of the https://github.com/scverse repositories, in public channels of our chat, or on the forums.
Occasionally, sensitive discussion may occur via a private message.

Decisions should be made in accordance with the mission and values of the scverse project.

Before each core team meeting, anyone from the community who wishes may sponsor a proposal by filing an issue in the [scverse/governance](https://github.com/scverse/governance) repository tagged `proposal`.
Proposals must be filed at least 24 hours before a meeting in order to be considered at that meeting, and must include:
 * a one-line summary (the subject line of the issue)
 * the full text of the proposal
 * any required background information
 * pros and cons
 * possible alternatives

A quorum is established in a meeting if half or more of voting members are present.

Once a person has sponsored a proposal, they are responsible for it. 
The group may not discuss or vote on the issue unless the sponsor or their delegate is present. 
The sponsor is also responsible for presenting the item to the group.
After the sponsor presents the proposal, a sense vote is cast for the proposal prior to any discussion:
 * Who likes the proposal?
 * Who can live with the proposal?
 * Who is uncomfortable with the proposal?

If all of the group likes or can live with the proposal, it is immediately accepted with no further discussion.

If most of the group is uncomfortable with the proposal, it is postponed for further rework by the sponsor.
If any members are uncomfortable they can briefly state their objections. 
A timer is then set for a brief discussion moderated by the facilitator. 
After 10 minutes or when no one has anything further to add (whichever comes first), the facilitator calls for a yes-or-no vote on the question: “Should we implement this decision over the stated objections?”. 
If a majority votes “yes” the proposal is implemented. Otherwise, the proposal is returned to the sponsor for further work.

## Suffrage

The [core team](#core-team) as defined above are voting members of this project. 

## Recording Decisions

Proposals and their decisions are tracked as issues in the [scverse/governance repository](https://github.com/scverse/governance/issues?q=is%3Aissue+label%3Aproposal). 
