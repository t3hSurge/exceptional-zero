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

## 2. The First Object of Investigation: Admissible Representation Change

Let a causal history be represented by a structure

\[
G=(V,E,\mathcal{R}),
\]

where `V` contains stages or events, `E` contains causal connections, and `\mathcal{R}` records independently specified structural features such as substrate continuity, process continuity, information flow, functional organization, or intervention relations.

A **representation change** is admissible when it changes the description without changing the causal history being described in the relevant structural sense.

That definition is deliberately provisional. The phrase **relevant structural sense** is exactly where identity could re-enter.

Three basic operations are distinguished:

1. **Refinement:** replace one coarse causal edge with a more detailed subgraph whose composition represents the same causal transition.
2. **Coarse-graining:** collapse a detailed causal subgraph into a single edge while preserving the relevant external input/output structure.
3. **Isomorphic redescription:** rename or structurally relabel nodes, edges, and predicates without changing the represented causal structure.

The investigation must not treat arbitrary additions or deletions of causal facts as mere representation changes. A refinement that introduces genuinely new causal structure is not automatically admissible.

The first question is therefore prior to any particular \(\Sigma\):

> **Can the equivalence relation \(G\sim H\) on representations be specified independently of which causal features \(\Sigma\) later treats as identity-relevant?**

If not, then \(\Sigma\) and representation admissibility are not genuinely separate layers. They form a single package whose invariance condition already contains the distinction the selection principle is supposed to discover.

---

## 3. Admissibility Constraints Before \(\Sigma\)

Hold \(\Sigma\) completely unspecified. Any admissibility relation \(\sim\) must be tested against these constraints before a candidate selection principle is privileged.

### AR-1 — Target Independence

\(G\sim H\) must be defined without reference to which stages are the same self, genuine, counterfeit, or otherwise identity-bearing.

### AR-2 — Structural Specification

The relation must be stated in terms of independently available structural facts about the represented causal systems, not by appeal to the persistence verdict that the representation is supposed to constrain.

### AR-3 — Isomorphism Compatibility

Pure relabeling or structurally equivalent redescription cannot alter admissibility.

### AR-4 — Refinement Independence

Splitting a causal transition into more detailed substeps must not change whether the descriptions represent the same history merely because the description became more detailed. A refinement that introduces genuinely new causal structure may, however, cease to be equivalent.

### AR-5 — Coarse-Graining Independence

Compressing a causal subgraph must not arbitrarily change representation-equivalence merely because descriptive resolution decreased. The permissible loss of information must be specified independently rather than by the identity verdict.

### AR-6 — No Hidden \(\Sigma\)

The definition of \(G\sim H\) cannot preserve precisely those causal features that a later \(\Sigma\) is supposed to select. Otherwise the selection problem has merely been moved upstream.

### AR-7 — Nontriviality of Representation Equivalence

The relation must permit genuinely equivalent descriptions while distinguishing descriptions that differ in causal structure. Declaring every pair equivalent makes invariance vacuous; declaring no pair equivalent makes invariance unusable.

These are constraints, not a supplied universal definition of admissibility.

---

## 4. Admissibility Battery

The battery now begins **before** any candidate \(\Sigma\) is introduced.

### Test A — Theseus: Process Versus Material Description

Represent the same replacement history once with explicit process-continuity edges and once with explicit material-provenance edges.

**Question:** Can the two descriptions be declared equivalent without deciding in advance whether process or material continuity is identity-relevant?

If equivalence requires choosing one, the admissibility relation already contains \(\Sigma\).

### Test B — Refinement of Theseus

Take a process-level representation and refine each replacement into individual operations, material transfers, and temporal stages.

**Question:** Can refinement preserve representation-equivalence without privileging process, matter, organization, or information?

A negative result would show that refinement invariance itself is carrying the missing selection principle.

### Test C — Coarse-Grained Theseus

Collapse the detailed replacement sequence into a smaller graph describing only the initial ship, replacement process, and final configurations.

**Question:** Can coarse-graining preserve equivalence without already deciding which features must survive the abstraction?

### Test D — Fission

Compare a fine-grained graph that explicitly displays the branch point with a coarse-grained graph in which the branch is represented as a single transition to two successors.

**Question:** Can both descriptions be equivalent without the equivalence rule itself deciding where identity terminates?

### Test E — Fusion

Perform the analogous comparison for a convergence point.

**Question:** Can refinement and coarse-graining preserve the same represented history without privileging one incoming causal line as identity-bearing?

### Test F — Counterfeit-Preserving Redescription

Take the perfect-counterfeit case and apply a redescription that preserves all structural facts available to \(\Sigma\).

