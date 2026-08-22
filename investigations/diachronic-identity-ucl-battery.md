# Diachronic Identity: UCL Battery and Causal-Provenance Failure Boundary

## Status

This investigation revises the earlier blanket claim that Unique Causal Lineage (UCL) survives the current diachronic-identity battery.

**Earned:** UCL cleanly distinguishes the original implanted-memory / perfect-counterfeit case and gives structurally coherent null verdicts for genuine branching and convergence once the junction rule is completed.

**Not earned:** UCL as a domain-general reductive theory of diachronic identity. Ship of Theseus exposes an unresolved choice inside the causal relation itself.

The canonical framework should therefore not state that UCL "survives the current Ship-of-Theseus, duplication, fission, convergence, discontinuity, memory-loss, and perfect-counterfeit battery." That claim was too broad for the derivation actually shown.

## 1. Runnable apparatus

Let `G = (V,E)` be a causal graph whose nodes are states and whose directed edges represent direct causal production.

For purposes of this battery, an edge may be treated as **continuous** when the successor derives from ongoing modification of the same physical substrate as its predecessor, and **spliced** when the successor is produced through an external process such as copying, insertion, or reconstruction that does not conserve substrate. This is an explicit modeling choice, not something already fixed by the original UCL definition.

A continuous chain from `p` to `s` uses only continuous edges.

`J_cut` is taken to hold along a chain only when no node on that chain has continuous out-degree greater than one or continuous in-degree greater than one. Thus genuine branch and merge junctions terminate the relevant lineage segment.

`C_*(p,s)` holds when a continuous chain exists from `p` to `s`.

`O(p,s)` holds when `p` is the unique earliest node satisfying the relevant origin condition for `s`.

`UCL(p,s)` requires the origin condition, the selected causal relation, and the non-junction continuation condition jointly.

Two repairs were required to make the original prose definition runnable:

1. `J_cut` must constrain both out-degree and in-degree if convergence/fusion is to be handled symmetrically.
2. Redundant parallel causal mechanisms between the same node pair must not be counted as multiple successor nodes if overdetermination is to avoid a spurious branch verdict.

Neither repair was explicit in the earlier short definition.

## 2. Battery

### 2.1 Fission / duplication

**Remote reconstruction.** If the original persists while a second successor is reconstructed from new matter, UCL can exclude the reconstruction if reconstruction is classified as a splice. But that verdict depends on choosing a material-continuity interpretation of `C_*`. A process-continuity interpretation can classify the case differently. This variant therefore inherits the unresolved continuity-selection problem.

**Genuine bisection.** If one state continuously produces two successors through a real physical split, the predecessor has continuous out-degree two and `J_cut` fails. Neither successor inherits the predecessor under UCL. This is a clean structural null verdict, not an intuition-driven choice.

**Net:** split result. Bisection survives; remote reconstruction is continuity-reading dependent.

### 2.2 Ship of Theseus

Consider gradual in-place replacement producing Ship A while discarded original planks are later reassembled into Ship B.

Under **process continuity**, Ship A has an unbroken causal process and Ship B contains a splice. UCL favors A.

Under **material continuity**, Ship A eventually contains none of the original matter while Ship B is composed of the original planks. UCL can therefore favor B.

Both readings can be specified without using identity language. UCL itself does not select between them.

**Verdict:** genuine failure of domain-general determination at the `C_*` layer. This is the decisive unresolved case.

### 2.3 Reconstruction after destruction

A subject is destroyed and later reconstructed from a stored blueprint.

Material and ordinary process continuity classify the later subject as a splice. An informational-continuity reading could instead treat the blueprint as preserving the relevant continuation.

The existence of this additional plausible reading reinforces, rather than resolves, the underdetermination exposed by Ship of Theseus.

### 2.4 Perfect counterfeit / implanted memory

Let `P` be the ordinary continuation from `S_t1` and `R` a physically external process that implants information indistinguishable from the relevant memory/content of `P`.

Across the continuity readings tested here, `R` has no causal chain from `S_t1`; its provenance runs through the implantation device. `P` has the ordinary continuous provenance.

