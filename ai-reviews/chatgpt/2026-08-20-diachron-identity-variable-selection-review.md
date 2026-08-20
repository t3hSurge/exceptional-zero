# Adversarial Review: Diachronic Identity — Variable / Outcome Selection

**Date:** 2026-08-20  
**Reviewed investigation:** `investigations/2026-08-20-diachron-identity-variable-selection.md`  
**Status:** Complete for the current round  
**Canonical status affected:** None

---

## 1. Executive finding

The first variable/outcome-selection battery does not produce a survivor.

The tested selectors fail in different ways:

- all descendants overgenerate;
- path membership is representation-dependent;
- minimal sufficient sets need not be unique;
- causal/Markov boundaries are model-relative and occur at multiple scales;
- counterfactual indispensability fails under overdetermination and depends on the chosen outcome;
- organizational closure admits nested or competing scales;
- intervention invariance relocates the problem into the choice of admissible interventions.

The strongest result is not that variable selection is impossible. It is that the causal semantics does not, by itself, privilege a unique variable set.

---

## 2. The important new distinction

The investigation has separated two things that had previously been close together:

\[
\text{causal model boundary}
\neq
\text{ontological identity boundary}.
\]

A causal model must choose variables to represent a system. That choice can be refined or coarsened while preserving the underlying causal process.

Therefore, an identity selector based directly on variable membership inherits a new burden:

> It must be invariant under admissible changes of causal representation.

Without that condition, the proposed identity relation can change merely because the modeler replaced one variable with two equivalent subvariables or aggregated several variables into one.

---

## 3. Why the failed candidates matter differently

### All descendants

This is not a subtle failure. Causal consequence is vastly broader than identity-bearing persistence. Environmental effects and downstream actions prove the point immediately.

### Path membership

This identifies causal connectivity, but the property is sensitive to graph representation. Splitting an intermediary node can create or remove apparent path-membership facts without changing the underlying process.

### Minimal sufficient set

This is a serious candidate because it attempts to remove irrelevant causes. But causal systems with overdetermination can have several incomparable minimal sufficient sets. The selector therefore needs a tie-breaker.

### Markov boundary / causal blanket

This is the strongest purely statistical/structural candidate in the first family. Its failure is not that it lacks formal definition; it is that the same model can contain multiple legitimate boundaries at different scales. A boundary is not automatically the boundary of a persisting self.

### Counterfactual indispensability

The earlier fixed counterfactual semantics already showed the central problem: indispensability is a relation to a chosen outcome. Change the outcome variable and the “indispensable” cause can change.

### Organizational closure

Mutual causal support can identify robust organizations, but organizations can be nested. Nothing in closure alone says which scale is the subject of persistence.

### Intervention invariance

This remains potentially useful as a constraint. But invariance is only relative to a class of interventions. Selecting the class is itself a nontrivial modeling choice.

---

## 4. The adversarial general form

The original implanted-memory attack can be lifted into a general schema.

Given a proposed selector \(Q\), construct two causally modeled processes \(P\) and \(R\) such that:

1. they agree on every variable family admitted by \(Q\);
2. they differ only on a variable family excluded by \(Q\);
3. the intended identity verdict distinguishes them.

Then either:

- \(Q\) fails to distinguish a counterfeit, or
- \(Q\) must be expanded to include the excluded family.

This converts the variable-selection problem into a controlled search for a representation-level version of the earlier counterfeit construction.

That is the strongest methodological result of the round.

---

## 5. Current status

**Variable/outcome selection remains Open.**

The first candidate families have been exhausted for this round, but the higher-level question remains:

> Can a target-independent selector survive admissible refinement and coarse-graining of the causal representation while still generating the same identity partition under `J_cut`?

This should be tested before introducing further ad hoc selector candidates.

---

## 6. Recommended next test

Construct explicit paired causal models related by a defined refinement/coarse-graining transformation.

For each pair, hold the underlying causal process fixed while changing only the representation. Then test whether a candidate selector produces corresponding lineage segments under `J_cut`.

The first serious counterexample would be a case where:

\[
M_1\simeq M_2
\]

in the relevant causal sense, but

\[
Q(M_1)\neq Q(M_2)
\]

in a way that changes the resulting identity partition.

If such cases are unavoidable, the variable-selection problem becomes a representation-invariance boundary rather than merely another collection of candidate failures.
