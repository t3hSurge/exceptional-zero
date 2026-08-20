# Review: Diachronic Identity — UCL Junction Rules

**Date:** 2026-08-20  
**Reviewed investigation:** `investigations/2026-08-20-diachron-identity-ucl-junction-rules.md`  
**Status of review:** Complete for the current round  
**Framework status affected:** None; this document records the review and does not itself alter canonical status.

---

## 1. Executive finding

The junction problem does not defeat UCL at the purely mathematical level.

A clean rule survives:

> **Cut lineage at every relevant causal branch or merge; define each maximal non-junction path as one lineage segment.**

This rule is independently specifiable, deterministic, invariant under graph isomorphism, and yields a genuine equivalence partition once the relevant causal graph is fixed.

But that success exposes a deeper problem rather than completing UCL:

> **What independently specifies which causal relation counts as the identity-relevant graph?**

The junction rule partitions the supplied graph. It cannot decide which causal edges belong in that graph without another criterion.

Thus the architecture now has three logically separate layers:

\[
\boxed{
\text{causal-relation admissibility}
\rightarrow
\text{origin admissibility}
\rightarrow
\text{junction partitioning}
}
\]

The third layer has a provisional survivor. The first remains the decisive unresolved problem.

---

## 2. Candidate J0 — causal connectivity

Treat every causally connected stage as belonging to one lineage.

This fails immediately under fission. If:

\[
A\to B,
\qquad A\to C,
\]

then both B and C remain connected to A, producing one putative identity with two distinct successors.

It also fails under fusion because:

\[
A\to C\leftarrow B
\]

places C in the lineage of both A and B.

**Verdict: reject.**

The failure is structural, not merely intuitive.

---

## 3. Candidate J1/J5 — cut at every relevant junction

The surviving rule defines a junction as a node with more than one relevant predecessor or more than one relevant successor. Lineage ends at every such junction, and a new lineage segment begins afterward.

This rule survives:

- pure branching;
- pure merging;
- branch followed by merge;
- shared origin followed by divergence;
- temporal gaps;
- gradual replacement;
- reconstruction as a new lineage.

The key formal fact is that maximal non-junction path membership induces equivalence classes. Reflexivity is immediate. Symmetry follows from common segment membership. Transitivity follows because two stages sharing the same maximal segment belong to the same segment.

So the earlier worry—“perhaps non-branching does not actually define an equivalence relation”—is resolved.

**Verdict: survives as a formal partition rule.**

---

## 4. Candidate J2 — privileged-parent inheritance

At a merge:

\[
A\to C\leftarrow B,
\]

choose one predecessor to carry identity forward.

The problem is not logical incoherence. The problem is the additional selection criterion required to make the choice.

Possible selectors—greater causal contribution, temporal priority, material majority, functional dominance—are all further assumptions. If A and B are structurally symmetric, choosing one without an independent asymmetry is arbitrary under the automorphism framework.

**Verdict: reject pending an entirely new independently specified selector.**

For the present UCL investigation, generating such selectors would simply move the unresolved problem to another name.

---

## 5. Candidate J3 — all-parent inheritance

Allow a merged stage to remain identical with every predecessor.

This directly conflicts with numerical identity:

\[
A\equiv C\land B\equiv C\Rightarrow A\equiv B.
\]

If A and B are distinct, the rule is inconsistent.

**Verdict: reject.**

---

## 6. Candidate J4 — terminate at branches but inherit through merges

This looks initially different from J2/J3, but the merge case forces the same choice.

If C inherits from one predecessor, J2 returns. If it inherits from both, J3 returns. If it inherits from neither, it becomes a new lineage and the rule becomes J1/J5.

**Verdict: no independent survivor.**

---

## 7. Candidate J6 — preserve pre-theoretic identity intuitions

Rules of the form “keep identity when we think it should continue” fail the anti-circularity check. The rule consults the identity verdict it is supposed to derive.

**Verdict: disqualified.**

