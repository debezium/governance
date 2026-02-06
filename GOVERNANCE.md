# Debezium Governance

This document defines the project governance for the [Debezium](https://debezium.io) project.

## Overview

Anyone can contribute to Debezium by following the [contribution workflow](https://github.com/debezium/debezium/blob/main/CONTRIBUTING.md) or discussing features and improvements on GitHub issues.
To become a committer in the Debezium project, start by making approved pull requests.
After sufficient trust is built working on Debezium, any current Debezium committer can nominate you to the steering committee for a committer role.

## Project Roles

For governance purposes, there are three formal roles for the Debezium project.

* **Contributor**: Any community member who is not yet a committer.
* **Committers**: A group of contributors with the right to merge pull requests into the Debezium repositories and publish releases.
* **Steering Committee**: A committee composed of committers with the final authority over all decisions made on the project.

### Contributor

Anyone who actively participates in the Debezium project is recognized as a contributor. 
While this often includes individuals who submit code changes via pull requests, contributors also encompass those who engage in discussions on GitHub issues and pull requests.

Contributors form the foundation of the Debezium community. 
We welcome and encourage everyone to get involved in any way they can.

### Debezium Committers

A Debezium committer is an individual who has been granted the right to merge pull requests into one of several Debezium GitHub repositories.
A pull request requires a voting/review procedure prior to merging, outlined below in the [Pull Requests](#pull-requests) section.

Debezium's committers are listed in the [committers.yml](./committers.yml).

### Steering Committee

The Debezium steering committee has the final authority over all decisions regarding the Debezium project, including:

* Whether pull requests are merged or retained in the event of a dispute.
* Who should become a committer or member of the steering committee.
* Whether any changes are necessary to the project's governance or other assets in this repository.

Debezium's steering committee members are listed in the [steering-committee.yml](./steering-committee.yml).

## Pull Requests

Pull requests against most repositories may be merged after receiving at least two positive committer or steering committee member votes.
Voting for pull requests can be done by providing a comment, a thumbs-up, or using the pull request approval workflow.

Pull requests that are small, low-risk, uncontroversial, or prefixed with `[ci]` or `[docs]` may be merged freely by anyone with commit privileges without a vote.
Examples of such pull requests may include, but are not limited to:

* Refactoring redundant code within a small number of files (2-5) that yields no behavior change.
* Adding or changing logged output.
* Adding or improving the test suite code with no loss of test coverage.
* Updating an action used by the GitHub actions, which commits should be prefixed with `[ci]`
* Fixing typos or very small clarifications to the documentation, which commits should be prefixed with `[docs]`

**Whenever in doubt about a pull request's scope or risk, fallback to the two positive vote requirement.**

The following repositories use a separate workflow and are excluded from this workflow:

* https://github.com/debezium/debezium-design-documents, see the [Proposals](#proposals) section.
* https://github.com/debezium/governance, see the [Project Governance Changes](#project-governance-changes) section.

## Proposals

Proposals, often referred to as _Debezium Design Documents_, are used to define changes to the Debezium project that could significantly impact its users or the project's direction.
Opening a proposal provides an opportunity for maintainers to review a concept before coding begins.
A proposal can be opened in the [Debezium Design Documents](https://github.com/debezium/debezium-design-documents) repository by creating a pull request.

Proposals require [lazy consensus voting](#lazy-consensus-voting), a procedure where steering committee members cast binding votes.
Any non-steering committee member may freely cast non-binding votes.
Non-binding votes are highly encouraged as they provide an indication to the proposals broader acceptance in the Debezium community.

Votes can be expressed by approving the pull request or specifying `+1` (thumbs-up emoji) on the original comment of the pull request.
Any other votes or positions can be expressed in a separate comment on the proposal.

**If you wish to express a disapproval with a `-1` (thumbs-down emoji), a reason must be given for the vote to be valid.**

## Project Governance changes

The [Debezium governance](https://github.com/debezium/governance.git) repository outlines the project's governance, code of conduct, along with a record of changes to steering committee and committer roles.

Any change in this repository requires an [explicit majority vote](#explicit-majority-voting) except for when a steering committee member marks themselves as Emeritus, which indicates they're transitioning to an inactive status.
The vote is held by the steering committee where each non-Emeritus committee member can cast a binding vote and there are no non-binding votes. 

The outcome of the vote will be made publicly available after the vote has concluded.

## Add/remove committers

The process to add or remove someone as a committer requires an [explicit majority vote](#explicit-majority-voting).
The vote is held by the steering committee, where each non-Emeritus committee member can cast a binding vote.

The outcome of the vote will be made publicly available, the [committers.yml](./committers.yml) file updated, and GitHub teams adjusted accordingly after the vote ends.

## Add/remove steering committee members

The process to add or remove someone as a steering committee member requires an [explicit majority vote](#explicit-majority-voting).
The vote is held by the steering committee, where each non-Emeritus committee member can cast a binding vote.

The outcome of the vote will be made publicly available, the [steering-committee.yml](./steering-committee.yml) file updated, and GitHub teams adjusted accordingly after the vote ends.

### Extended absence

If a steering committee member is absent for more than 6-months, the committee will contact the member directly via email.
If there is no response from the committee member after a 1-month period, the committee member will be moved to Emeritus status by updating the [steering-committee.yml](./steering-committee.yml) accordingly.

### Moving from Emeritus to active member

If an Emeritus committee member wishes to return to active status, this change requires an [explicit majority vote](#explicit-majority-voting), as if we're adding a new committee member.
If the Emeritus committee member is reinstated, the [steering-committee.yml](./steering-committee.yml) should be updated to reflect the change in Emeritus status.

### Other changes

Unless already specified in herein, all other changes to the project require an [explicit majority vote](#explicit-majority-voting) of steering committee members.
Additionally, any committee member, at any time, may request that any change require an explicit majority vote by the steering committee.

## Voting strategies

The Debezium project uses a voting system to guarantee no single member or entity can dominate the project, and ensures continued success and diversity in the project's forward vision.

The formal voting process involves the creation of a GitHub issue or pull request.
A vote is indicated by specifying `yes` or `no` on the issue or pull request, which can include the thumbs-up or thumbs-down emojis, or the use of the GitHub approval workflow.
After a defined period of time, votes are tallied, and the outcome is published.

Debezium uses several different strategies to handle voting, shown here:

* [Lazy consensus voting](#lazy-consensus-voting)
* [Explicit majority voting](#explicit-majority-voting)

Each of these strategies rely on two types of votes: 

* **Binding**: a vote from a member with specific roles used to tally the outcome of the vote. The determination of what roles are considered for binding votes is based on the subject area of the vote, such as a project proposal or governance changes as examples. 
* **Non-Binding**: any other vote cast by individuals who do not meet the binding vote requirements. While these votes do not count toward the outcome tally, they are heavily relied upon to guide those with binding-vote rights to the outcome that beset fits all involved. The use of non-binding votes, where applicable, is highly encouraged. 

### Lazy consensus voting

A lazy consensus vote uses **+1**, **0**, or **-1** to indicate one's position on a topic.

* `+1` indicates you approve
* `-1` indicates you disapprove 
* `0` indicates you have no specific opinion

The voting process concludes when there are at least three `+1` binding votes, and no `-1` binding votes.
The vote should be open for at least **3** days to allow everyone to participate.

### Explicit majority voting

An explicit majority vote uses **+1** or **-1** to indicate one's position on a topic.

* `+1` indicates you approve
* `-1` indicates you disapprove
* If you have no opinion, you should abstain from voting

The vote succeeds when at least **three binding** votes are cast, and two-thirds of cast binding values are `+1`.
The vote should be open for at least **3** days to allow everyone to participate.

## Code of Conduct

All participants in the project are expected to adhere to the project's [Code of Conduct](./CODE_OF_CONDUCT.md).
Pleasure ensure you are familiar with its guidelines and expectations, as it's essential for maintaining a positive and collaborative environment.

## Trademark Policy

The Debezium logos, icons, and domain names are protected by trademark rights.
Usage of these trademarks must adhere to our [Trademark Policy](https://www.commonhaus.org/policies/trademark-policy/).

## Contributing

We welcome all forms of contributors, from code improvements to documentation and design.
For details on how to contribute and the process your contributions will follow, please read our [Contributing Guidelines](https://github.com/debezium/debezium/blob/main/CONTRIBUTING.md).
