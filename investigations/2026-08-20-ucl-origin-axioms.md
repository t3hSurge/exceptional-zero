# Investigation: UCL — Candidate Axioms for the Admissible Origin Class

**Date:** 2026-08-20  
**Status:** Open / in progress  
**Related investigation:** `investigations/2026-08-20-diachron-identity-causal-provenance-survivor.md`

---

## 1. Question

Can Candidate F — **Unique Causal Lineage (UCL)** — be formulated from a principled class \(\mathcal O\) of admissible origin predicates, specified independently of diachronic identity, such that the resulting lineage relation is well-defined and non-arbitrary on causal graphs with branching, merging, duplication, reconstruction, and temporal gaps?

The investigation deliberately separates two questions:

1. **Origin admissibility:** when does a predicate \(O\) legitimately count as an independently specified origin predicate?
2. **Lineage partitioning:** given \(O\) and a causal graph, what rule turns origins and causal edges into disjoint persistence lineages?

A failure of the second does not by itself refute the first.

---

## 2. Candidate axiom family \(\mathcal O\)

The following are proposed as **candidate constraints**, not yet accepted axioms.

### O1 — Target Independence

\(O(x)\) must be definable without using diachronic identity, “same self,” “genuine past,” ownership, first-person privilege, actualness of the target history, or an equivalent target-bearing predicate.

This is the formal version of the anti-circularity requirement.

### O2 — Structural Invariance

