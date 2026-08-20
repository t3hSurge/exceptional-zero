# Branching Policy

`main` is the canonical accepted state of Exceptional Zero.

## Branch types

Use short-lived descriptive branches for work that is not yet accepted:

| Prefix | Purpose | Example |
|---|---|---|
| `investigation/` | Test a question or claim | `investigation/relational-vocabulary` |
| `proposal/` | Propose a conceptual or textual change | `proposal/status-table` |
| `revision/` | Revise an existing section | `revision/part-six` |
| `review/` | Preserve or organize a review pass | `review/claude-2026-08-20` |
| `docs/` | Repository/documentation maintenance | `docs/repository-structure` |

## Rule

A branch is a workspace, not an epistemic status. The existence of a branch does not mean its claims are accepted.

## Merge principle

Substantive changes should be reviewed before entering `main`. The branch should make the proposed change legible through its diff. Once accepted, merge the branch and, when the conceptual change is significant, record it in `CHANGELOG.md`.

## History

Do not use branches as an alternative to Git history. Old commits already preserve the development record. Keep a branch after merge only when it has continuing value; otherwise it may be deleted without losing its commits from the merged history.
