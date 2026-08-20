# Investigation: Diachronic Identity — Fixed Counterfactual Causal Relation

**Date:** 2026-08-20  
**Status:** Open / candidate under pressure  
**Related investigations:**
- `investigations/2026-08-20-diachron-identity-causal-provenance-survivor.md`
- `investigations/2026-08-20-diachron-identity-ucl-junction-rules.md`

---

## 1. Question

Can a single, explicitly fixed counterfactual/intervention semantics supply the causal relation \(C_*\) required by UCL without importing diachronic identity through the choice of variables, interventions, or outcomes?

The test is deliberately narrower than “what is the right causal relation?” One intervention semantics is fixed first, then attacked without being modified in response to failures.

## 2. Fixed semantics

Use a structural causal model (SCM)

\[
M=(U,V,F)
\]

with exogenous variables \(U\), endogenous variables \(V\), and structural equations \(F\).

Admissible interventions are single-variable surgical interventions \(do(V_i=v')\) on variables in \(V\), with all exogenous variables \(U\) and all non-target structural equations held fixed.

For this round, the candidate causal relation is:

> A stage/event \(y\) is \(C_*\)-relevant to a later stage/event \(x\) iff there exists an admissible intervention on the endogenous variable representing \(y\) such that, with the background variables and all other structural equations fixed, the value of the endogenous variable representing \(x\) changes.

Formally, for variables \(Y,X\):

\[
Y\;C_*\;X
\quad\text{iff}\quad
\exists y'\neq y:\;M_{do(Y=y')}\models X\neq x.
\]

The intervention semantics, background variables, and structural equations are held fixed throughout the battery.

**Important limitation:** the semantics operates on a pre-specified variableization. The question is whether that variableization can remain independently specified rather than being chosen to encode the desired identity verdict.

## 3. Independence check

The SCM semantics itself is third-person and target-independent. It does not use “same self,” “genuine past,” ownership, or first-person privilege.

So the candidate clears the first anti-circularity gate.

That is not yet enough. The variable representing “the stage,” the outcome variable \(X\), and the admissible intervention target \(Y\) must also be fixed independently. Otherwise identity can re-enter through variable selection rather than through the definition of the causal relation itself.

## 4. Test 1 — Overdetermination

Suppose two independent predecessors \(A\) and \(B\) are sufficient for a later state \(C\): either one alone would have produced \(C\).

Under the fixed counterfactual criterion, intervening on \(A\) alone leaves \(C\) unchanged, and intervening on \(B\) alone leaves \(C\) unchanged.

Therefore neither gets \(C_*\)-credit under the strict necessity-based criterion.

This is a genuine result of the fixed semantics, not a patchable accident.

**Problem:** a causally continuous successor can have no qualifying predecessor at all under overdetermination. UCL would therefore cut the lineage even though causal structure remains continuous.

**Verdict:** fails persistence under overdetermination.

## 5. Test 2 — Preemption

Let \(A\) be the actual cause of \(C\), while \(B\) is a backup that would have produced \(C\) if \(A\) had not acted.

With the SCM containing the backup mechanism, intervention on \(A\) changes \(C\), so \(A\;C_*\;C\) can hold. The preempted backup \(B\) may fail the same test because its activation does not change the actual outcome under the fixed model.

This is a strength compared with naive ancestry: the semantics can distinguish actual from merely available causal routes.

**Verdict:** survives this case locally.

But the result is explicitly model-dependent: changing which backup variable is represented, or how the intervention is formalized, can change which causal route receives credit.

## 6. Test 3 — Repair

Suppose a system at \(A\) is damaged and later repaired to the same functional state \(B\).

Under the fixed SCM, the relevant question is whether interventions on the earlier-stage variable \(A\) change the later-state variable \(B\).

If the repair process overwrites the state and shields \(B\) from \(A\), then \(A\not C_* B\). The model therefore cuts persistence across repair.

If the repair is represented as a causal transformation preserving some state variable from \(A\), then \(A\;C_*\;B\) can hold.

The semantics itself does not determine which variableization is correct.

**Verdict:** underdetermined by variableization; no identity-specific answer follows from the intervention semantics alone.

