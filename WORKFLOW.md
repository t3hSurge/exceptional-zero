# Exceptional Zero Repository Workflow

This repository is the working record of the Exceptional Zero framework: its current formulation, investigations, critiques, revisions, and superseded formulations.

## 1. Source of authority

`exceptional-zero.md` is the canonical framework.

A claim is not part of the canonical framework merely because it appears in an investigation or branch. Canonical status is conferred only by incorporation into `exceptional-zero.md` on `main`.

Git history is the authoritative revision history of the repository, including superseded formulations and ordinary document changes.

## 2. Main branch

`main` represents the accepted canonical repository state.

Changes to the canonical framework should normally reach `main` only after the proposed change has been examined and deliberately accepted.

Bounded investigations, status/index synchronization, and other repository maintenance may be committed directly to `main` when they are explicitly scoped as such and do not silently promote an unaccepted claim into the canonical framework.

## 3. Working branches

Branches are temporary workspaces for work that benefits from isolation or from a reviewable proposed diff. Use descriptive names such as:

- `investigation/relational-vocabulary`
- `proposal/status-table`
- `revision/part-six`
- `docs/repository-structure`

A branch may contain an argument, revision, experiment, or structural change without implying that the change has been accepted.

When a branch contains a proposed canonical change, review it and merge it deliberately into `main`. A rejected or abandoned branch remains part of Git history unless there is a reason to delete it.

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

An investigation may end by resolving its question, by showing that a candidate fails, or by isolating a deeper unresolved question. In the last case, the deeper question should be recorded as a new bounded investigation rather than treated as failure of the preceding investigation.

The repository may therefore contain several linked investigations that form a derivational sequence. Their relationship should be explicit, while their epistemic statuses remain distinct.

## 5. Documentation and rendering standard

Repository documentation is authored in **GitHub-compatible Markdown**. GitHub rendering is the baseline human-readable presentation; local editors such as Obsidian or Typora may provide enhanced rendering but are not required to read the documentation.

### 5.1 Mathematical notation

Use Markdown math syntax that renders consistently on GitHub and in common MathJax-based Markdown readers:

- **Inline mathematics:** `$...$`
- **Display/block mathematics:** `$$...$$`
- **LaTeX commands:** use standard MathJax/LaTeX inside those delimiters.

For example:

```markdown
The central implication is $\mathrm{Particularity}(S)\Rightarrow Z(S)$.

$$
\boxed{\mathrm{Particularity}(S)\Rightarrow Z(S)}
$$
```

Use `\boxed{...}` only inside a math block when a visual box is actually part of the intended mathematical presentation.

**Prefer display math for Markdown-sensitive expressions.** If an inline mathematical expression contains characters that can be interpreted by Markdown—especially `_`, `*`, backticks, or similar syntax—promote the expression to a `$$...$$` block rather than escaping those characters inside `$...$`. For example:

```markdown
The live architecture is:

$$
G_P,G_M\rightarrow[\sim]\rightarrow[G^*]\rightarrow\Sigma
$$
```

This is preferred to forcing a dense expression such as `$G_P,G_M\rightarrow[\sim]\rightarrow[G^*]\rightarrow\Sigma$` inline.

For simple inline identifiers with subscripts or superscripts, ordinary `$...$` is acceptable when the surrounding Markdown parser will not reinterpret the notation. When in doubt, use a display block.

**Use `\ast` instead of a raw `*` for starred mathematical symbols.** GitHub's Markdown preprocessing can reinterpret raw asterisks even inside otherwise valid math. Write `$G^\ast$`, `$G^\ast_1$`, and `$C_\ast$` rather than `$G^*$`, `$G^*_1$`, or `$C_*$`. This is especially important for symbols combining stars with subscripts, and it keeps the source portable across GitHub and MathJax-based readers.

**Do not rely on `\operatorname{...}` in repository mathematics.** GitHub's math renderer is stricter than a full MathJax environment. Use portable forms such as `\mathrm{...}` instead. For example, write `$\mathrm{Aut}(S)$` rather than `$\operatorname{Aut}(S)$`.