**Question:** Can target and counterfeit remain equivalent in exactly the respects that matter, without the equivalence relation quietly excluding the counterfeit because it knows which history is genuine?

### Test G — Counterfeit-Separating Redescription

Now use a redescription that makes the external splice explicit without changing the underlying causal history.

**Question:** Is the distinction between genuine and counterfeit created by the representation, or merely exposed by it? An admissibility relation must not manufacture the distinction merely by choosing a privileged vocabulary.

### Test H — Redundant Causal Edges

Represent two independently sufficient causal mechanisms either as separate parallel edges or as one aggregated causal edge.

**Question:** Can these representations be equivalent without making a hidden judgment about which causal mechanism counts?

### Test I — Irrelevant Side-Effects

Refine a causal history by adding side-effects that are causally real but intuitively irrelevant to persistence.

**Question:** Can the refined and unrefined descriptions remain equivalent without \(\sim\) already knowing which causal features are irrelevant?

### Test J — Causal Counterfeit

Construct a counterfeit that matches the genuine continuation on every feature selected by a future \(\Sigma\) under one representation, while differing on a feature that another admissible representation makes salient.

**Question:** Can equivalence between the descriptions be fixed independently of the identity verdict, or does the representation relation have to know that one history is genuine in order to classify the descriptions as equivalent?

---

## 5. The Strong Failure Mode

The most important possible failure is not simply that one candidate \(\Sigma\) picks the wrong ship.

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

---

## 9. Test A Result — The Admissibility Trilemma

Test A is now closed at the stated level. It does **not** prove that an admissibility relation is impossible. It establishes that ordinary graph isomorphism alone cannot settle whether the process-based representation \(G_P\) and material-based representation \(G_M\) count as the same history when they privilege different causal relations.

Three constructions remain:

| Construction | Result | Problem |
|---|---|---|
| **A1. Strict structural equivalence** | \(G_P \not\sim G_M\) | The representation difference is already decisive; \(\Sigma\) never gets to choose between the causal vocabularies. |
| **A2. Maximal / common-history equivalence** | \(G_P \sim G_M\) | Requires an independently specified common structure \(G^*\) of which both are genuine projections. |
| **A3. Selective equivalence** | Depends on which features are preserved | The missing selection principle has been moved into \(\sim\). |

The earned result is therefore:

\[
\boxed{\text{Test A cannot determine }G_P\sim G_M\text{ without either strictness, a deeper common structure, or selective equivalence.}}
\]

The live architecture consequently becomes:

\[
G_P,G_M \;\longrightarrow\; [\sim] \;\longrightarrow\; G^* \;\longrightarrow\; \Sigma.
\]

No candidate \(G^*\) is promoted by Test A. The next object is whether an independently specified common structure can exist without becoming a dumping ground for every feature a later theory might call identity-relevant.

---

## 10. Test B — The Common-Structure Trilemma

Hold \(\Sigma\) completely unspecified. Let \(G^*\) be any proposed representation-independent common structure satisfying AR-1 through AR-7.

Ask whether its structural vocabulary is **selective, exhaustive, or insufficient**.

### B1. Selective \(G^*\)

\(G^*\) preserves some relations and excludes others. Selectivity is legitimate only if the exclusion rule has an independent structural source — for example mathematical type, causal direction, locality, conservation, or a formal graph constraint.

A selective proposal passes the surface form of AR-1 if its rule contains no identity vocabulary. But it must also pass the justification layer: adoption of the rule cannot be motivated by the persistence verdict it is intended to produce.

AR-6 imposes the additional constraint that the retained structure must not already perform the work of \(\Sigma\). If the rule excludes process continuity in favor of material continuity, or vice versa, and thereby uniquely determines the persistence partition, then \(G^*\) has hidden \(\Sigma\). If it excludes features without constraining the identity problem at all, the exclusion is identity-idle and does not explain why \(G^*\) was introduced.

### B2. Exhaustive \(G^*\)

\(G^*\) retains every independently describable relation. This is **not automatically circular**. An exhaustive structure could serve as a neutral substrate for a later \(\Sigma\).

The pressure is whether its membership condition has a principled, non-unrestricted boundary. If every conceivable predicate can simply be added, \(G^*\) becomes an unrestricted container rather than a substantive structural object.

Exhaustiveness therefore remains live pending a test of whether its membership condition can be independently bounded.

### B3. Insufficient \(G^*\)

\(G^*\) retains only enough information to make representations equivalent while destroying distinctions that a later \(\Sigma\) would need.

This branch is already eliminated as a viable solution: a common structure that cannot support the distinctions required by the subsequent selection step is insufficient by construction.

