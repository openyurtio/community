Note :This document keeps changing based on the status and feedback from Community.
This document gives a brief overview of the community roles with the requirements and responsibilities associated with them.

| Role | Responsibilities | Requirements | Defined by |
| -----| ---------------- | ------------ | -------|
| [Member](#Member) | Active contributor in the community | Sponsored by 2 Reviewers and multiple contributions to the project | OpenYurt GitHub organization Member |
| [Reviewer](#Reviewer) | Review contributions from other members | Sponsored by 1 Approver and History of review and authorship | OWNERS file reviewer list and add `lgtm` label to specific PRs |
| [Approver](#Approver) | Contributions acceptance approval | Sponsored by 2 maintainers and Highly experienced active reviewer and contributor | OWNERS file approver list and add `approved` label to specific PRs |
| [Maintainer](#Maintainer) | Set direction and priorities | Sponsor from 3 maintainers, demonstrated responsibility and excellent technical judgement | MAINTAINERS file maintainer list |

## Member

Members are continuously active contributors in the community. They can have issues and PRs assigned to them. Members are expected to remain active contributors to the community.

### Requirements

- Have made multiple contributions to the project or community. Contribution may include, but is not limited to:
    - Authoring or reviewing PRs on GitHub
    - Filing or commenting on issues on GitHub
    - Contributing to community discussions (e.g. meetings, discussion group)
- Sponsored by 2 reviewers
    - With no objections from other reviewers
- Open an issue against the openyurtio/openyurt repository.

### Responsibilities and privileges

- Be a [Member of the OpenYurt GitHub organization](https://github.com/orgs/openyurtio/people)
- Responsive to issues and PRs assigned to them
- Active owner of code they have contributed (unless ownership is explicitly transferred)
    - Code is well tested
    - Tests consistently pass
    - Addresses bugs or issues discovered after code is accepted

## Reviewer

Reviewers are able to review code for quality and correctness. They are knowledgeable about both the codebase and software engineering principles.

### Requirements

- As a Member and have reviewed at least 5 PRs to the codebase
- Knowledgeable about the codebase
- Sponsored by an approver and with no objections from other approvers
- Open an issue against the specific repository(like openyurtio/openyurt) and done through PR to update OWNERS file of specific repository.

### Responsibilities and privileges

- Has right to add `lgtm` label to PRS
- Responsible for project quality control
    - Focus on code quality and correctness, including testing and factoring
    - May also review for more holistic issues, but not a requirement

## Approver

Code approvers are able to both review and approve code contributions. While code review is focused on code quality and correctness, approval is focused on holistic acceptance of a contribution including: backwards / forwards compatibility, adhering to API and flag conventions, subtle performance and correctness issues, interactions with other parts of the system, etc.

### Requirements

- Primary reviewer for a number of substantial PRs to the codebase
- Sponsored by 2 maintainers and with no objections from other maintainers
- Open an issue against the specific repository(like openyurtio/openyurt) and done through PR to update OWNERS file of specific repository.

### Responsibilities and privileges

- Has right to add `approved` label to PRs
- Demonstrate sound technical judgement and make sure the feature has deeply been discussed before `/approve`
- Responsible for project quality control
    - Focus on holistic acceptance of contribution such as dependencies with other features, backwards / forwards compatibility, API and flag definitions, etc
- Mentor members and reviewers

## Maintainer

Maintainers are the first and foremost contributors that are committed to the success of OpenYurt project.

### Requirements

- Sponsored by 3 maintainers and with no objections from other maintainers
- Deep understanding of the technical goals and direction
- Deep understanding of the technical domain
- Sustained contributions to design and direction by doing all of:
    - Authoring and reviewing proposals
    - Initiating, contributing and resolving discussions (emails, GitHub issues, meetings)
    - Identifying subtle or complex issues in designs and implementation PRs
- Open an issue against the openyurtio/openyurt repository and done through PR to update Maintainers file.

### Responsibilities and privileges

- Set technical direction and priorities
- Classify GitHub issues and perform pull request reviews for other maintainers and the community.
- During GitHub issue classification, apply all applicable [labels](https://github.com/openyurtio/openyurt/labels)
  to each new issue. Labels are extremely useful for follow-up of future issues. Which labels to apply
  is somewhat subjective so just use your best judgment.
- Make sure that ongoing PRs are moving forward at the right pace or closing them if they are not
  moving in a productive direction.
- Participate when called upon in the security release process. Note
  that although this should be a rare occurrence, if a serious vulnerability is found, the process
  may take up to several full days of work to implement.
