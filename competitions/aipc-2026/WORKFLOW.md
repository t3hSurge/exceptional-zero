# AIPC 2026 — workflow and instance interface

This document defines how a new AI instance enters the competition project, what context it may receive, what kinds of contribution are legitimate, and how work is recorded.

It is a **workflow document, not an essay argument**.

The purpose is reproducibility: another model or instance should be able to enter the project without relying on conversational memory or on the current author's informal explanation of the process.

---

## 1. Project boundary

The AIPC project is an external experiment in AI-generated philosophical writing.

The public Exceptional Zero repository is research context and methodological infrastructure. It is not the source of arguments that the competition essay is supposed to defend.

The private `aipc-2026` repository contains unpublished essay work and generation records.

A new AI instance should therefore be told explicitly which of the following it is being asked to do:

- **proposal work** — formulate or refine a question without supplying its answer;
- **generation work** — independently generate philosophical arguments in response to a selected question;
- **revision work** — improve an existing AI-generated draft under generic constraints;
- **methodology work** — document what happened during a run;
- **evaluation work** — test a draft for overclaim, circularity, ambiguity, objection handling, or other defects without inventing the replacement argument unless the run explicitly permits that role.

Do not silently change roles during a run.

---

## 2. Context levels

Context should be supplied at the minimum level necessary for the task.

### Level 0 — Question only

Use for an independent generation run.

Provide:

- the selected philosophical question;
- generic competition constraints;
- generic methodological constraints;
- requested format/length.

Do **not** provide:

- Exceptional Zero conclusions;
- investigation verdicts that answer the question;
- status-table rows that settle the issue;
- hidden preferred answers;
- arguments to reproduce.

### Level 1 — Question plus neutral scaffolding

May additionally provide:

- outline headings;
- word-count targets;
- objection-section requirements;
- bibliography format;
- anonymization requirements;
- logging requirements.

Scaffolding must not encode a substantive thesis or proof strategy.

### Level 2 — Current draft

Use when revising an existing competition draft.

The draft may be supplied as an object of analysis. Its claims remain **claims of the draft**, not premises adopted by the revising instance.

The instance should distinguish:

- what the draft asserts;
- what follows from the draft's premises;
- what is unsupported;
- what is ambiguous;
- what requires revision.

A draft's conclusion is never promoted merely because it already appears in the draft.

### Level 3 — Methodology record

A later instance may inspect prior run logs to reconstruct the process for the methodology report. This is documentary work, not permission to retroactively rewrite the intellectual history of the essay.

---

## 3. Contribution boundary

The central authorship boundary is:

> **Human direction may determine the problem and the constraints; the AI must supply the substantive argument.**

Permitted human contributions include:

- choosing among question-level proposals;
- imposing generic quality constraints;
- asking for objections, counterarguments, clarification, or compression;
- requesting multiple independent drafts;
- selecting a draft for further development;
- identifying an apparent flaw without supplying the replacement argument;
- correcting factual or formatting errors where the correction does not constitute a substantive philosophical move;
- maintaining files, logs, word counts, and anonymity.

Forbidden substantive steering includes:

- supplying the desired argument;
- specifying the decisive premise or proof move;
- giving a formal model whose substantive features determine the result;
- supplying a novel objection together with its intended resolution when that resolution is the intellectual contribution;
- rewriting prose into the desired philosophical position;
- feeding prior investigation conclusions into the generation prompt as premises.

If a correction requires the human to invent the next substantive move, stop and let the AI generate that move or record the failure.

---

## 4. Epistemic discipline

All substantive claims should carry their actual epistemic status in the working record.

The project uses the following vocabulary:

- **Derived** — follows under stated assumptions or from an explicit argument.
- **Believed** — currently endorsed but not established by the available argument.
- **Boundary** — a tested route failed or a distinction has been established as a limit on inference.
- **Open** — a live question not yet settled by the available work.
- **Regulative Principle** — a methodological rule retained because it prevents an identified inference error; it is not an ontological result.

Do not use “complete at this level” as an epistemic status.

A negative result should preserve the exact failed candidate and failure mode whenever practical.

---

## 5. Anti-smuggling rule

Do not import a stronger concept through a weaker word.

In particular, distinguish:

- description from instantiation;
- structural succession from temporal passage;
- orientation from transition;
- formal transformation from actual occurrence;
- correlation from response;
- response from interiority;
- totality from unity;
- self-identity from numerical uniqueness;
- non-extendibility from totality;
- methodological prohibition from ontological impossibility.

If a conclusion requires a concept that has not itself been specified, mark the dependency instead of silently treating the concept as primitive.

---

## 6. Fresh-generation rule

For an original essay generation run:

1. Record the selected question.
2. Record the context level used.
3. Start a fresh generation session.
4. Preserve the complete prompt and response log.
5. Generate independently before importing any later critique.
6. Record substantive revisions separately from generic editing.
7. Never backfill the log to make the argument appear more independent than it was.

If the AI independently rediscovers an idea already present in the public research record, record that as a rediscovery rather than pretending the idea was historically absent.

---

## 7. Draft lifecycle

Each essay should have an explicit lifecycle:

`question → independent generation → selection → generic revision → adversarial check → finalization → methodology record`

The stages must remain distinguishable in the private repository.

A later draft may supersede an earlier draft, but the earlier draft remains part of the provenance record unless there is a specific reason to remove it.

---

## 8. Evaluation without takeover

When an AI instance is acting as evaluator rather than generator, it may identify:

- unsupported premises;
- invalid inference;
- equivocation;
- circularity;
- hidden temporal or causal assumptions;
- unhandled objections;
- ambiguity;
- scope mismatch;
- places where a conclusion exceeds what the argument establishes.

Unless the run explicitly changes roles, the evaluator should not silently repair the argument by supplying the missing substantive idea.

The cleanest record is often:

> **Here is the gap. I do not know how to close it without adding a new premise.**

That is a result, not a failure of documentation.

---

## 9. Private/public boundary

Public:

- questions;
- generic workflow;
- epistemic rules;
- competition constraints;
- provenance and ledger information that does not disclose unpublished essay text.

Private:

- essay bodies;
- generation transcripts;
- draft-specific argument development;
- unpublished outlines containing substantive argument;
- methodology records that would reveal unpublished essay content before publication.

“Off `main`” is not a privacy boundary. Public branches remain public.

---

## 10. Entry procedure for a new AI instance

A fresh instance should receive, in order:

1. this workflow;
2. the epistemology document;
3. the selected proposal/question;
4. only the minimum additional context required for the current role;
5. the current draft, if and only if the task is draft analysis or revision.

The instance should then state what role it is performing before substantive work begins.

This is intended to make the process portable across models, sessions, and collaborators.
