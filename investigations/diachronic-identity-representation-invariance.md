# Diachronic Identity: Representation-Invariance Test

**Status:** Open investigation  
**Scope:** The selection principle between independently specified causal features in UCL  
**Depends on:** UCL architecture; `J_cut` held fixed; no new causal family introduced here

---

## 1. Starting Point

The current UCL architecture is:

\[
O \;\rightarrow\; [\text{selection of identity-relevant causal features}] \;\rightarrow\; C_* \;\rightarrow\; J_{\text{cut}}.
\]

The perfect-counterfeit / implanted-memory result is earned and robust. `J_cut` is a workable mathematical partition once a causal graph is fixed. What remains unresolved is the middle selection step.

Ship of Theseus is the decisive pressure point. Process continuity and material continuity can each be specified without identity language, yet they yield opposite positive persistence verdicts. UCL itself contains no rule selecting between them.

The next question is therefore not "which causal family should replace `C_*`?" It is:

> **Can a target-independent principle select identity-relevant causal features while remaining invariant under admissible changes in the representation of the same causal history?**

No answer is assumed.

---

## 2. What Counts as a Representation Change?

Let a causal history be represented by a structure

\[
G=(V,E,\mathcal{R}),
\]

where `V` contains stages or events, `E` contains causal connections, and `\mathcal{R}` records independently specified structural features such as substrate continuity, process continuity, information flow, functional organization, or intervention relations.

A **representation change** is admissible when it changes the description without changing the causal history being described in the relevant structural sense.

Three basic operations are distinguished:

1. **Refinement:** replace one coarse causal edge with a more detailed subgraph whose composition represents the same causal transition.
2. **Coarse-graining:** collapse a detailed causal subgraph into a single edge while preserving the relevant external input/output structure.
3. **Isomorphic redescription:** rename or structurally relabel nodes, edges, and predicates without changing the represented causal structure.

The investigation must not treat arbitrary additions or deletions of causal facts as mere representation changes. A refinement that introduces genuinely new causal structure is not automatically admissible.

The unresolved task is to specify the admissibility relation itself without using the desired identity verdict to define it.

---

## 3. Candidate Invariance Conditions

A proposed selection principle \(\Sigma\) for identity-relevant causal features should satisfy, at minimum, the following constraints.

### RI-1 — Target Independence

\(\Sigma\) must be stated without reference to:

- the entity that is "really" the same,
- the desired persistence verdict,
- the "genuine" past,
- psychological ownership,
- or any equivalent identity-bearing predicate.

If a representation is selected because it gives the pre-theoretically preferred identity answer, the selection has failed the anti-circularity test.

### RI-2 — Isomorphism Invariance

If two causal representations are isomorphic descriptions of the same structure, \(\Sigma\) must select corresponding causal features in the same way.

Pure relabeling cannot change what counts as identity-relevant.

### RI-3 — Refinement Stability

If a causal edge \(e\) is refined into a subgraph \(H\) without changing the represented causal transition, \(\Sigma\) must not reverse its identity-relevance merely because the description became more detailed.

A candidate may legitimately identify a feature newly exposed by refinement only if that feature represents genuinely new causal structure rather than descriptive granularity.

### RI-4 — Coarse-Graining Stability

If a detailed causal subgraph is compressed into a single edge while preserving the relevant structure, \(\Sigma\) must not manufacture or destroy identity relevance solely through compression.

RI-3 and RI-4 together prohibit a theory from locating identity in an artifact of descriptive resolution.

### RI-5 — Representation-Independent Verdict

If two admissible representations encode the same causal history, the induced persistence relation must agree across them.

Formally, for admissibly equivalent representations \(G\sim H\),

\[
\Sigma(G) \cong \Sigma(H)
\]

in the sense that corresponding stages receive the same identity-relevant classification.

### RI-6 — Nontriviality

\(\Sigma\) must select enough structure to distinguish at least the robust counterfeit case from its genuine continuation. A rule that declares every causal feature irrelevant is invariant but useless.

Conversely, a rule that treats every causal edge as identity-bearing is also unacceptable if it makes ordinary branching, convergence, and duplication collapse into indiscriminate persistence.

### RI-7 — Generality Without Target-Tuning

The same selection principle must be usable across the cases for which UCL is intended, without adding a new identity-motivated exception for each case.

A domain-specific restriction may be legitimate if independently justified. What is disallowed is a sequence of clauses whose only common function is reproducing desired identity judgments.

---

## 4. First Adversarial Battery

The battery is designed to attack the invariance conditions themselves rather than to propose another causal vocabulary.

### Test A — Ship of Theseus Under Refinement

Represent gradual plank replacement at two resolutions:

- coarse: one continuous process from the original ship-stage to the final ship-stage;
- fine: a sequence of individual replacement events, each with material and process relations separately represented.

**Question:** Can \(\Sigma\) select process continuity or material continuity without changing its verdict merely because the representation is refined?

A candidate that favors process at the coarse level but material at the fine level fails RI-3.

### Test B — Ship of Theseus Under Coarse-Graining

Start with the detailed replacement graph and collapse the replacement sequence into one transition.

**Question:** Does the selected identity-relevant feature survive compression?