The corrected trilemma is therefore:

\[
\boxed{G^*\text{ must be selective, exhaustive, or insufficient.}}
\]

Only the insufficiency branch is presently defeated. Selective and exhaustive remain live.

### Success Criterion

A successful \(G^*\) would be an independently specified structure that is either:

- **selective**, under a non-identity-bearing structural rule; or
- **exhaustive**, under a principled, non-unrestricted membership condition;

and that still projects both \(G_P\) and \(G_M\) while preserving enough distinction for a later nontrivial \(\Sigma\).

### Boundary Criterion

A Boundary would be earned only if **every** admissible \(G^*\) satisfying AR-1–AR-7 either:

- requires identity-bearing selection in its construction;
- becomes unrestricted; or
- loses the distinctions needed by \(\Sigma\).

That would establish:

\[
\boxed{\text{No representation-independent common structure satisfying AR-1--AR-7 can support the proposed selection strategy.}}
\]

No such universal negative has yet been earned.

---

## 11. Selective \(G^*\): Pressure Test Against AR-1 and AR-6

The selective branch is now tested abstractly, without constructing a candidate \(G^*\) and without introducing \(\Sigma\).

### AR-1 — Target Independence

AR-1 has two layers here.

**Surface layer:** the exclusion rule contains no reference to sameness, genuine continuation, counterfeit status, identity-bearing features, or equivalent target vocabulary.

**Justification layer:** the choice to adopt the exclusion rule is itself not motivated by the identity verdict it happens to produce.

Many formally structural rules could pass the surface layer — mathematical type, causal direction, locality, temporal order, conservation, graph degree, connectedness, and similar constraints. But no candidate has yet been exhibited whose adoption is independently licensed and whose consequences survive the full battery without target-driven tuning.

**Provisional result:** AR-1 does **not** eliminate selective \(G^*\). It leaves the branch conditional on an independently licensed exclusion rule.

### AR-6 — No Hidden \(\Sigma\)

AR-6 is stronger than the vocabulary test. A rule can be stated without identity language and still functionally perform the selection that \(\Sigma\) was supposed to perform.

For the Theseus pair, a selective \(G^*\) has three broad possibilities:

1. **Retain both process and material structure.** Both remain available to a later \(\Sigma\). AR-6 is satisfied, but selectivity has largely retreated toward the exhaustive branch on the decisive features.
2. **Exclude one of process or material continuity.** If that exclusion uniquely determines the persistence partition under fixed `J_cut`, the excluded/retained choice is already \(\Sigma\). AR-6 fails.
3. **Retain some third family while excluding both.** AR-6 asks whether that third family itself determines persistence or leaves the competing readings available. If it determines the verdict, it is again hidden \(\Sigma\); if it has no bearing on the selection problem, its exclusion is identity-idle.

The earned diagnostic is therefore:

\[
\boxed{\text{selective exclusion either pre-settles identity or does not do the work }G^*\text{ was introduced to do.}}
\]

This is a **joint burden**, not yet a failure. AR-1 and AR-6 have not been shown jointly unsatisfiable.

### Current Selective-Branch Status

| Branch | AR-1 | AR-6 |
|---|---|---|
| **Selective \(G^*\)** | Open, conditional on independent structural licensing | Open, narrowed: exclusion must not pre-settle identity and must not be identity-idle |
| **Exhaustive \(G^*\)** | Not yet tested | Not yet tested |
| **Insufficient \(G^*\)** | Eliminated | Eliminated |

The next pressure on the selective branch, if continued, is the **joint satisfiability of AR-1 and AR-6**. No concrete selective rule should be manufactured before that abstract burden is tested.

---

## 12. Exact Current Status

| Item | Status |
|---|---|
| Test A | **Closed — conditional failure / \(G^*\) isolated** |
| \(G^*\) trilemma (Test B) | **Open — selective and exhaustive live; insufficient eliminated** |
| Selective \(G^*\) vs. AR-1 | **Open, conditional** |
| Selective \(G^*\) vs. AR-6 | **Open, narrowed by joint burden** |
| Exhaustive \(G^*\) | **Open, not yet tested** |
| \(G^*\) overall | **Open** |
| \(\Sigma\) | **Untouched** |
| UCL reduction | **Open** |

No candidate \(G^*\) has been promoted. No \(\Sigma\) has been introduced. No ranking has been made. No universal negative has been earned.

The next actual work is either to test whether AR-1 and AR-6 are jointly satisfiable for the selective branch, or, separately, to open the exhaustive branch. The investigation must not silently convert the present joint burden into a failure.
