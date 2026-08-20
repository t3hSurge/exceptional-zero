# Investigation: Diachronic Identity — UCL Junction Rules

**Date:** 2026-08-20  
**Status:** Open / current round tested  
**Related investigation:** `investigations/2026-08-20-diachron-identity-causal-provenance-survivor.md`

---

## 1. Question

With the origin predicate \(O\) held fixed and independently specified, can the Unique Causal Lineage (UCL) candidate be completed by an independently specified rule for branching and merging that partitions temporal stages into coherent lineage segments without consulting the pre-theoretic identity verdict?

The pressure battery is:

- pure branch;
- pure merge;
- branch followed by later merge;
- overdetermined causation;
- shared origin followed by divergence;
- total reconstruction from original parts;
- gradual replacement;
- temporal discontinuity.

The question is not which rule best matches intuition. It is which rules are mathematically coherent, independently specified, and what identity-theoretic commitments they actually impose.

---

## 2. Setup

Fix a temporal causal structure with:

- domain \(D\) of stages/events;
- a previously specified causal relation \(C\);
- an independently specified origin predicate \(O\);
- no identity predicate.

A candidate lineage relation must be a relation on stages derived only from this structure.

The previous UCL proposal used a **non-branching continuation** condition but had not fixed how a lineage should be segmented at junctions. That omission is the present target.

---

## 3. Candidate J0 — Causal connectivity

**Rule:** Any two stages connected by a causal path belong to the same lineage.

### Branch

\[
A\to B,\qquad A\to C.
\]

Then both \(B\) and \(C\) remain in the same lineage as \(A\).

### Fission

This yields one predecessor that is identical with two distinct successors. That violates ordinary numerical identity if the lineage relation is supposed to be identity.

### Merge

\[
A\to C\leftarrow B.
\]

Then \(C\) belongs to both lineages.

### Verdict

**Fails.** Causal connectivity is too coarse. It is a connectedness relation, not a workable identity relation.

---

## 4. Candidate J1 — Cut at every branching or merging junction

Define the junction set \(J\) as stages/events at which the relevant causal graph has either:

- more than one relevant successor, or
- more than one relevant predecessor.

Remove those junction points from the continuation relation and define a lineage segment as a maximal connected non-junction path.

Equivalently: a predecessor lineage ends at a branch or merge; successor continuation begins as a new segment after the junction.

### Pure branch

\[
A\to\{B,C\}.
\]

The lineage containing \(A\) terminates at the branch. \(B\) and \(C\) begin distinct successor segments.

Thus neither \(B\) nor \(C\) is identical with \(A\), and \(B\) and \(C\) are distinct from each other.

### Pure merge

\[
A\to C\leftarrow B.
\]

The lineages containing \(A\) and \(B\) terminate at the merge; \(C\) begins a new segment.

Thus \(C\) is not identical with either predecessor.

### Branch then later merge

\[
A\to\{B,C\}\to D.
\]

The two successor segments remain distinct. If they later merge:

\[
B,C\to D,
\]

both terminate and a new segment begins at \(D\).

There is no ambiguity or inheritance conflict.

### Overdetermined causation

Suppose two causes contribute to \(C\) without the graph representing a merger of two candidate identities. Under J1, the formal result depends entirely on whether the causal relation \(C\) counts those influences as distinct predecessors.

That is not a defect in J1 itself. It exposes a separate requirement: the *relevant causal relation* must already be specified independently. Otherwise ordinary environmental causation can create junctions everywhere and make persistent identity impossible.

### Shared origin + later divergence

One origin can generate multiple non-branching segments after divergence, but the pre-divergence segment terminates at the divergence. Thus shared origin does not imply shared identity after branching.

### Reconstruction from original parts

A later reconstruction from parts of an earlier object is not on the same uninterrupted causal lineage as the original process unless the causal relation explicitly contains that restoration as continuation. J1 therefore yields non-identity by default.

### Gradual replacement

No junction occurs merely because parts are replaced one at a time, so the lineage continues.

### Temporal discontinuity

A time gap does not itself create a junction. A continuing causal edge or chain can cross the gap.

### Formal property

J1 can be made into a genuine equivalence relation: “belongs to the same maximal non-junction path segment.” Reflexivity, symmetry, and transitivity follow from segment membership.

### Verdict

**Survives the graph-theoretic junction battery.**

But it does not by itself establish personal identity. Its crucial unresolved dependency is the prior specification of which causal relation counts as identity-relevant.

---

## 5. Candidate J2 — Privileged-parent inheritance at a merge

At a merge:

\[
A\to C\leftarrow B,
\]

choose one parent as the identity-bearing predecessor.

### Pressure

The rule requires a criterion for why \(A\) rather than \(B\) is privileged.

Possible criteria include greater causal contribution, temporal priority, material majority, informational dominance, or functional dominance.

None is built into “merge” itself. Each introduces an additional selection principle that must be independently specified.

### Automorphism pressure

If the two parents are structurally symmetric, any choice of one is arbitrary under automorphism. Privileging one therefore requires an additional asymmetry outside the base graph or a target-shaped stipulation.

