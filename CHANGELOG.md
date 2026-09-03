# Changelog

Significant conceptual and structural changes are recorded here. Routine wording edits remain in Git history.

## 2026-09-03

### Methodological enclosure (third-order)

- Added `investigations/2026-09-03-methodological-enclosure.md`.
- Isolated Methodological Enclosure as the suspected failure mode: the methodology can detect claim-failures inside its admissible space while remaining unable to detect that its admissibility conditions exclude the relevant truth.
- Recorded M1–M3 as already handled (internal error, overreach, missing candidate). Isolated M4 (missing category) as the live test.
- Specified attack families M-A (counterexample methodology), M-B (alien truth), and M-C (self-application) without constructing them.
- Recorded “Meta-Boundary” as an unadopted candidate label only. No sixth status. No canonical edit. No escape hatch.

## 2026-08-29

### Repository editing workflow

- Codified patch-first editing in `WORKFLOW.md`: maintained documents should be edited from the exact current revision by the smallest practical patch, with the diff inspected before commit.
- Prohibited reconstructing large canonical documents from conversational text for surgical edits; whole-file replacement is reserved for deliberate rewrites whose complete replacement has been independently verified.

### Canonical math-rendering cleanup

- Corrected remaining GitHub/MathJax rendering edge cases in `exceptional-zero.md` by using `\\ast` for starred mathematical symbols and moving the dense representation-invariant architecture expression to a display-math block.
- Preserved the canonical wording and epistemic content; this was a formatting-only maintenance pass.

### Legend refinement

- Tightened `guides/legend-of-the-exceptional-zero.md` into a canonical-framework-only companion to `exceptional-zero.md`.
- Removed later investigation notation and research-local symbols from the legend rather than allowing it to become a second research index.
- Kept the legend focused on canonical symbols, epistemic statuses, logical distinctions, the Actualization Boundary, and the canonical diachronic-identity architecture.
- Preserved the GitHub/MathJax-compatible formatting standard: `$...$` for inline mathematics and `$$...$$` for display mathematics.

<!-- remainder of changelog preserved in prior commits; see Git history for 2026-08-28 and earlier entries -->
