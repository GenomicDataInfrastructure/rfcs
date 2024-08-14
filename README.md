# Genomic Data Infrastructure RFCs
## UNDER CONSTRUCTION - Not ready for RFCs
The RFC process is still under construction, and needs to be well-defined and accepted before it can process RFCs.

As such, contributions should be strictly limited to the process and the documents around it.

## What is an RFC?

The "RFC" (request for comments) process is intended to provide a
consistent and controlled path for new features or processes to enter into production.

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put
through a bit of a design process and produce a consensus among the service providers, product owners and decision makers of the infrastructure.

## The RFC life-cycle

An RFC goes through the following stages:

- **Pending:** when the RFC is submitted as a discussion thread. We use discussions instead of Pull Requests as the former provides better discussion threading.
- **Active:** when an RFC is acknowledged and undergoing implementation. The feature may be shipped as experimental during this phase.
- **Landed:** when an RFC's proposed changes are shipped as stable in a release.
- **Rejected:** when an RFC is officially rejected or dropped.

## When to follow this process

You need to follow this process if you intend to make "substantial" changes.

What constitutes a "substantial" change is evolving based on community norms, but may include the following:

- A new feature that creates new API surface area
- Changing the semantics or behavior of an existing API
- The removal of features that are already shipped as part of the release channel
- New process or operational procedure.

Some API changes do not require an RFC:

- Additions that strictly improve objective, numerical quality criteria
- Fixing objectively incorrect behavior
- Rephrasing, reorganizing or refactoring
- Addition or removal of warnings

# Gathering feedback before submitting

It's often helpful to get feedback on your concept before diving into the
level of API design detail required for an RFC. **You may open an
issue on this repo to start a high-level discussion**, with the goal of
eventually formulating an RFC pull request with the specific implementation
design.

## What the process is

In short, to get a major change in GDI, one must first get the
RFC merged into the RFC repo as a markdown file. At that point the RFC
is 'active' and may be implemented.

1.  Work on your proposal in a Markdown file based on the template (`0000-template.md`) found in this repo.

    - Put care into the details: **RFCs that do not present convincing motivation, demonstrate understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly-received**.

2.  Open a new thread in [Discussions](https://github.com/GenomicDataInfrastructure/rfcs/discussions) and make sure to set category to "RFC Discussions".

    - Build consensus and integrate feedback in the discussion thread. RFCs that have broad support are much more likely to make progress than those that don't receive any comments.

3.  Eventually, the (TODO: AC Process) will decide whether the RFC is a candidate
    for inclusion in GDI.

    - An RFC can be modified based upon feedback from the (TODO: AC process). Significant modifications may trigger a new final comment period.

    - An RFC may be rejected after public discussion has settled and comments have been made summarizing the rationale for rejection. A member of the (TODO: AC Process) should then close the RFC's associated pull request.

    - An RFC may be accepted at the close of its final comment period. A (TODO: AC Process) member will merge the RFC's associated pull request, at which point the RFC will become 'active'.

4.  If the proposal has been approved for inclusion, you can prepare a Pull Request:

    - Fork this repo.

    - Create your proposal as `active-rfcs/0000-my-change.md` (where "my-change" is descriptive. don't assign an RFC number yet).

    - Submit a pull request. Make sure to link to the discussion thread.

## Details on Active RFCs

TODO: Rephrase section below

Once an RFC becomes active then authors may implement it and submit the
feature as a pull request to the repo. Becoming 'active' is not a rubber stamp, and in particular still does not mean the feature or process will ultimately
be merged; it does mean that the approver(s) defined in the acceptance criteria have agreed to it in principle
and are amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is
'active' implies nothing about what priority is assigned to its
implementation, nor whether anybody is currently working on it.

Modifications to active RFC's can be done in followup PR's. We strive
to write each RFC in a manner that it will reflect the final design of
the feature; but the nature of the process means that we cannot expect
every merged RFC to actually reflect what the end result will be at
the time of the next major release; therefore we try to keep each RFC
document somewhat in sync with the language feature as planned,
tracking such changes via followup pull requests to the document.

## Implementing an RFC

The author of an RFC is not obligated to implement it. Of course, the
RFC author (like any other developer) is welcome to post an
implementation for review after the RFC has been accepted.

An active RFC should have the link to the implementation PR listed if there is one. Feedback to the actual implementation should be conducted in the implementation PR instead of the original RFC PR.

If you are interested in working on the implementation for an 'active'
RFC, but cannot determine if someone else is already working on it,
feel free to ask (e.g. by leaving a comment on the associated issue).

## Reviewing RFC's

Members of the approver(s), defined in the AC depending on their expertise, role w.r.t. GDI, governance, or GDI reviewing role, will attempt to review some set of the open RFC
pull requests on a regular basis. If an approver believes an RFC PR is ready to be accepted into active status, they can approve the PR using GitHub's review feature to signal their approval of the RFC. The approvers may review the RFC using an alternate collaborative tool, although the history of the RFC should be preserved, hence the preferrence for GitHub. 

**GDI's RFC process owes its inspiration to the [Vue RFC process](https://github.com/vuejs/rfcs)**
