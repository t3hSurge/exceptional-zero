# Branching Policy

`main` is the canonical accepted state of Exceptional Zero.

## Branch types

Use short-lived descriptive branches for work that benefits from isolation or from a reviewable proposed diff:

| Prefix | Purpose | Example |
|---|---|---|
| `investigation/` | Isolate a substantive question or claim | `investigation/relational-vocabulary` |
| `proposal/` | Propose a conceptual or textual change | `proposal/status-table` |
| `revision/` | Revise an existing section | `revision/part-six` |
| `docs/` | Repository/documentation maintenance | `docs/repository-structure` |

These prefixes describe workspace purpose, not epistemic status.

## When to branch

Branch when the work benefits from isolation, parallel development, or a reviewable proposed diff. A bounded investigation may also be committed directly to `main` when it is explicitly scoped and does not alter the accepted canonical framework.

Repository maintenance and synchronization work may likewise be committed directly to `main` when the change is clearly administrative or documentary rather than an unreviewed canonical claim.

## Rule

A branch is a workspace, not an epistemic status. The existence of a branch does not mean its claims are accepted.

`main` is allowed to contain active investigation records. What distinguishes canonical acceptance is not the branch on which a claim first appears, but whether the claim has been deliberately incorporated into `exceptional-zero.md`.

## Canonical changes

Changes to `exceptional-zero.md` that alter the accepted framework should normally be proposed through a branch or otherwise receive deliberate review before entering `main`.

The canonical document must reflect exactly what the investigation established—no more and no less. A change to an investigation, index, or repository policy does not by itself promote the underlying investigation result into the canonical framework.

## Merge principle

When a branch contains a proposed canonical or substantive repository change, the branch should make the proposed change legible through its diff. Once accepted, merge it into `main` and, when the conceptual or structural change is significant, record it in `CHANGELOG.md`.

## History

Do not use branches as an alternative to Git history. Old commits already preserve the development record. Keep a branch after merge only when it has continuing value; otherwise it may be deleted without losing its commits from the merged history.
