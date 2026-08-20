# Investigation: Diachronic Identity — Variable / Outcome Selection

**Date:** 2026-08-20  
**Status:** Open / first battery complete  
**Related investigations:**
- `investigations/2026-08-20-diachron-identity-causal-provenance-survivor.md`
- `investigations/2026-08-20-diachron-identity-causal-relation-cstar.md`
- `investigations/2026-08-20-diachron-identity-cstar-intervention-semantics.md`

---

## 1. Question

Given a fixed structural-causal semantics and a surviving partition rule `J_cut`, can a target-independent rule select the variables, intervention targets, background variables, and outcome variables whose counterfactual dependence is supposed to constitute the identity-relevant causal relation `C_*`?

The rule must be specified without reference to:

- same self;
- genuine past;
- mine/ownership;
- intended identity verdict;
- any equivalent target-bearing description.

The purpose is not to find the intuitively nicest variable set. It is to determine whether the causal model itself contains a principled way to select one.

---

## 2. Fixed causal semantics

Hold the previously tested intervention semantics fixed:

\[
M=(U,V,F),
\]

with a fixed structural-equation model, a fixed background assignment to the exogenous variables, and surgical interventions on specified endogenous variables.

For a specified source variable `X` and outcome variable `Y`, the candidate causal-relevance relation is counterfactual dependence under the fixed model:

