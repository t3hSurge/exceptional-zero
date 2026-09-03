# AIPC 2026 generation protocol

This protocol exists so the essays can meet the competition’s AI-authorship rule. It is stricter than the Exceptional Zero research method.

Heuristic from the rules: **AI should be the sole author.** Humans may provide corrective guidance and direction. Essays with insufficient AI involvement are ineligible for prizes.

---

## Permitted human acts

These track the official examples.

1. Choose a topic as a *question*, not as an argument.
2. Apply generic method constraints: address prominent objections; include an objections-and-replies section; stay under 6,000 words; do not claim more than is argued; distinguish derived / believed / open if the AI itself adopts a status vocabulary.
3. Ask the AI to generate multiple independent drafts and select among them.
4. Give argument-agnostic direction: expand this paragraph; consider this published author; add a technical appendix; cut for length; anonymize.
5. Build argument-agnostic scaffolds (file layout, word-count checks, log retention).

---

## Forbidden human acts

These track the official “not permitted” list.

1. Supply an argument (“refute X *by the following argument*”).
2. Specify a formal model’s features in advance (“create a model with X, Y, and Z”).
3. Conduct rigorous critique that *gives the AI significant ideas*.
4. Write essay prose.
5. Paste Exceptional Zero results, status-table rows, or investigation conclusions into the essay as content to defend.
6. Prompt-inject the judges.

Corrective guidance that only flags overclaim, circularity, or missing objection *without offering the replacement argument* is the intended human role. If a correction would require inventing the next move, stop and let the AI invent it or fail.

---

## Relation to Exceptional Zero

The EZ process (adversarial co-construction, status locks, refusal to promote) is **not** the essay-generation protocol.

It may appear in the methodology report as:

- background for topic selection;
- a description of a prior research method that this competition run is *not* using for the essay body.

It may not appear in the essay as imported theorems.

If an essay independently rediscovers something already in the repo, that is allowed only if the rediscovery is produced under this protocol and is not fed in by the human.

---

## Run shape (one essay)

1. Human records the topic question in `TOPICS.md`.
2. AI produces at least two independent drafts with no EZ text in the prompt.
3. Human may select a draft and request generic revision.
4. AI revises. Human does not insert arguments.
5. Word count ≤ 6,000 excluding bibliography.
6. Full chat log stored under `logs/`.
7. Human does not treat the finished essay as a status change for the canonical framework.

---

## Anonymity

Essays and the methodology report must be anonymized for review. Do not include the GitHub repo name, “Exceptional Zero” as a claimed prior publication, or personal identifiers in the essay body. The methodology report may describe the method without naming the public repo if that would break anonymity; the organizers still see identity.
