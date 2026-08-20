# Review: Diachronic Identity — Fixed Counterfactual C* Semantics

**Date:** 2026-08-20  
**Reviewed investigation:** `investigations/2026-08-20-diachron-identity-cstar-intervention-semantics.md`  
**Status of review:** Complete for the current round  
**Framework status affected:** None; this is a review record, not a canonical status change.

---

## 1. Executive finding

The fixed structural-causal-model semantics succeeds at doing something important: it turns “counterfactual causal relevance” into a precise, independently computable relation once the model is fully specified.

It does **not** recover a domain-general identity relation.

The decisive failure is not that counterfactual reasoning is vague. The semantics is explicit. The failure is that its result depends on prior choices about:

- which variables represent the stages,
- which variables are admissible intervention targets,
- which variables count as the persistence-relevant outcome,
- and which background variables are held fixed.

Overdetermination additionally defeats the strict necessity formulation directly: a successor can have multiple sufficient predecessors while none is counterfactually necessary.

The candidate therefore fails in the fixed form tested, while leaving a narrower meta-question open: can variableization and outcome selection themselves be fixed by an independent structural rule without importing identity?

---

## 2. The fixed semantics is genuinely fixed

The investigation correctly freezes one structural causal model:

\[
M=(U,V,F)
\]

with surgical single-variable interventions \(do(V_i=v')\), exogenous background \(U\) fixed, all non-target equations fixed, and causal relevance defined by an observed change in a specified later variable.

That is a real improvement over loose appeals to “what would have happened.”

The candidate is therefore entitled to a fair test. Its failures cannot be blamed on semantic vagueness.

---

## 3. Overdetermination is the cleanest direct failure

If two predecessors are independently sufficient for a later state,

\[
A\lor B\rightarrow C,
\]

then intervening on either predecessor alone can leave \(C\) unchanged.

Under the necessity-based \(C_*\), neither predecessor qualifies.

This matters because the failure arises **inside the fixed semantics itself**. No variableization dispute is needed.

So a necessity-only counterfactual relation cannot be the general causal backbone of persistence without an additional treatment of redundant causation.

Any repair to that treatment would have to be independently specified rather than chosen to recover preferred identity verdicts.

---

## 4. Preemption shows the semantics is useful but not sufficient

The fixed SCM can handle some preemption cases more successfully than naive ancestry. An actual causal route may change the outcome under intervention while a backup route does not.

That is a genuine success of the formalism.

But it should not be overcounted. It shows that the relation captures one interesting causal notion; it does not show that this notion is the persistence relation relevant to personal identity.

---

## 5. Repair, cloning, and reconstruction expose model-selection dependence

The same broad physical history can be represented with different endogenous variables.

In repair:

- the old state variable may remain causally upstream of the repaired state, or
- the repair process may overwrite the old state and make the later state depend only on the repair apparatus.

In cloning:

- the original may be represented as a direct parent of the clone, or
- the cloning operation may be the direct parent, with the original treated as an input to that operation.

In reconstruction the same issue appears again: causal dependence can be located in the surviving parts, the storage medium, the reconstruction process, or a higher-level organizer, depending on the structural variables selected.

These are not merely notational differences if the SCM's causal graph is supposed to be the ontology used to define \(C_*\). They can change the resulting identity-relevant relation.

So the candidate has relocated part of the original problem:

> What selects the right variables?

---

## 6. Irrelevant side effects expose the outcome-selection problem

The candidate also needs a distinguished later outcome variable \(X\).

But a causal predecessor can affect innumerable downstream variables that are irrelevant to the continued existence of the candidate entity.

If every downstream effect counts, \(C_*\) becomes far too broad.

If only certain downstream variables count, the theory needs an independent rule selecting those variables.

And if the rule says, in effect, “the variables constitutive of the same entity,” then the target has entered through the outcome definition.

This is the exact analogue of the origin-selection problem one level higher:

\[
\text{origin selection}\quad\leftrightarrow\quad\text{variable/outcome selection}.
\]

Both are potential locations where identity can be smuggled into an otherwise third-person causal theory.

---

## 7. The counterfeit test remains decisive

A causal counterfeit can match every relation represented in the fixed SCM while differing in some external history omitted from the model.

Then the two histories are counterfactually equivalent relative to that model:

\[
P\sim_{C_*}R.
\]

The only way to distinguish them is to enlarge the model to include the omitted relation.

That is not a defect in counterfactual reasoning; it is a reminder that the causal model has a domain-of-description problem.

The candidate therefore does not defeat the deeper counterfeit pressure. It demonstrates that **model specification is part of the causal criterion**.

---

## 8. What the candidate actually contributes

The fixed counterfactual semantics yields a useful conditional theorem-shaped result:

> Given a completely specified SCM, intervention regime, background, variableization, and outcome variable, counterfactual dependence defines a determinate causal relation.

That is worth keeping.

But it cannot yet supply the missing \(C_*\) for UCL because the framework still lacks an independently justified answer to:

\[
\boxed{\text{Which variables and outcomes are the persistence-bearing ones?}}
\]

That is now the live pressure point.

---

## 9. Status

**Fixed counterfactual C* candidate: failed in the tested form.**

The candidate is not rejected because counterfactuals are illegitimate or because causal models cannot be formalized. It fails because:

1. strict necessity breaks under overdetermination;
2. repairs, cloning, and reconstruction yield different causal relations under different target-independent-looking variableizations;
3. irrelevant side effects force an outcome-selection rule;
4. perfect counterfeits return whenever relevant external structure is omitted.

The surviving question is narrower:

> Can a target-independent structural rule choose the relevant variables, interventions, background, and outcomes so that the resulting causal relation is stable across these cases?

No such rule has yet been established.

---

## 10. Consequence for the UCL program

The three-layer architecture should remain:

\[
O\rightarrow C_*\rightarrow J_{\text{cut}}.
\]

But the present round does **not** advance \(C_*\) toward a successful candidate. Instead it clarifies what a successful \(C_*\) would have to accomplish.

The next pressure should therefore target **variableization and outcome selection**, not another synonym for causal relevance.

That keeps the investigation theorem-shaped and avoids candidate proliferation.