**Verdict:** UCL cleanly excludes the counterfeit and retains the genuine continuation. This is the case UCL was actually built to solve, and the result is robust across the tested readings of continuity.

### 2.5 Convergence / fusion

If two distinct predecessors continuously produce one successor, the successor has continuous in-degree two. Under the completed `J_cut`, the junction terminates both incoming lineage segments.

**Verdict:** neither predecessor is assigned the successor. The result is structurally coherent, but depends on the explicit in-degree completion of `J_cut`.

### 2.6 Branch then later merge

Any path crossing both a branch and a later merge contains junctions at both ends. Under `J_cut`, the path cannot remain one lineage segment across either junction.

**Verdict:** no UCL persistence relation spans the branch-and-merge sequence. This composes the branch and merge results rather than independently resolving a new metaphysical problem.

### 2.7 Overdetermined provenance

If two independently sufficient causal mechanisms produce the same successor from the same predecessor, the mechanisms are distinct causes but need not constitute distinct successor nodes. Treating parallel edges between the same node pair as a single successor relation avoids an artificial branch.

**Verdict:** UCL can remain intact after this explicit graph-modeling convention. The convention was not present in the original prose definition and should be recorded as part of the formal apparatus rather than silently assumed.

### 2.8 Cloning / shared origin

A clone produced from extracted genetic material develops through an independent process while the original continues. The original substrate does not continuously branch into the clone.

**Verdict:** UCL does not identify the clone with the original. This is a clean structural separation under the tested causal readings.

## 3. Synthesis

| Case | Result | Dependence |
|---|---|---|
| Perfect counterfeit | **Survives** | Robust across tested continuity readings |
| Cloning / shared origin | **Survives** | No additional patch beyond the stated provenance idea |
| Genuine bisection | **Survives as a null verdict** | Requires completed `J_cut` |
| Fusion / convergence | **Survives as a null verdict** | Requires completed `J_cut` |
| Branch → merge | **Survives as a null verdict** | Composes completed `J_cut` |
| Overdetermination | **Survives conditionally** | Requires explicit parallel-edge convention |
| Remote duplication | **Underdetermined** | Depends on continuity reading |
| Reconstruction after destruction | **Underdetermined** | Inherits continuity ambiguity; informational reading adds another option |
| Ship of Theseus | **Fails as a determinate criterion** | Process and material continuity give different verdicts |

## 4. Architectural consequence

The earlier architecture

`O → C_* → J_cut`

remains useful, but the battery shows that `C_*` is not yet a determinate identity-bearing relation. The live architecture is therefore better recorded as:

`O → [selection of the identity-relevant causal relation] → C_* → J_cut`

The unresolved question is not merely whether some causal relation can distinguish histories. It can. The question is whether there is an independently specified, target-independent principle that selects the causal features that count as identity-bearing across cases where plausible causal continuities diverge.

Ship of Theseus is the cleanest demonstration that this selection problem is real.

## 5. Consequence for the Recurring Signature

The broad exceptionless thesis that every non-target-bearing third-person account must collapse into underdetermination or circularity is **not** supported once UCL is considered. The perfect-counterfeit case is a genuine counterexample to that universal form.

But the earlier downgrade must not be strengthened into the opposite overclaim. UCL has not earned the status of a general third-person survivor across the full identity battery. Its success is narrower: it establishes that at least some external causal asymmetries can independently distinguish a genuine history from an informational counterfeit.

The appropriate live question is therefore narrower than the original universal claim:

> Can a principled class of independently specified causal/provenance relations be identified that survives the Ship-of-Theseus family without importing the identity verdict through the choice of what counts as continuity?

That question remains **Open**.

## 6. Methodological result

This pass also reinforces a standing rule of the framework: a status label cannot substitute for a shown derivation. Calling UCL a "provisional survivor" did not earn survival across seven named adversarial cases when the cases themselves had not been walked through.

The correct workflow is to expose the formal apparatus, record every modeling choice needed to make it runnable, run the battery, and then shrink the claim to the exact cases that actually survived.

This is an instance of the framework's own adversarial standard catching overreach in the framework's report of itself.