\[
C_*(X,Y)
\quad\text{iff}\quad
Y_{do(X=x)}\neq Y_{do(X=x')}
\]

for at least one admissible pair of source values `x,x'`, holding the declared background fixed.

This semantics is not being changed in this investigation. The only question is which variables and outcomes are admitted into the relation.

---

## 3. Candidate selection rules

### Rule A — All causally downstream variables

Select every endogenous variable causally downstream of the candidate stage.

**Independence:** passes formally; no identity language is required.

**Pressure:** fails by overgeneration. A single stage typically has enormous numbers of downstream consequences: environmental effects, speech, artifacts, other people's states, heat, sound, and remote consequences. Under `J_cut`, these irrelevant effects create branches constantly and would terminate persistence almost everywhere.

The rule therefore gives a causal graph, not a useful individuation relation.

**Verdict:** fails by overgeneration.

### Rule B — Variables on every causal path to the stage's future state

Select the variables that lie on causal paths into the later state.

**Independence:** formally definable.

**Pressure:** fails by representation dependence. The same causal process can be represented with fine-grained variables, coarse-grained variables, or deterministic intermediary variables. A variable can appear path-essential in one representation and disappear entirely in another without any physical change.

So the rule selects features of the model's vocabulary rather than an invariant property of the causal process.

**Verdict:** fails by representational dependence.

### Rule C — Minimal causal basis / smallest sufficient variable set

Select a minimal set of variables sufficient to generate the later outcome under the structural model.

**Independence:** formally stated without identity.

**Pressure:** minimal sets need not be unique. Overdetermination gives multiple sufficient sets of equal status. Preemption can produce locally minimal sets that differ across model resolutions. Reconstruction can produce alternative minimal descriptions of the same later state.

Any tie-breaking rule must be independently specified or it becomes the missing selection principle in disguise.

**Verdict:** fails on non-uniqueness.

### Rule D — Maximal causal Markov blanket / boundary

Select variables constituting the smallest boundary that screens the candidate system from the rest of the model under the chosen conditional-independence semantics.

**Independence:** potentially strong; the rule is entirely structural/statistical.

**Pressure:** the Markov boundary can depend on the variableization and probability model. Multiple boundaries can exist. More importantly, a causal boundary is a model-relative boundary, not automatically an individuation boundary. A thermostat, a colony, a processor, or a human organism can each admit plausible causal blankets at different scales.

The rule therefore identifies a statistically useful subsystem but does not establish why that subsystem is the persisting entity.

**Verdict:** useful structural boundary, not identity criterion.

### Rule E — Counterfactual indispensability

Select variables whose removal or intervention would prevent the later stage from occurring under the fixed model.

**Independence:** formally definable.

**Pressure:** overdetermination immediately defeats uniqueness. If two causes independently suffice, neither is indispensable. If a later state has multiple realizations, the indispensability relation depends on which outcome variable is chosen. Repair and reconstruction can move indispensability from one variable set to another without changing the broader process.

**Verdict:** fails on overdetermination and outcome dependence.

### Rule F — Organizational closure / mutual counterfactual support

Select a set of variables whose members mutually sustain one another under the fixed causal model and whose future states depend on the set as a whole.

**Independence:** definable without personal-identity vocabulary.

**Pressure:** multiple scales can satisfy closure simultaneously. The same system can contain nested organizations. Nothing in closure alone privileges the organism over an organ, the person over the nervous subsystem, or an artifact over a component assembly.

Selecting the “right” organizational scale therefore reproduces the original problem at a different level.

**Verdict:** too plural and scale-dependent to ground identity without an extra selection principle.

### Rule G — Intervention-invariance / stable causal role

Select variables whose causal role remains invariant under an admissible class of interventions and model refinements.

**Independence:** formally attractive.

**Pressure:** the admissible intervention class becomes the decisive choice. Under one intervention family a variable may be stable; under another it may not. Model refinement can split one stable role into several variables or aggregate several roles into one. The rule therefore relocates rather than removes the selection problem.

**Verdict:** live as a methodological constraint, but not yet an identity selector.

---

## 4. Full pressure battery

### Overdetermination

Rules based on indispensability or minimal sufficiency fail because several independent causes can support the same outcome. `C_*` can remain well-defined while identity-relevant selection does not.

### Preemption

Causal ancestry and counterfactual dependence can disagree depending on the structural model. A preempted backup can have ancestry without being counterfactually necessary for the observed outcome.

### Repair

A repair can replace the variables through which a system previously maintained a causal role. A material criterion can declare identity lost; an organizational criterion can preserve it; an intervention-based criterion depends on which variables are treated as the outcome.

### Cloning

A clone can reproduce the same internal organization while having a different production history. Any rule based on internal variables alone fails the provenance distinction; any rule based on production variables needs an independently specified boundary for which production relations matter.

### Reconstruction

Reassembly from the original parts can preserve material variables while breaking the original causal organization, or preserve a causal role while changing material composition. No tested selection rule derives a unique verdict without choosing which variable family matters.

### Irrelevant side effects

The all-descendants rule is immediately defeated: causal descendants are not thereby identity-bearing. A person's footprint, sound, effect on another person, or environmental disturbance is caused by the person without being part of the persisting self.

Any rule that excludes these effects needs a principled boundary, and the tested structural rules do not provide one uniquely.

### Causal counterfeit

Construct a rival process matching every variable included by the selection rule but differing in an excluded variable family. If the rival counts as distinct under the intended identity verdict, the selection rule was too narrow. If it is included as the same identity, the rule risks overgeneration. This is the general adversarial form of the original P/R test.

---

## 5. What the battery establishes

The tested rules do not all fail for the same reason, but they expose a common boundary:

\[
\boxed{\text{The causal model determines causal structure more readily than it determines the privileged variable set.}}
\]

The model can tell us:

- what depends on what;
- what changes under intervention;
- which variables are upstream or downstream;
- which paths are blocked or active;
- which variables form a statistical/causal boundary.

It does not, by those facts alone, tell us:

> **which collection of variables is the entity whose persistence we are trying to define.**

This is not yet a proof that no such rule can exist. It is a first bounded failure of the major target-independent selection families tested here.

---

## 6. Important distinction: model boundary versus ontological boundary

A causal model requires variables. A variableization is already a choice of representation.

If two causally equivalent descriptions use different variable sets, then a selector based on variable membership can be representation-sensitive even when the underlying causal process is not.

Therefore any successful identity-selection rule must satisfy an additional invariance requirement:

> **Model refinement or coarse-graining must not change the identity relation merely by changing the vocabulary used to describe the same causal process.**

That requirement is stronger than ordinary causal sufficiency and has not been established for any candidate tested so far.

---

## 7. Current status

**Variable/outcome selection remains Open.**

No candidate tested in this first battery has supplied a target-independent rule that uniquely selects the identity-bearing variables across overdetermination, preemption, repair, cloning, reconstruction, side-effects, and causal-counterfeit cases.

The strongest live possibility is not a particular variable family but a higher-level invariance requirement: a successful selector would need to survive admissible changes of causal representation while still yielding a stable partition under `J_cut`.

That is a new theorem-shaped question, not another candidate family.

---

## 8. Next required test

Do not generate another list of variable-selection intuitions yet.

Instead formalize the representation-invariance requirement:

> Given two causally equivalent structural models related by an explicitly defined refinement/coarse-graining transformation, does a candidate selector choose corresponding identity-bearing variables and induce the same UCL partition?

If no target-independent selector survives this representation-invariance test, the failure will be stronger than any single candidate failure: it will show that the variable-selection problem is not merely difficult but unstable under changes of description.

If one selector does survive, it becomes the next serious candidate for `C_*`.