### Verdict

**Fails as an unqualified rule.** A domain-specific privileged-parent criterion could be proposed, but that would reopen origin/selection rather than solve the junction problem generally.

---

## 6. Candidate J3 — All-parent inheritance at a merge

Declare the merged stage identical with every contributing parent.

### Pressure

If \(A\neq B\), then:

\[
A\equiv C\land B\equiv C
\]

would imply:

\[
A\equiv B,
\]

contradicting numerical distinction.

### Verdict

**Fails.** It makes the purported identity relation non-consistent with ordinary identity.

---

## 7. Candidate J4 — New identity only at branch, not at merge

Terminate lineage at branching but allow one or more predecessors to continue through a merger.

### Pressure

At a merge, the successor would have to inherit from at least one predecessor. If it inherits from both, J3 returns. If it inherits from one, J2 returns.

There is no independent third option.

### Verdict

**Collapses into J2 or J3.** No independent survivor.

---

## 8. Candidate J5 — New lineage at every junction

This is the abstract formulation of J1:

> A lineage is a maximal interval of the causal graph containing no node with more than one relevant incoming or outgoing continuation edge.

It is deterministic and graph-invariant once the relevant causal relation has been fixed.

Its consequences are explicit:

- branch terminates the predecessor lineage;
- merge terminates all predecessor lineages;
- the junction begins a new lineage;
- later divergence begins new lineages again;
- reconstruction begins a new lineage unless the causal relation explicitly makes it continuous.

### Verdict

**Coherent as a partition rule.** It is the strongest currently surviving junction rule.

However, the same unresolved issue remains: the rule partitions whatever graph was supplied. It does not independently tell us which causal edges belong to the identity-relevant graph.

---

## 9. Candidate J6 — Choose junction behavior by preservation of pre-theoretic identity intuitions

Examples:

- preserve identity through gradual reconstruction if intuitively desired;
- preserve one branch if one feels psychologically continuous;
- terminate identity at fusion only when numerical identity would otherwise become ambiguous.

### Verdict

**Disqualified.** This is a target-selection rule disguised as a junction rule. It consults the identity verdict to determine the formal partition it was supposed to explain.

---

## 10. Battery summary

| Rule | Branch | Merge | Branch→Merge | Circularity | Partition | Verdict |
|---|---|---|---|---|---|---|
| J0 Causal connectivity | Fails | Fails | Fails | Pass | Too coarse | Reject |
| J1 Cut at every junction | Pass | Pass | Pass | Pass | Yes | **Survives** |
| J2 Privileged parent | Requires criterion | Requires criterion | Requires criterion | Risky | Yes only after extra rule | Reject pending new criterion |
| J3 All-parent inheritance | Fails identity | Fails | Fails | Pass | No coherent identity | Reject |
| J4 Branch-only termination | Pass | Collapses to J2/J3 | Fails | Risky | Not independent | Reject |
| J5 New lineage at every junction | Pass | Pass | Pass | Pass | Yes | **Survives; equivalent to J1** |
| J6 Intuition-preserving | Variable | Variable | Variable | **Fails** | Variable | Reject |

J1 and J5 are not competing theories. They are two descriptions of the same surviving partition rule.

---

## 11. The important result

The junction problem is **not** itself the fatal flaw we expected.

A clean, independently specified partition rule exists:

\[
\boxed{
\text{cut the lineage at every relevant causal branch or merge}
}
\]

This yields equivalence classes of maximal non-junction paths.

That solves the purely mathematical partition problem.

But it exposes a deeper dependency one level earlier:

> **What makes a causal relation “relevant” to identity?**

If every physical causal influence counts, then ordinary objects participate in enormous branching causal graphs and UCL becomes unusably fragmented. If only a selected class of causal edges counts, that selection requires its own independent criterion.

Therefore the architecture now has three layers:

\[
\boxed{
\text{causal-relation admissibility}
\rightarrow
\text{origin admissibility}
\rightarrow
\text{junction partitioning}
}
\]

The junction problem can be solved formally, but only after the relevant causal relation is fixed.

---

## 12. Current status

**Junction partition rule:** Strong provisional survivor.

J1/J5 is independently specified, graph-invariant, deterministic, and produces a genuine equivalence partition of stages once the relevant causal graph is fixed.

**UCL as full identity theory:** Still Open.

The remaining unresolved question is now more fundamental than the junction problem:

> What principled, non-target-bearing criterion selects the causal relation whose branches and merges are identity-relevant?

No status upgrade is warranted for UCL as a whole yet.

---

## 13. Next pressure test

Do not generate more junction rules. The surviving junction rule is now fixed for purposes of further testing.

The next investigation should hold J1/J5 fixed and pressure-test the **causal relation itself** against:

- ordinary environmental causation;
- epigenetic and developmental influence;
- social and linguistic causation;
- component-level causation;
- overdetermined causes;
- causal chains with irrelevant side effects;
- clone creation;
- restoration and repair.

The question is whether an independently specified causal relation can be selected without making “identity-relevant cause” the criterion in disguise.
