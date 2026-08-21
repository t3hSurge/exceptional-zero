# Exceptional Zero Repository Workflow

This repository is the working record of the Exceptional Zero framework: its current formulation, investigations, critiques, revisions, and superseded formulations.

## 1. Source of authority

`exceptional-zero.md` is the canonical framework.

A claim is not part of the canonical framework merely because it appears in an investigation, AI analysis, branch, issue, or archived document. Canonical status is conferred only by incorporation into `exceptional-zero.md` on `main`.

Git history is the authoritative revision history. The archive is for material worth preserving as a standalone historical artifact, not for every superseded version of the canonical document.

## 2. Main branch

`main` represents the accepted state of the framework.

Changes to the canonical framework should normally reach `main` only after the proposed change has been examined and deliberately accepted. Direct experimentation on `main` should be avoided unless explicitly authorized as repository maintenance.

## 3. Working branches

Branches are temporary workspaces for proposed changes. Use descriptive names such as:

- `investigation/relational-vocabulary`
- `proposal/status-table`
- `revision/part-six`
- `review/2026-08-20-track1`

A branch may contain an argument, revision, experiment, or structural change without implying that the change has been accepted.

When a branch is ready for consideration, it can be reviewed and merged into `main`. A rejected or abandoned branch remains part of Git history unless there is a reason to delete it.

## 4. Investigations

`investigations/` contains bounded questions, tests, counterexamples, formal checks, and other work whose purpose is to determine whether a claim should survive.

An investigation should state:

1. the question being tested;
2. the current claim or candidate formulation;
3. what would count against it;
4. the reasoning or evidence examined;
5. the result;
6. the resulting epistemic status, if one can be assigned.

An investigation does not automatically alter the canonical framework.

## 5. AI reviews

`ai-reviews/` records source analyses from AI collaborators, including substantive adversarial reviews and syntheses.

AI output is evidence of an argument having been considered, not evidence that the argument is correct. AI analyses therefore do not become canonical merely by being stored here.

Prefer one file per substantive analysis, with a date and subject in the filename. Preserve enough context to make the analysis intelligible without relying on the original chat.

A review should distinguish clearly between:

- results already established by the investigation;
- new deductions made during review;
- objections or counterexamples;
- recommendations for further testing;
- any proposed status change.

There is currently no separate `reviews/` directory. Keeping substantive reviews under `ai-reviews/<source>/` preserves both review function and source provenance.

## 6. Archive

`archive/` contains superseded formulations or other historical artifacts that are useful to preserve as documents in their own right.

Do **not** copy every old version of `exceptional-zero.md` into the archive. Git already preserves those versions and their diffs.

Archive a document when its historical or conceptual identity matters independently of Git history—for example, a substantially different framework formulation, a discarded formalization, or a milestone report.

Archived material is not authoritative unless the canonical framework explicitly incorporates a result from it.

## 7. Changelog

`CHANGELOG.md` records significant conceptual changes to the framework, not routine wording edits.

Use it for changes such as:

- a claim changing epistemic status;
- a theorem or derivation being corrected;
- a scope restriction being added;
- a major concept being introduced or removed;
- a significant failed argument being documented;
- a structural reorganization that changes how the framework is read.

Git commit history remains the detailed record of all edits.

## 8. Suggested review cycle

For a substantive proposed change:

1. **State the question.** Put the issue in `investigations/` or an appropriately named branch.
2. **Attack the claim.** Reviewers, including AI collaborators where useful, should look specifically for hidden assumptions, scope errors, invalid inference, or counterexamples.
3. **Record useful source analyses.** Preserve substantive AI analyses in `ai-reviews/` when they are worth retaining as source material.
4. **Run substantive review.** When open investigations exist and no separate framework question is active, review those investigations directly and record the strongest findings in `ai-reviews/` under the reviewing source.
5. **Revise the proposal.** Make the smallest change that the surviving analysis warrants.
6. **Check status.** Decide whether the result is Derived, Believed, Boundary, Open, or Regulative Principle, and whether that label is actually supported.
7. **Review the diff.** Confirm that the canonical text says exactly what the investigation established—no more and no less.
8. **Merge deliberately.** Only then incorporate accepted conclusions into `main`.
9. **Record the milestone.** Add a concise entry to `CHANGELOG.md` when the conceptual change is significant.

## 9. Epistemic discipline

The repository follows the same discipline as the framework itself:

> Nothing is stronger than its status.

A proposal may be interesting without being established. A failed search may establish a Boundary without establishing a universal negative. Agreement from an AI collaborator does not turn a belief into a derivation. A polished formulation does not strengthen the underlying claim.

The repository structure is intended to preserve those distinctions rather than blur them.
