# Debezium Governance

This document defines the project governance for the [Debezium](https://github.com/debezium) project.

## Overview

Anyone can contribute to Debezium by following the [contribution workflow](https://github.com/debezium/debezium/CONTRIBUTE.md) or discussing features and improvements on GitHub issues.

## Project Roles

For governance purposes, there are two formal roles for the Debezium project.

* **Steering Committee**: A committee composed of committers with the final authority over all decisions made on te project.
* **Committers**: A group of contributors with the right to merge pull requests into the Debezium repositories and publish releases.

## Debezium Committers

A Debezium committer is an individual who has been granted the right to merge pull requests into one of several Debezium GitHub repositories.
A pull request requires a voting/review procedure, outlined below in the [Voting Rules and Procedures](#voting-rules-and-procedures) section prior to merging.

To become a committer in the Debezium project, start by making approved pull requests.
After sufficient trust is built through with on Debezium, any current Debezium committer can nominate you to the steering committee for a committer role.

Debezium's committers are listed in the [COMMITTERS.yml](./committers.yml).

## Steering Committee

The Debezium steering committee has the final authority over all decisions regarding the Debezium project, including:

* Whether pull requests are merged or retained in the event of a dispute.
* Who should become a committer or member of the steering committee.
* Whether any changes are necessary to the project's governance or other assets in this repository.

Debezium's steering committee members are listed in the [COMMITTEE.yml](./committee.yml).

## Voting rules and procedures

The Debezium project uses a voting system to guarantee no single member can dominate the project, and ensures continued success and diversity in the project's forward vision.

The formal voting process involves the creation of a GitHub issue, pull request, or steering committee mailing list email thread.
A vote is indicated by specifying `yes` or `no` on the issue, pull request, or mailing list thread.
After a defined period of time, votes are tallied, and the outcome is published.

Debezium uses several voting mechanisms and procedures for various purposes.

* [Pull request approvals](#pull-request-approvals)
* [Lazy consensus votes](#lazy-consensus-votes)
* [Explicit majority votes](#explicit-majority-votes)

Debezium also relies on the notion of **binding** and **non-binding** votes.

A **binding vote** is one cast by specific individuals with given roles based on the voting procedure, who's vote is used to calculate the outcome.
A **non-binding vote** is one cast by individuals who do not have binding vote roles, and these votes do not count toward the outcome, but are used to guide those with binding votes to a resolution that best fits all involved.

The following describes for each procedure, those who may vote, how the votes are recorded, and duration of the vote.

### Pull request approvals

Pull requests against most repositories may be merged after receiving at least two positive committer votes.
Voting for pull requests can be done using a comment or approving the pull request on GitHub.
If the pull request author is a member of the Debezium steering committee, this counts as one of the two required votes.

Pull requests that are small, low-risk, uncontroversial, or prefixed with `[ci]` or `[docs]` may freely be merged by any committer without any votes.
Whenever in doubt about the pull request's scope and risk, use the two positive vote requirement.

### Lazy consensus votes

Lazy consensus votes use the **+1**, **0**, or **-1** votes where:

* `+1` indicates **yes** or the **affirmative**
* `-1` indicates **no** or the **negative**
* `0` indicates you have no specific opinion

The voting process concludes when there are at least three `+1` binding votes, and no `-1` binding votes.
The vote should be open for at least **TBD** days to allow everyone to participate.

### Explicit majority votes

An explicit majority vote is simply a `+1` or `-1` based vote.
The vote succeeds when at least **three binding** votes are cast, and two-thirds of cast binding values are `+1`.
The vote should be open for at least **TBD** days to allow everyone to participate.

## Voting for specific subject areas

The following describes the voting procedures for specific subject areas.

### Governance changes

Except for the steering committee members marking themselves as Emeritus, all changes in the [governance](https://github.com/debezium/governance) repository require an explicit majority vote of steering committee members.
These votes are held on the steering committee's mailing lists, and the outcome will be publicly published.

### Add/remove steering committee members

Votes to add or remove steering committee members require an explicit majority vote of steering committee members.
These votes are held on the steering committee's mailing list, and the outcome will be publicly published.

### Add/remove committers

Votes to add or remove committers require an explicit majority vote of steering committee members.
These votes are held on the steering committee's mailing list, and the outcome will be publicly published.

### Proposals

Proposals can be opened in the [Debezium Design Documents](https://github.com/debezium/debezium-design-documents) repository.
Proposals should cover any changes to the Debezium project that might significantly impact its users or the project's direction.

Proposals require a lazy consensus approval of steering committee members; however, non-binding votes are highly encouraged to signal to the committee the proposals acceptance to the broader Debezium community.

Votes can be expressed by approving the pull request or specifying `+1` in a comment.
Other votes, with reasons, can be expressed in a comment.

**Specifying a `-1` vote must specify a reason.**

### Pull requests in non-governance & proposal repositories

Votes on pull requests not in the [governance](https://github.com/debezium/governance) or [Debezium Design Documents](https://github.com/debezium/debezium-design-documents) repositories will use the pull request vote strategy.

### Other changes

Unless already specified in herein, all other changes to the project require an explicit majority of steering committee members.
Additionally, any committee member, at any time, may request that any change require an explicit majority of steering committee votes.

## Code of Conduct

All participants in the project are expected to adhere to the project's [Code of Conduct](./CODE_OF_CONDUCT.md).
Pleasure ensure you are familiar with its guidelines and expectations, as it's essential for maintaining a positive and collaborative environment.

## Trademark Policy

The Debezium logos, icons, and domain names are protected by trademark rights.
Usage of these trademarks must adhere to our [Trademark Policy](https://www.commonhaus.org/policies/trademark-policy/).

## Contributing

We welcome all forms of contributors, from code improvements to documentation and design.
For details on how to contribute and the process your contributions will follow, please read our [Contributing Guidelines](https://github.com/debezium/debezium/CONTRIBUTE.md).
