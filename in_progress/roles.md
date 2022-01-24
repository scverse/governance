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

Potential contributors are encouraged to read the Contributing Guide (**TODO**) as well as the Code of Conduct (**TODO**)

A community member becomes a contributor when the following criteria are met:

- At least two core developers from separate employers agree membership is a good idea.
- The new member has supported the project several times, either through code or otherwise, and has demonstrated a willingness to help solve other people's problems, not just their own.
- The new member demonstrates some degree of familiarity of open source practices and online courtesy.

## Core developers

Core developers are community members that have demonstrated continued commitment to the project through ongoing contributions.
They have shown they can be trusted to maintain the scverse with care.
Becoming a core developer allows contributors to merge approved pull requests, cast votes for and against merging a pull-request, and be involved in deciding major changes to the API, and thereby more easily carry on with their project related activities. 
Core developers appear as organization members on the scverse [GitHub organization](https://github.com/orgs/scverse/people) and are on our [@zarr-developers/core-devs](https://github.com/orgs/zarr-developers/teams/core-devs) GitHub team (**TODO**).
Core developers are expected to review code contributions while adhering to the [core developer guide](CORE_DEV_GUIDE.md) (**TODO**).
New core developers can be nominated by any existing core developer, and for details on that process see our core developer guide.

## Steering Council

The Steering Council (SC) members are core developers who have additional responsibilities to ensure the smooth running of the project.
SC members are expected to participate in strategic planning, approve changes to the governance model, and make decisions about funding granted to the project itself.
(Funding to community members is theirs to pursue and manage). 
The purpose of the SC is to ensure smooth progress from the big-picture perspective.
Changes that impact the full project require analysis informed by long experience with both the project and the larger ecosystem.
When the core developer community (including the SC members) fails to reach such a consensus in a reasonable timeframe, the SC is the entity that resolves the issue.

Members of the steering council also have the "owner" (**TBD**) role within the [zarr-developers GitHub organization](https://github.com/zarr-developers/)
and are ultimately responsible for managing the [scverse](https://github.com/scverse) GitHub account, the [@zarr_dev](https://twitter.com/zarr_dev)
twitter account, the [scverse website](https://scverse.org), and other similar scverse-owned resources.

The steering council is currently fixed in size to three members.
This number may be increased in the future, but will always be an odd number to ensure a simple majority vote outcome is always possible. 
The initial steering council of Zarr consists of

* [Ryan Abernathey](https://github.com/rabernat)

* [John Kirkham](https://github.com/jakirkham)

* [Alistair Miles](https://github.com/alimanfoo)

* [Josh Moore](https://github.com/joshmoore)

* [Ryan Williams](https://github.com/ryan-williams)

The SC membership is revisited every January.
SC members who do not actively engage with the SC duties are expected to resign.
New members are added by nomination by a core developer.
Nominees should have demonstrated long-term, continued commitment to the project and its mission and values.
A nomination will result in discussion that cannot take more than a month and then admission to the SC by consensus.
During that time deadlocked votes of the SC will be postponed until the new member has joined and another vote can be held.

The Zarr steering council may be contacted at `zarr-steering-council@googlegroups.com`, or via the [@zarr-developers/steering-council](https://github.com/orgs/zarr-developers/teams/steering-council) GitHub team. (**TODO**)

# Decision Making Process

Decisions about the future of the project are made through discussion with all members of the community.
All non-sensitive project management discussion takes place on the issue trackers of the https://github.com/scverse repositories.
Occasionally, sensitive discussion may occur via a private message.

Decisions should be made in accordance with the mission and values of the scverse project.

scverse uses a “consensus seeking” process for making decisions.
The group tries to find a resolution that has no open objections among core developers.
Core developers are expected to distinguish between fundamental objections to a proposal and minor perceived flaws that they can live with, and not hold up the decision-making process for the latter.
If no option can be found without objections, the decision is escalated to the SC, which will itself use consensus seeking to come to a resolution.
In the unlikely event that there is still a deadlock, the proposal will move forward if it has the support of a simple majority of the SC.

Decisions (in addition to adding core developers and SC membership as above) are made according to the following rules:

- **Minor documentation changes**, such as typo fixes, or addition / correction of a
  sentence, require approval by a core developer *and* no disagreement or requested
  changes by a core developer on the issue or pull request page (lazy
  consensus). Core developers are expected to give "reasonable time" after approval and before merging for others
  to give their opinion on the pull request if they’re not confident others
  would agree, where "reasonable time" is likely one working day.

- **Code changes and major documentation changes** require agreement by *one*
  core developer *and* no disagreement or requested changes by a core developer
  on the issue or pull-request page (lazy consensus). For all changes of this type,
  core developers are expected to give "reasonable time" after approval and before
  merging for others to weigh in on the pull request in its final state, where
  "reasonable time" is likely a few working days.

- **Changes to APIs** require a dedicated issue on the related
  issue tracker, e.g. [muon](https://github.com/scverse/muon/issues), and follow the
  decision-making process outlined above, though "reasonable time" is likely extended
  to at least a week.

- **Changes to the specification** require a dedicated issue on the [issue tracker](https://github.com/zarr-developers/zarr-specs/issues) and even more time than an API change.
  The appropriate length of time is currently under discussion.

- **Changes to this governance model or our mission, vision, and values**
  require a  dedicated issue on our [issue tracker](https://github.com/zarr-developers/governance/issues)
  and follow the decision-making process outlined above, with "reasonable time" being
  at least two weeks. However, if there is unanimous agreement from core developers on the change,
  it can move forward faster.

If an objection is raised on a lazy consensus, the proposer can appeal to the community and core developers and the change can be approved or rejected by escalating to the SC.