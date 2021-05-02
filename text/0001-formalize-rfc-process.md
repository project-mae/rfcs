# Request for Comments

- Feature Name: `formalize-rfc-process`
- Start Date: 2021-05-02
- RFC PR: [project-mae/rfcs#0001](https://github.com/project-mae/rfcs/pull/0001)

<!--

DO NOT REMOVE THIS BLOCK. If any amendments are made by future RFCs or decision,
please open a Pull Request to document links to these amendments here. Also,
uncomment the following section of the block as the template for documenting
templates.

## Amendments

- Amended by: [project-mae/rfcs#0000](https://github.com/pro/rfcs/pull/0000) (if applicable)
  - Description: One sentence description of amendment

-->

## Summary

[summary]: #summary

This RFC creates a formal process to document and discuss major changes to the
structure of MAE, via the adoption of the system described in
[`README.md`](../README.md) and [`0000-template.md`](../0000-template.md) in this
repository, and influenced by the [Rust language RFC
system](https://github.com/rust-lang/rfcs/blob/master/0000-template.md).

## Motivation

[motivation]: #motivation

The RFC process is a widely used process that allows for all parties/stakeholders to
present ideas and views for consideration in larger decisions that may impact those
parties/stakeholders, and creates a rigorous process for approval of new ideas into
MAE to ensure greater success.

## Explanation

[basic-explanation]: #basic-explanation

As explained in [`README.md`](../README.md), anyone may open a RFC to MAE (such as
this one), detailing requested changes to MAE, and opening a public forum of
discussion regarding this topic. Once accepted as a valid RFC, the pull request will
be changed to `active` from `draft`, and a 7-day discussion period regarding the RFC
will be opened. Excepting any major opposition to the RFC, the RFC will automatically
be approved at the end of the 7 days, and willl then be open for implementation. An
RFC being merged, however, does not guarantee implementation in any way.

## Reference

[reference]: #reference

### RFC creation

When an RFC idea is created, the user will switch either (a): to another branch
within the RFC repository, or to a personal fork of the RFC repository, and copy the
[`0000-template.md`](../0000-template.md) file to `text/0000-<name>.md` (where name
is changed to a descriptive, lowercase, snake-case name that is identical to the
feature name field on the document). The user will then make any relevant edits to
the template provided, while avoiding changes to the rfc tracking link given at the
top of the page.

The user will then create a pull request to the `main` branch of this repository to
initiate the RFC approval process. The pull request may contain one and only one
file, the `text/0000-template.md` file. The pull request must be created with the
option to allow repository maintainers to edit the file, and be a `draft` pull
request.

### Receival of RFC

When a prospective RFC is received, it will be assigned an RFC number that is
identical to the pull-request number assigned to the created pull request for the
RFC. Then, the RFC file-name will be changed (either manually or automatically) to
reflect the correct pull request number, and the tracking link on the document will
be updated to point to the correct pull request link.

### Activation

Before the RFC is approved, it must be looked over by one of the following in order
to gain activation to become a RFC:

- at least two authorized MAE members, including one manager, _including_ the
  manager(s) of the team(s) it most directly impacts
- a visionary

#### Rights of Visionaries

Visionaries may, at any time, deny the approval of a prospective RFC.

### Comments

Upon becoming approved, the RFC's pull request shall be marked as `active` (either
manually or automatically), and a 7-day period will be started during which time the
RFC may be commented on, unless permitted by a visionary, in which circumstances a
RFC's request phase may be shortened to a minimum of 24 hours.

During this time, any and all amendments, contributions, and suggestions to the RFC
are open, and will be implemented if reasonably considered.

At the end of this period, the RFC will be considered merged, excepting any valid
concerns or challenges to it which may indefinetely extend the RFC, and will be both:

- merged on GitHub
- considered a formal part of MAE

#### Rights of Managers

Managers may prevent the merging of RFCs that directly impact their teams, as subject
to review by other managers and visionaries.

#### Rights of visionaries

Visionaries may, at any time, deny the merging of a RFC.

### Merged RFCs

The implementation of merged RFCs is not guaranteed, but rather **allowed**. Any
major changes must go through the RFC process, but the merging of an RFC does not
signify the implementation of a change. Pull requests for RFCs may be opened once the
RFC has been activated, but may not be merged into their respective repos until the
RFC itself is merged into MAE.

### This RFC

This RFC, specifically, must be approved by the unanimous consent, or without
objection, by the managers and visionaries, as no prior consensus is present about
major changes.

## Drawbacks

[drawbacks]: #drawbacks

The RFC process may be cumbersome, and the over-formalization of such a process may
lead to it existing only in theory, and the _de facto_ method for approving changes
may become more informal.

## Rationale and alternatives

[rationale-and-alternatives]: #rationale-and-alternatives

The usage of the RFC process for major changes is a compromise between the informal
and formal decision systems in order to create rapid implementation while still
enabling everyone to share their opinions for major changes.

The two alternatives are:

- **Completely informal decision-making**: Under this system, all decisions would be
  made in an informal setting over voice or text.

- **Completely formal RFC process**: Under this system, all decisions- major or
  minor, must be made via RFC.

The system chosen is the best system as it provides flexibility between the two
systems depending on type of changes requested - minor ones are informal, while
broader ones are more formal.

## Precedent

[precedent]: #precedent

This system is directly inspired by the Rust Programming Language's system of
[RFCs](https://github.com/rust-lang/rfcs/blob/master/0000-template.md). It has been
adapted into our RFC process and structure as evident in [`README.md`](../README.md)
and [the RFC template](../0000-template.md).

## Unresolved questions

[unresolved-questions]: #unresolved-questions

- How will RFC amendments be addressed? Will they follow a more rigorous set of
  guidelines?

## Future possibilities

[future-possibilities]: #future-possibilities

Future possibilites to enhance RFCs include the creation of a bot/ci that
automatically checks and approves RFCS, opening discussion earlier, and
automatically-merges them unless instructed not to.