## 7. Test 4 — Cloning

A stage \(A\) is used to construct clone \(B\). \(B\) may be structurally or informationally identical to \(A\), while its immediate causal production is mediated by a cloning process \(K\).

Under the SCM, intervention on \(A\) may change \(B\) if \(A\) is represented as an active parent of the cloning process. But an alternative equally legitimate variableization can make \(K\) the direct parent of \(B\) while treating \(A\) as background input to \(K\).

The resulting \(C_*\) relation differs without any change to the target identity question.

**Verdict:** exposes variable-granularity dependence.

## 8. Test 5 — Reconstruction

An object is dismantled and later reconstructed from preserved original parts.

If the reconstruction variable depends on the stored parts but not on the earlier assembled object-state variable, the earlier stage fails the \(C_*\) test.

If the earlier object-state is represented as a causal organizer of the storage/reconstruction process, the relation can be restored.

Again, both models can represent the same observable history while producing different \(C_*\) relations.

**Verdict:** variableization/model-structure dependence; no independent identity result.

## 9. Test 6 — Irrelevant side-effects

Suppose an earlier stage \(A\) causes many downstream effects, most irrelevant to the persistence of the candidate entity. A surgical intervention on \(A\) may alter one of those side-effects while leaving the candidate's later state unchanged.

The fixed semantics avoids counting such an effect only if the target outcome variable \(X\) is restricted in advance to the relevant state variables.

But that restriction is itself the problem:

> Which later variables count as the entity's persistence-relevant state without consulting the identity verdict?

If the outcome space contains everything downstream, causal relevance is too broad. If it contains only the variables judged to constitute the persistent entity, identity has entered through the outcome selection.

**Verdict:** no target-independent outcome restriction has yet been earned.

## 10. Test 7 — Causal counterfeit

Construct two processes \(P\) and \(R\) that are identical with respect to all variables and interventions admitted by the chosen SCM, but differ in some external history not represented in \(M\).

Then every admissible intervention gives the same result for \(P\) and \(R\):

\[
P\sim_{C_*}R.
\]

The counterfactual semantics therefore cannot distinguish them.

Adding the omitted provenance relation would distinguish them, but that simply enlarges the model and reopens the question of which relations are admissible.

This is the same domain-of-\(S\) problem already found with UCL.

**Verdict:** the fixed semantics does not escape the counterfeit problem; it relocates it to model specification.

## 11. What survives

The fixed SCM semantics establishes a clean conditional result:

> Once an SCM, variableization, intervention set, background variables, and outcome variable are fixed, the counterfactual dependence relation \(C_*\) is independently computable and can distinguish some causal routes, including certain preemption cases.

But the identity problem is not thereby solved. The choices that determine which stages are represented as variables, which interventions are admissible, and which outcomes count as persistence-relevant can change \(C_*\) without changing the underlying ordinary description of the case.

Thus the main obstruction is no longer “counterfactual causation is vague.” The semantics can be fixed. The obstruction is:

\[
\boxed{\text{identity-relevant variableization is not yet independently specified}.}
\]

## 12. Status

**Candidate \(C_*\): failed as a domain-general identity criterion in the fixed form tested.**

This does not show that no counterfactual causal theory could work. It shows that the particular fixed intervention semantics does not itself determine which variables and outcomes constitute the persistence-bearing entity. Overdetermination also directly breaks the strict necessity formulation.

The result therefore narrows the live space:

- the intervention semantics is mathematically well-defined;
- it is not sufficient to recover identity without additional variable-selection principles;
- adding those principles without target-smuggling is the next possible task, but should not be assumed necessary to be possible;
- UCL remains a provisional survivor only at the broader architecture level, not because this particular counterfactual \(C_*\) succeeded.

## 13. Next question

Do not immediately invent another causal criterion.

The exact remaining question is now:

> Can the relevant variables, admissible interventions, and persistence-bearing outcomes be selected by a target-independent structural rule, or is “the part of the causal model that counts for identity” itself another identity-shaped primitive?

Until that is answered, the counterfactual family remains exhausted for this fixed semantics.