If \(f:S\to S'\) is an isomorphism between the relevant causal structures, then:

\[
O(x)\iff O(f(x)).
\]

The origin predicate cannot depend on labels, names, or an observer's presentation of the graph.

### O3 — External/Pre-Identity Specification

The facts used to determine \(O\) must be available independently of the identity verdict the predicate is later used to determine. Examples may include a specified creation event type, a biological production event, or a defined causal-boundary condition.

This blocks a disguised Construction B such as “the event from which the genuine self originates.”

### O4 — Non-Retrospective Selection

\(O\) should not be selected by inspecting which later stages one already wants to count as the same entity. A candidate origin rule may refer to the causal structure in a fixed model, but it may not choose \(O\) by solving the identity problem first.

### O5 — Determinate Admissibility

For a given structure, the rule for whether an event is an origin must have a determinate result. If several events satisfy \(O\), that multiplicity must be represented explicitly rather than hidden by an unstated uniqueness assumption.

### O6 — Extension Stability

If the causal graph is extended by adding later events without changing the already specified past structure, an event that was an \(O\)-origin does not cease to be one merely because a later identity verdict becomes inconvenient.

This tests whether “origin” is genuinely historical rather than retrospectively selected.

---

## 3. What these axioms actually give

O1–O6 constrain the **origin predicate**, but they do not yet define identity.

In particular, they do not imply:

\[
\exists ! o\;O(o)
\]

for every candidate entity or history.

Nor do they imply that every temporal stage belongs to exactly one maximal non-branching path from an origin.

This separation is critical. UCL previously bundled “unique origin” and “non-branching lineage” together. The present pass shows that the two uniqueness claims are logically distinct.

---

## 4. Candidate lineage axioms

Even with an admissible \(O\), a further lineage rule is required.

### L1 — Causal Continuation

A stage belongs to a lineage only through the stipulated causal relation \(C\) from its predecessor stage.

### L2 — Non-Branching Continuation

A lineage follows at most one successor from each stage.

### L3 — Junction Termination

At a node where the relevant causal graph branches or merges, a lineage cannot pass through the junction while remaining one non-branching lineage.

This is what allowed the original UCL candidate to survive fission and fusion.

### L4 — Boundary Assignment

A rule is required for stages at or immediately after a junction. Options include:

- terminate the predecessor lineage and begin multiple successor lineages;
- terminate prior identity and create a new lineage at the junction;
- exclude junction stages from lineage membership;
- impose a principled parent-selection rule.

No option is currently preferred.

### L5 — Partition Requirement

If UCL is to constitute an identity relation over stages, every stage in the domain must belong to exactly one equivalence class:

\[
\forall x\;\exists! [x].
\]

Equivalently, the proposed identity relation must be reflexive, symmetric, and transitive and its equivalence classes must partition the stages.

This requirement exposes the central unresolved problem: L1–L3 alone do not guarantee L5 on arbitrary causal graphs.

---

## 5. Pressure test: branching

Consider:

\[
A\to B,\qquad A\to C.
\]

Under L2–L3, the predecessor lineage terminates at the branch and two successor lineages begin.

This is coherent and avoids declaring:

\[
A=B\quad\text{and}\quad A=C
\]

when \(B\neq C\).

But the result is a substantive axiom: identity terminates at branching unless a further rule is supplied.

No contradiction has been found. The cost is explicit and must not be hidden.

**Result:** branching is compatible with UCL, but only because UCL chooses identity termination at the junction.

---

## 6. Pressure test: merging / fusion

Consider:

\[
A\to C,\qquad B\to C.
\]

A non-branching path cannot contain both predecessor histories and still remain a single path.

If \(C\) belongs to both prior lineages, the proposed identity relation is not a partition.

If \(C\) belongs to exactly one, a parent-selection rule is required.

If \(C\) belongs to neither and begins a new lineage, identity terminates at the merge and a new lineage begins.

The third option is structurally clean, but it is an additional substantive rule, not a theorem of causal provenance alone.

**Result:** fusion exposes a genuine partitioning choice that UCL itself does not determine.

---

## 7. Pressure test: shared production event

One origin event may produce multiple later branches, as in cloning or twinning.

A shared origin does not by itself entail shared diachronic identity. Under non-branching lineage, identity may terminate at the first branch and split into distinct successor lineages.

This means:

\[
O(A)=O(B)
\]

does not imply:

\[
A\equiv_{UCL}B.
\]

That is a useful result: **common origin and diachronic identity must not be conflated.**

However, it also shows that “unique origin” is not sufficient to explain identity. The lineage rule does additional work.

---

## 8. Pressure test: overdetermined causation

Suppose a stage \(C\) has two independent causal parents \(A\) and \(B\), neither of which is a simple branch of the other.

A pure causal-path definition may admit multiple valid paths into \(C\). The graph therefore fails the uniqueness assumptions needed for a simple lineage partition.

Possible repairs are:

1. define a distinguished causal relation narrower than generic causation;
2. terminate prior lineages at overdetermined-causation points;
3. impose a parent-selection principle.

Option 1 is independently specifiable only if the narrower causal relation is itself justified without identity. Options 2 and 3 are substantive additions.

**Result:** ordinary causation is too broad for UCL without further structure.

---

## 9. Pressure test: reconstruction

A reconstruction from original parts can have strong material similarity to an earlier object while possessing a distinct causal history.

UCL selects the continuously descended vessel rather than the later reconstruction when the construction event and causal path are independently specified.

This remains a strength of the candidate.

But if the original lineage is itself dismantled and later resumed, the answer depends on whether the causal relation remains continuous through the dismantling interval. That is not determined by “causation” in the abstract; the relevant causal relation must be fixed independently.

**Result:** survived only with a specified causal relation, not generic causal language.

---

## 10. Pressure test: temporal discontinuity

A temporal gap does not itself break UCL. If a stipulated causal relation connects the pre-gap and post-gap stages and no junction rule terminates the lineage, continuity can persist.

This is consistent with the earlier memory-loss result.

The pressure point is the same as reconstruction: “causal continuity” must be defined independently enough to distinguish genuine continuation from merely related later events.

**Result:** survives in principle; depends on independent specification of the relevant causal relation.

---

## 11. Pressure test: isomorphism

O2 is necessary for UCL to remain a structural criterion rather than a naming convention.

If two causal models are isomorphic and the origin predicate is transported through the isomorphism, corresponding origins must correspond to corresponding lineage classes.

Therefore a mere redescription cannot change the identity verdict.

This does **not** imply that two causal histories in the same ambient structure must be interchangeable. External provenance can break the symmetry by being part of the structure itself. That is exactly why UCL survived the earlier internal counterfeit.

**Result:** O2 is compatible with the UCL survivor and clarifies what the “external asymmetry” claim means formally.

---

## 12. The main result of the axiom pass

The origin and lineage problems separate cleanly.

### Origin problem

The strongest current candidate admissibility conditions are:

\[
O1+O2+O3+O4+O5+O6.
\]

They successfully block the obvious circular constructions and preserve structural invariance, but they do not by themselves provide a universal origin predicate.

### Lineage problem

Even granting a good origin predicate, the following are still required to obtain an equivalence relation:

\[
L1+L2+L3+L4+L5.
\]

L4 is where arbitrary causal graphs force an additional selection or termination rule.

Therefore:

\[
\boxed{
\text{admissible origin}\not\Rightarrow\text{identity relation}
}
\]

and:

\[
\boxed{
\text{non-branching causal lineage}\not\Rightarrow\text{partition without a junction rule}
}
\]

These are the two current unresolved hinges.

---

## 13. Strongest surviving formulation of UCL

The most defensible current form is not:

> Identity is the relation of sharing a unique causal origin.

It is:

> **Candidate UCL:** A possible account of diachronic identity is obtained by combining an independently specified origin predicate with a specified causal relation and an independently specified rule for terminating or restarting identity at branching, merging, or other lineage junctions.

This is not yet a theory. It is a schema whose missing pieces are now explicit.

---

## 14. What would count as a genuine success

A successful UCL theory would require all of the following:

1. A principled class \(\mathcal O\) of origin predicates satisfying O1–O6 or a demonstrably better set.
2. A causal relation \(C\) independently specified and not tuned to identity outcomes.
3. A junction rule satisfying L4 without being chosen solely to recover pre-theoretical identity verdicts.
4. A proof that the resulting relation is an equivalence relation and therefore partitions the relevant stages.
5. Survival under the full adversarial battery.
6. A demonstration that the resulting criterion does not collapse into “the lineage whose later stages we already regard as the same self.”

Until then, UCL remains a provisional survivor rather than a reduction of identity.

---

## 15. Current status

**UCL:** provisional survivor.  
**Admissible-origin class \(\mathcal O\):** open.  
**Junction/partition rule:** open.  
**Diachronic identity reduction via UCL:** open.

The next phase should pressure-test candidate axiom sets against concrete graph families and ask whether the axioms are independently motivated or merely engineered to preserve desired identity verdicts.
