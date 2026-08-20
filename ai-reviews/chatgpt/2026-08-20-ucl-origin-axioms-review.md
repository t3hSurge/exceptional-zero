# Review: UCL — Candidate Axioms for the Admissible Origin Class

**Date:** 2026-08-20  
**Reviewed investigation:** `investigations/2026-08-20-ucl-origin-axioms.md`  
**Status:** Complete for the current round  
**Canonical framework status affected:** None

---

## 1. Main result

The axiom pass correctly separates two problems that had previously been bundled together:

1. **Origin admissibility:** what makes an origin predicate independently specified rather than identity in disguise?
2. **Lineage partitioning:** given admissible origins and a causal graph, what rule produces disjoint persistence lineages?

This separation is itself a substantive methodological improvement.

The current candidate origin constraints O1–O6 are useful as admissibility tests, but they do not generate a domain-general origin predicate. Likewise, L1–L3 constrain a non-branching lineage but do not by themselves produce a partition on arbitrary causal graphs. L4 — what happens at branch/merge junctions — is the remaining explicit selection point.

---

## 2. Origin axioms: pressure assessment

### O1 — Target Independence

This is necessary and strong. It directly blocks Construction B. It is also the easiest axiom to state and the hardest to make completely formal: “does not use identity” is a semantic restriction on a language or definition, not yet a mathematical object.

**Assessment:** keep as a methodological axiom; formalization remains open.

### O2 — Structural Invariance

This is clean and mathematically natural:

\[
O(x)\iff O(f(x))
\]

under isomorphism. It prevents labels and presentation choices from carrying identity.

**Assessment:** strong candidate axiom.

### O3 — External/Pre-Identity Specification

Useful, but partly overlaps O1. Its value is practical: it forces the investigator to identify what fact makes the event an origin before using it to determine identity.

**Assessment:** keep, but eventually test whether it is genuinely independent of O1.

### O4 — Non-Retrospective Selection

This catches a subtler form of circularity: a rule can be formally free of the word “identity” while still being selected only after looking at the desired identity verdicts.

**Assessment:** important methodological constraint, but not yet formal enough to be an axiom in a mathematical theorem.

### O5 — Determinate Admissibility

Correctly prevents hidden multiplicity. But determinacy alone is weak: a rule can determinately select the wrong thing.

**Assessment:** useful bookkeeping requirement, not an identity-generating principle.

### O6 — Extension Stability

This is valuable because it blocks retrospective origin selection. However, whether it is required depends on how the underlying structure is modeled: if origins are properties of complete structures rather than growing histories, “extension” itself needs formal treatment.

**Assessment:** promising, but technically downstream of the modeling choice.

---

## 3. The main formal discovery: partition failure at junctions

The strongest result of this pass is not an axiom about origin at all.

It is this:

> A non-branching-path rule does not automatically define an equivalence relation on arbitrary causal graphs.

For a branch:

\[
A\to B,\quad A\to C,
\]

the non-branching rule can terminate identity at the junction. That is coherent, though substantive.

For a merge:

\[
A\to C,\quad B\to C,
\]

the later stage \(C\) cannot remain in both predecessor lineages if the relation is to be an equivalence relation. One must therefore either:

- terminate both prior lineages and start a new one at \(C\),
- select one parent lineage,
- or leave \(C\) outside the lineage partition.

The original UCL candidate had treated non-branching as if it solved this automatically. It does not.

**This is a genuine newly isolated gap.**

---

## 4. A warning about “unique origin”

The phrase “unique origin” contains two logically distinct ideas:

\[
\text{there is a unique event satisfying }O
\]

and:

\[
\text{there is a unique lineage relation extending from that event}.
\]

The former does not imply the latter.

A single origin can produce two branches. Multiple origins can converge. A process can have overdetermined causal parents. Therefore UCL cannot treat uniqueness of origin as sufficient for identity without an additional graph rule.

This is especially important for twins/clones:

\[
O(A)=O(B)
\]

does not imply:

\[
A\equiv B.
\]

The non-branching clause is doing real work there.

---

## 5. Generalization result

The current axiom set supports a useful negative result:

\[
\boxed{\text{admissible origin} \not\Rightarrow \text{identity relation}}
\]

and:

\[
\boxed{\text{non-branching causal lineage} \not\Rightarrow \text{partition without a junction rule}.}
\]

This does not weaken the original UCL survivor. It clarifies exactly what it survived and exactly what remains missing.

The survivor's causal asymmetry remains genuine: unlike purely internal memory/information relations, external provenance can distinguish an internally perfect counterfeit. But the existence of that asymmetry does not yet specify how all persistence cases are to be partitioned into identities.

---

## 6. Recommended next pressure test

Do not generate another origin predicate yet.

The next test should hold \(O\) fixed and attack **junction rules** first, because that is now the more sharply isolated structural gap.

Test at minimum:

1. pure branching;
2. pure merging;
3. branch followed by merge;
4. overdetermined causation;
5. shared origin with independent later divergence;
6. reconstruction after total causal interruption.

For each proposed junction rule, ask three questions:

1. Is it independently specified?
2. Does it produce a genuine equivalence relation?
3. Is its choice motivated by the structure itself, or merely by the identity verdict it is intended to reproduce?

Only after the junction problem is solved should the full origin class \(\mathcal O\) be considered mature enough for a general UCL theorem.

---

## 7. Status

**UCL:** provisional survivor.  
**Origin admissibility class:** open.  
**Junction/partition rule:** newly isolated open problem.  
**Reduction of diachronic identity:** open.

No canonical status upgrade is warranted.
