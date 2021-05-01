# RFCs (Requests for Comments)

This repo contains all RFCs for Project MAE.

## When to use RFCs

In Project MAE, RFCs are to be used for all major decisions, while minor
implementation-specific details may be resolved without going through the RFC
process.

## Creating an RFC

1. Create a branch, either on a fork or this repo that has a short, descriptive name
   of your RFC.
2. On the branch, copy `0000-template.md` to  `text/0000-<name>.md`, where `<name>`
   is replaced by the name of your suggestion Do _not_ assign a RFC number - this is
   the PR number and will be added later.
3. Populate your RFC markdown file with a detailed description of your suggestion(s).
   - __Important: the template is just that - a template. It is not necessary to use
     all sections, answer all questions. Use the questions as guides rather than
     prompts.__
4. Once your document is complete, open a **draft** pull request to the `main` branch
   of this repo.
5. At this time, the document will be assigned a RFC number. Please rename your
   document accordingly, replacing `0000` with the RFC number, preceded by zeroes
   such that the number takes up four characters:
    - e.g. RFC #554 will be `text/0554-....`
    - e.g. RFC #1 will be `text/0001-....`
6. Continue working on the RFC, making edits as necessary.
7. Once all edits are finalized, mark the PR ready for review.
8. Upon passing initial review, the RFC will be marked as *active*.
    - Once an RFC is active, it is open to: community debate, implementations
      submitted as PRs (if applicable), etc.
9. After a period of 14 days, the RFC will be merged, unless it has been
   denied/closed as an active RFC.

***Note: Merging of an RFC does not guarantee its implementation, only that it has
been acquesied to. Anyone is free to implement an RFC and submit a PR.***

_Inspired by and adapted from the [Rust RFC
process](https://github.com/rust-lang/rfcs)._
