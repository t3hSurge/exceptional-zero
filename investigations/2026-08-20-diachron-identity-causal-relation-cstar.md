# Investigation: Diachronic Identity — The C* Battery

**Date:** 2026-08-20  
**Status:** Open / in progress  
**Related investigations:**
- `investigations/2026-08-20-diachron-identity-causal-provenance-survivor.md`
- `investigations/2026-08-20-ucl-origin-axioms.md`
- junction/partition investigation for `J_cut`

## 1. Question

Given a fixed, independently specified origin predicate `O` and a fixed junction rule `J_cut`, can the UCL architecture supply an independently specified restriction `C*` on the full causal graph such that:

1. `C*` is defined without reference to personal identity, genuine past, ownership, or any equivalent target-bearing notion;
2. `C*` is non-trivial rather than counting every causal influence;
3. `O + C* + J_cut` yields a usable persistence relation;
4. the relation survives irrelevant side-effects, redundant causes, cloning, repair, reconstruction, fission, fusion, and perfect counterfeit tests;
5. the restriction is principled enough to generalize beyond one specially chosen domain.

This is a reduction test, not a presumption that such a `C*` exists.

## 2. Fixed components

The origin problem is held separate. The causal relation is the only variable in this pass.

`O`: an independently specified origin predicate, taken locally for the test domain. No identity-bearing interpretation of `O` is permitted.

`J_cut`: cut a lineage at every relevant branch or merge; a lineage is a maximal non-junction path under `C*`. The partition rule is held fixed rather than regenerated for each candidate.

The present question is therefore exactly:

\[
O \rightarrow C_* \rightarrow J_{cut}
\]

with `O` and `J_cut` fixed.

## 3. Why `C*` is necessary

The total causal graph is too large. A stage is causally connected to environmental events, incidental effects, other agents, background processes, component failures, language, social institutions, and countless downstream consequences.

If every causal edge counts, almost every stage participates in many branches and mergers, so `J_cut` would fragment the apparent lineage nearly everywhere.

Therefore UCL requires a restricted causal sub-relation `C*`.

The anti-circularity rule forbids defining `C*` as:

> the causal relation that preserves the same self.

The candidate must instead be specified by a causal criterion whose meaning is fixed before the identity verdict is known.

## 4. Candidate C1 — Biological/developmental causation

### Specification

Include causal edges participating in the organism's specified developmental process: reproduction, embryonic development, tissue differentiation, and the causally continuous maintenance of organism-level biological organization.

### Pressure

**Ship of Theseus / gradual replacement:** irrelevant or partially applicable. The criterion was designed for organisms, not artifacts. This is immediately a domain restriction rather than a general theory of diachronic identity.

**Cloning:** one organism can causally produce multiple organisms. `J_cut` handles the branch by terminating the predecessor lineage, but the criterion now says identity terminates at reproduction. That is coherent but domain-specific.

**Tissue replacement / repair:** some replacement operations remain inside the specified developmental/maintenance process, while others do not. A further rule is needed to say which causal processes count as constitutive maintenance rather than ordinary environmental influence.

**Chimerism / fusion:** two developmental histories can become one organism. The causal graph contains a merger, so `J_cut` terminates both predecessor lineages and starts a new one. Again coherent, but the biological criterion does not itself explain why the merged organism should be treated as a successor in the identity sense.

### Verdict

This is independently describable, but it is not domain-general. It supplies a biology-specific `C*`, not a general theory of identity.

**Status: survives locally; fails domain-generalization test.**

## 5. Candidate C2 — Material/component causation

### Specification

Count causal edges by which the material components of a later object descend from, or physically constitute, earlier components of that object.

### Pressure

**Ship of Theseus:** gradual material replacement eventually destroys material lineage, while ordinary causal continuity remains. The candidate therefore rejects identity after enough replacement unless an additional organizational rule is added.

**Reconstruction:** the original parts can be reassembled into a later object. Material provenance can make the reconstruction look strongly related to the original, potentially competing with the continuously repaired vessel. Nothing in material provenance alone chooses between them.

**Cloning:** identical material composition or duplicated source material does not provide uniqueness.

**Irrelevant side-effects:** material causal ancestry includes traces that are not constitutive of the object at all.