This is exactly Construction B at the level of junction handling.

---

## 8. The real discovery: relevant causation is now the bottleneck

J1/J5 solves the partition problem only relative to a specified graph.

But ordinary causation is massively branching. A human's state causes countless environmental, bodily, social, linguistic, and downstream effects. If every such edge counts, then almost every stage sits inside a huge branching graph and the junction rule terminates lineages constantly.

Therefore UCL cannot simply say:

> “Use causation.”

It must say:

> “Use **this particular causal relation** C.”

And that is the next candidate-selection problem.

The candidate cannot be:

> “the causal relation that preserves personal identity.”

That is Construction B again.

Nor can it merely be:

> “the causal relation relevant to the object.”

because “relevant” now performs the selection work without an independent criterion.

The central unresolved question is therefore:

\[
\boxed{
\text{What makes a causal edge identity-relevant without identity already being assumed?}
}
\]

This is substantially sharper than the previous junction question.

---

## 9. Pressure-test outcome by case

### Pure branch

J1 handles it cleanly: predecessor lineage terminates; distinct successor segments begin.

### Pure merge

J1 handles it cleanly: predecessor lineages terminate; a new segment begins.

### Branch then later merge

Each branch is distinct; the later merger creates a new segment. No identity class is forced to split and recombine.

### Overdetermined causation

The formal rule is neutral. Whether overdetermined causes create a junction depends on whether they are included as multiple predecessors in C. This means overdetermination has not been solved—it has exposed dependence on causal-relation admissibility.

### Shared origin plus later divergence

The common lineage ends at divergence. Distinct successor lineages result. This is coherent but commits UCL to identity termination at branching.

### Total reconstruction from original parts

Absent a continuous C-path, reconstruction starts a new segment. This distinguishes historical continuation from material reuse.

### Temporal discontinuity

A gap in time does not matter if C connects the stages across it. This preserves one lineage without appealing to memory.

### Gradual replacement

Replacement does not create a junction unless the chosen C-relation itself introduces one. UCL therefore survives Theseus-style replacement at the graph level.

---

## 10. What this does to the status of UCL

This round strengthens, rather than weakens, the provisional survivor result.

The earlier concern was:

> perhaps non-branching continuation cannot even produce a coherent identity relation.

The answer is now:

> it can, provided “relevant causal relation” is fixed.

But it simultaneously reveals the deeper burden:

> fixing the relevant causal relation may be doing the work that “origin” was previously suspected of doing.

So UCL still has not become a theory of diachronic identity.

Its strongest present form is:

\[
\boxed{
O + C_{*} + J_{\mathrm{cut}}
}
\]

where:

- \(O\) is an independently specified origin predicate;
- \(C_{*}\) is an independently specified identity-relevant causal relation;
- \(J_{\mathrm{cut}}\) cuts lineage at every branch or merge in \(C_{*}\).

We now know that \(J_{\mathrm{cut}}\) is not the principal unresolved component. \(C_{*}\) is.

---

## 11. Recommended next test

Do not generate more junction rules.

Hold:

\[
J_{\mathrm{cut}}
\]

fixed.

The next investigation should test candidate definitions of \(C_{*}\) against:

- ordinary environmental causation;
- developmental and biological causation;
- social and linguistic causation;
- component-level causation;
- causal overdetermination;
- irrelevant side effects;
- cloning;
- restoration;
- repair and replacement;
- causal chains containing many non-identity-preserving consequences.

The criterion for success is the same as before:

> specify the causal relation before knowing which stages are supposed to count as the same self.

A candidate that survives this test would leave UCL with only the origin problem. A candidate that repeatedly requires “identity-relevant” selection by hand would show that the causal provenance survivor is local rather than general.

---

## 12. Status

**Junction rule:** provisional survivor as a mathematical partition rule.

**UCL:** provisional survivor, still open as a general theory.

**Diachronic identity reduction:** open.

No canonical status change is warranted.