**Do not unnecessarily escape LaTeX subscripts inside math delimiters.** In mathematical mode, write `$G^\ast_1$` rather than `$G^*\_1$`. The escaped underscore can render incorrectly when mixed with Markdown parsing. If the expression is too Markdown-sensitive for safe inline use, move it to a display block instead.

Prefer mathematical delimiters over raw Unicode for formal expressions when the expression contains operators, superscripts, subscripts, or other structure that benefits from consistent rendering. Unicode is fine for ordinary prose and standalone symbols where it improves readability.

### 5.2 Markdown versus literal code

Use backticks for filenames, paths, literal identifiers, code, and repository structure, for example `exceptional-zero.md` or `C_*` when the identifier itself is being discussed as code/literal text. Use math delimiters when the item is being presented as mathematics, for example $C_*$.

Do not use editor-specific extensions for essential meaning or presentation. Core content should remain understandable in raw Markdown and readable in the GitHub-rendered view.

### 5.3 Scope of the standard

This rendering standard applies to canonical documents, guides, repository policy, and other maintained human-facing documentation.

`investigations/` is a historical research layer. Existing investigation files do not need to be reformatted merely to conform to this standard. New or substantially revised investigation documents should prefer the common syntax when practical, but preserving historical wording and formatting is more important than cosmetic normalization.

The **Legend of the Exceptional Zero** is the notation guide for what symbols mean; this section is the repository guide for how those symbols are written and rendered in Markdown.

### 5.4 Patch-first editing

For a surgical change to an existing document, edit the current file by patch rather than reconstructing the entire document from conversational text.

The required sequence is:

1. **Fetch the current file.** Work from the exact current revision, not from a remembered or copied earlier version.
2. **Apply the smallest textual change.** Prefer a line- or hunk-level patch for a local edit.
3. **Inspect the diff.** Confirm that every changed line is intentional before committing.
4. **Commit the verified result.** The committed snapshot should contain only the requested change and any explicitly accompanying documentation change.

A large canonical document must **not** be regenerated or pasted through an LLM write operation merely to make a local edit. Whole-file replacement is reserved for deliberate document rewrites where the complete replacement has itself been independently verified.

For canonical documents, preserving the existing text is a higher priority than convenience. If a requested edit can be expressed as a small patch, the repository should record it as a small patch in Git history.

## 6. Changelog

`CHANGELOG.md` records significant conceptual and structural changes, not routine wording edits.

Use it for changes such as:

- a claim changing epistemic status;
- a theorem or derivation being corrected;
- a scope restriction being added;
- a major concept being introduced or removed;
- a significant failed argument being documented;
- a structural reorganization that changes how the framework is read.

Git commit history remains the detailed record of all edits.

## 7. Suggested work cycle

For a substantive investigation or proposed change:

1. **State the question.** Put the issue in `investigations/` or, when isolation is useful, on an appropriately named branch.
2. **Attack the claim.** Examine hidden assumptions, scope errors, invalid inference, or counterexamples.
3. **Follow the result.** Resolve the question, record a candidate failure, or isolate a deeper question without forcing the preceding investigation to answer it.
4. **Revise the proposal.** Make the smallest change that the surviving analysis warrants.
5. **Check status.** Decide whether the result is Derived, Believed, Boundary, Open, or Regulative Principle, and whether that label is actually supported.
6. **Review the repository state.** Confirm that canonical text, investigation indexes, and other navigation documents say exactly what the investigations establish—no more and no less.
7. **Accept deliberately.** Only then incorporate an accepted conclusion into `exceptional-zero.md` on `main`.
8. **Record the milestone.** Add a concise entry to `CHANGELOG.md` when the conceptual or structural change is significant.

## 8. Epistemic discipline

The repository follows the same discipline as the framework itself:

> Nothing is stronger than its status.

A proposal may be interesting without being established. A failed search may establish a Boundary without establishing a universal negative. A polished formulation does not strengthen the underlying claim. A newly isolated question is not evidence for any answer to that question.

The repository structure is intended to preserve those distinctions rather than blur them.