### Verdict

It is independently specified but too narrow and conflicts with persistence under gradual replacement without supplementary stipulation.

**Status: fails as a general `C*`.**

## 6. Candidate C3 — Environmental / relational embedding

### Specification

Count causal edges by which a stage remains causally embedded in the same externally specified environment: location, infrastructure, social setting, records, tools, and interactions.

### Pressure

**Irrelevant side-effects:** this relation is radically overinclusive. A self can causally affect a nearby wall, database, road, or stranger without those effects belonging to the self's persistence relation.

**Relocation:** moving an organism or artifact changes environmental embedding while apparently preserving whatever identity UCL is meant to track.

**Perfect counterfeit:** a sufficiently engineered counterfeit can be placed in the same environment and interact with it identically.

**Cloning:** two clones can share the same social and environmental setting.

To restrict the relation to “environmental causes relevant to maintaining the entity” reintroduces a constitutive relevance criterion that now needs its own specification.

### Verdict

Environment supplies genuine external causation but no principled reason for selecting identity-relevant edges from the total environmental causal graph.

**Status: fails as a general `C*`.**

## 7. Candidate C4 — Social / linguistic causal lineage

### Specification

Count causal edges through which later stages are produced by continuing social identity practices: naming, records, legal recognition, interpersonal recognition, language use, and other socially maintained continuities.

### Pressure

**Independence:** the relation is third-person and externally checkable in many cases.

**Coverage:** infants, isolated people, animals, artifacts outside human institutions, and pre-social development are not naturally covered.

**Counterfeit:** a socially recognized duplicate can receive the same name, records, and institutional treatment.

**Circularity risk:** restricting the relevant social relations to those that track “the same person” simply renames the identity criterion.

### Verdict

Real causal structure, but domain-limited and vulnerable to the same relevance-selection problem as environmental causation.

**Status: fails as a general `C*`.**

## 8. Candidate C5 — Actual-cause / counterfactual dependence

### Specification

Count a causal edge `a -> b` in `C*` when changing or intervening on `a`, under a formally specified intervention model, changes `b` while relevant background conditions are held fixed.

This candidate is attractive because it is not tied to biology, artifacts, or social practice. It defines causal relevance by counterfactual dependence rather than by the identity verdict the edge is supposed to produce.

### Pressure

**Redundant causation:** if two independent causes each suffice for `b`, neither is a simple but-for cause even though both may be part of the actual causal history.

**Overdetermination:** there may be several actual causal routes, none uniquely selected by simple counterfactual dependence.

**Background/intervention choice:** the result depends on which variables may be intervened on and which are held fixed. That intervention model is an independently specified structure, but different reasonable intervention choices can produce different `C*` relations.

**Side-effects:** a single event can counterfactually affect enormous numbers of downstream variables, reintroducing the fragmentation problem.

**Repair:** a replacement component may be counterfactually necessary for later functioning without being a descendant of the same material components. That may be useful, but it does not by itself distinguish identity from functional dependence.

**Cloning/fission:** a single predecessor can be counterfactually relevant to two successors. `J_cut` handles the branch, but the resulting “identity terminates at fission” conclusion is still a substantive UCL commitment.

**Perfect counterfeit:** if the counterfeit has genuinely different causal provenance, counterfactual structure can distinguish it. But if the counterfeit is embedded in a world engineered to reproduce the same intervention relations, the symmetry returns. The candidate therefore inherits the general `S`-domain issue already identified by Track 1.

### Verdict

This is the strongest candidate tested so far because it is domain-general and independently specifiable in principle. But it does **not yet** supply a unique `C*`: counterfactual relevance depends on an intervention/background model, and different independently reasonable choices can produce different causal subgraphs.

**Status: promising but unresolved.**

## 9. Candidate C6 — Constitutive/organizational causation

### Specification

Count causal edges that participate in maintaining the organization that makes the later stage the kind of entity it is: edges whose disruption would destroy the relevant organizational process.

### Pressure

This looks attractive for gradual replacement, repair, and biological maintenance. It also appears to distinguish constitutive processes from incidental side-effects.