If material continuity disappears merely because individual material transfers are no longer represented, the candidate may be representation-dependent rather than identity-relevant.

### Test C — Isomorphic Redescription

Rename stages, reverse arbitrary labels, and replace equivalent structural descriptions with isomorphic predicates.

**Question:** Does \(\Sigma\) remain unchanged?

This is the easiest condition and therefore the weakest test. Passing it is necessary but not informative by itself.

### Test D — Split Description of a Single Causal Mechanism

Represent one physical process either as:

\[
A\to B
\]

or as

\[
A\to X\to Y\to B.
\]

The intermediate stages carry no independent causal novelty; they merely expose the process's internal steps.

**Question:** Does the identity-relevance of the original transition survive the insertion of such intermediate nodes?

A candidate that changes verdict because the graph has more nodes fails refinement stability.

### Test E — Redundant Causal Description

Represent one causal transition with several independently sufficient descriptions of the same mechanism: physical, functional, and counterfactual descriptions that are known to co-refer structurally.

**Question:** Does \(\Sigma\) privilege whichever description happens to be chosen as the primary encoding?

If so, the selection principle is representation-relative.

### Test F — Counterfeit-Preserving Redescription

Take the perfect-counterfeit case and redescribe both genuine and counterfeit histories at progressively different levels:

- physical substrate,
- process history,
- functional organization,
- information flow.

The genuine continuation and counterfeit remain distinguishable in the full causal history, but different representations expose different features.

**Question:** Can \(\Sigma\) preserve the robust genuine/counterfeit distinction without arbitrarily privileging one vocabulary?

This test is crucial because RI-6 requires the selection principle to retain the one result UCL actually earned.

### Test G — Fission With Different Granularities

Represent a branching event as:

\[
A\to B,C
\]

or as a detailed process in which the branch emerges through a sequence of increasingly divergent intermediate states.

**Question:** Does `J_cut` still terminate the lineage at the same structural point once \(\Sigma\) is applied?

This tests whether the selection layer and the already-provisional junction rule remain compatible under representation changes.

### Test H — Merge With Different Granularities

Likewise represent

\[
B,C\to D
\]

at coarse and fine resolutions.

**Question:** Does the selected causal relation preserve the same termination at the convergence point?

A selection principle that makes fusion appear identity-preserving only at one resolution fails RI-4.

### Test I — Counterfactual Model Re-encoding

Where \(C_*\) is represented counterfactually, encode the same intervention structure using different but equivalent variable decompositions.

**Question:** Does \(\Sigma\) change which variables or outcomes count merely because the model has been factored differently?

This directly revisits the earlier failure of fixed counterfactual semantics, without introducing a new intervention semantics.

### Test J — Causal Counterfeit

Construct a counterfeit that matches the genuine continuation on every feature selected by \(\Sigma\) under one representation, while differing on a feature that another admissible representation makes salient.

**Question:** Does the candidate have a principled reason to reject the counterfeit that survives the representation change?

If the answer depends on which representation was chosen first, \(\Sigma\) has not supplied the missing selection principle.

---

## 5. The Strong Failure Mode

The most important possible failure is not simply that one candidate picks the wrong ship.

It is this:

> **A representation-invariant selection principle may be unable to exist unless the representation-equivalence relation already contains the identity-relevant distinction.**

If determining whether two descriptions are "the same causal history" requires deciding which causal features are identity-relevant, then the invariance test becomes circular one level earlier. The proposed cure would merely move the selection problem into the definition of admissible representation changes.

This is the key circularity test for the present investigation.

---

## 6. What Would Count as a Survivor?

A survivor need not solve diachronic identity outright. It must first establish a narrower result:

1. A target-independent selection principle \(\Sigma\) can be stated.
2. \(\Sigma\) is invariant under a clearly specified class of admissible representation changes.
3. The admissibility class itself does not encode the desired identity verdict.
4. \(\Sigma\) preserves the robust perfect-counterfeit result.
5. \(\Sigma\) interacts coherently with the fixed `J_cut` rule.
6. The principle handles both refinement and coarse-graining without case-by-case target tuning.

Only after these conditions are met would it make sense to ask whether the resulting \(C_*\) yields a genuine reduction of diachronic identity.

---

## 7. What Would Count as a Boundary?

A boundary would be earned if repeated, independently specified attempts show one of the following:

- every target-independent \(\Sigma\) is representation-sensitive;
- every representation-equivalence criterion capable of making \(\Sigma\) invariant already presupposes the identity distinction;
- invariance forces triviality (all causal features count or none count);
- or a principled selection survives some representations but necessarily fails under another admissible refinement/coarse-graining.

That would not prove that no conceivable selection principle exists. It would establish a defined boundary for reduction by representation-invariant causal selection, with the failed mechanism identified precisely.

---

## 8. Current Status

**Open.** No candidate selection principle has yet been tested.

The investigation begins here, not with a preferred answer. In particular, process continuity and material continuity are not being ranked in advance. The task is to determine whether anything above them can select between them without importing the identity verdict.

The Ship of Theseus remains the decisive case, but it is now being used as a test of the *selection architecture* rather than as an invitation to generate another causal family.
