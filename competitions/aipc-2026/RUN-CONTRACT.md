# Run contracts

One contract per generation pass. Fill the fields before the first prompt. Do not start a pass with an empty contract.

The methodology report should point here and to `logs/`, not reconstruct process from memory.

---

## Template

```
Run ID:
Topic:
Model:
Date:
Allowed human interventions:
Forbidden interventions:
Prompt provenance:
Number of independent drafts:
Selection procedure:
Revision procedure:
Log location:
Final submission hash:
```

---

## T1-A — not started

```
Run ID: T1-A
Topic: Can “atemporal” be specified without presupposing the temporal or performative content it is meant to exclude?
Model:
Date:
Allowed human interventions: topic question; generic method (objections-and-replies; ≤6000 words; no overclaim); argument-agnostic expand/cut/consider-author after draft exists.
Forbidden interventions: supplied arguments; formal-model spec; EZ premises/conclusions/terminology-as-result; next philosophical move at a stall; human prose in the essay body; cross-read of T1-B before both drafts exist.
Prompt provenance: question + generic constraints only. No AT batteries, no O1/O2, no investigation endpoints.
Number of independent drafts: this file is draft A of two. No cross-pollination with T1-B before selection.
Selection procedure: after T1-A and T1-B both exist, human may choose one or neither.
Revision procedure: argument-agnostic only. Stall → name the stall; do not supply the next move.
Log location: logs/T1-A/
Final submission hash:
```

## T1-B — not started

```
Run ID: T1-B
Topic: same question as T1-A
Model:
Date:
Allowed human interventions: same as T1-A
Forbidden interventions: same as T1-A, plus no cross-read of T1-A before both drafts exist
Prompt provenance: same constraint as T1-A; independent session
Number of independent drafts: this file is draft B of two
Selection procedure: after both drafts exist
Revision procedure: same as T1-A
Log location: logs/T1-B/
Final submission hash:
```

T2 and T3 have no contracts until T1-A/T1-B exist and a selection decision is recorded.