But “the kind of entity it is” is ambiguous. If the relevant organization is specified independently—say, by a physical or functional model—the candidate may be legitimate. If the organizational boundary is chosen because it tracks the pre-theoretic individual, the criterion is circular.

**Repair:** some repairs become constitutive; others incidental. The model must specify the organization before knowing which answer to identity to produce.

**Cloning:** two copies can instantiate the same organization. Organization alone does not establish one lineage.

**Reconstruction:** a reconstructed artifact can instantiate the same organization as an earlier artifact without belonging to the same causal process.

**Fission:** one organization can branch into two successor organizations.

Thus constitutiveness may help identify important causal edges, but cannot itself determine lineage identity.

### Verdict

Potentially useful as a component of `C*`, but not sufficient on its own. Its legitimacy depends on an independently specified organizational model that has not yet been provided.

**Status: unresolved, with a defined circularity risk.**

## 10. Cross-candidate result

The candidate families divide into three groups.

### A. Domain-specific survivors

Biological/developmental and social/linguistic causation can be independently specified in bounded domains, but they do not generalize to a theory of arbitrary diachronic identity.

### B. Overbroad or too narrow relations

Material and environmental causation either omit intuitively important persistence cases or include huge numbers of irrelevant causes.

### C. Potentially domain-general candidates

Counterfactual causal relevance and constitutive/organizational causation remain genuinely interesting because they are not tied to one physical domain. Neither has yet produced a unique, non-arbitrary `C*`.

The current pressure therefore does **not** justify saying that causal provenance has failed. It has narrowed the surviving search to a more precise question:

> Can a domain-general causal relevance relation be specified independently of identity and uniquely enough that `O + C* + J_cut` yields a stable lineage partition?

## 11. A stronger formal constraint on `C*`

A legitimate `C*` must satisfy at least:

**C1 — Target independence.** The definition contains no identity, genuine-past, ownership, or equivalent target term.

**C2 — Isomorphism invariance.** Isomorphic causal structures produce isomorphic `C*` relations.

**C3 — Non-triviality.** `C*` is neither the full causal graph nor the empty graph merely by construction.

**C4 — Junction stability.** `C*` combined with `J_cut` yields maximal non-junction segments rather than a graph whose segmentation depends on the identity verdict.

**C5 — Redundancy tolerance.** Redundant or overdetermined causal routes cannot force arbitrary identity changes merely because one route becomes unnecessary.

**C6 — Side-effect rejection.** Ordinary downstream causal consequences do not automatically become part of the persistence relation.

**C7 — Counterfeit sensitivity.** If two stages differ in independently specified causal provenance, `C*` must be able to preserve that difference when it is relevant; otherwise UCL loses the very asymmetry that made it a survivor.

**C8 — Domain portability.** The definition should not contain organism-, artifact-, or person-specific assumptions unless the theory explicitly announces itself as domain-restricted.

These are constraints, not a completed definition of `C*`.

## 12. Result

No candidate `C*` has yet earned general survivor status.

The strongest current candidate is **counterfactual causal relevance**, because it has genuine domain-general potential and can be independently specified without identity language. Its unresolved problem is not obvious circularity but **model dependence**: the intervention/background structure used to define causal relevance may itself select different causal subgraphs.

Constitutive/organizational causation remains a second live candidate, but it has a sharper circularity risk around the individuation of the organization itself.

The biological, material, environmental, and social candidates do not currently provide a domain-general solution.

**Current status:** `C*` remains **Open**. UCL remains a **provisional survivor** rather than a completed reduction.

## 13. Next test

Hold `O` and `J_cut` fixed.

Do not generate another broad family of causal relations yet. Pressure-test the strongest domain-general candidate—counterfactual causal relevance—by fixing a formal intervention model and asking whether the resulting `C*` is invariant under reasonable alternative choices of background variables and interventions.

The critical cases are:

1. overdetermination;
2. preemption;
3. redundant repair;
4. cloning/fission;
5. reconstruction;
6. irrelevant downstream effects;
7. engineered perfect counterfeit with matched intervention structure.

If reasonable intervention models disagree about `C*`, then causal relevance has not earned the uniqueness needed by UCL. If they converge on a principled subgraph without consulting identity, that would be the first serious route toward a general `C*`.
