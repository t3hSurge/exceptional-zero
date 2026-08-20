# Investigation: Recurring Signature — Track 1 (Structural Derivation)

**Date:** 2026-08-20  
**Status of investigation:** Open / in progress  
**Related canonical claim:** Recurring Signature (Part Eight) remains **Open**

---

## 1. Question

Can the recurring failure of third-person relational accounts (underdetermination or circularity) across for-this, truth, and diachronic identity be derived from the Exceptional Zero / *Z(S)*, or from a controlled generalization of non-transitivity, without inserting the target by hand?

## 2. Current candidate formulation

**Candidate:** Any structure *S* whose relations are restricted to a non-identity, third-person vocabulary cannot isolate the target (genuine past / for-this / truth-maker) by automorphism-invariant means without either leaving it underdetermined among orbits or requiring a relation that already encodes the target. Therefore the pattern is a structural consequence of the demand for intrinsic asymmetry that the Cut formalizes.

This candidate is **not** yet claimed. It is the hypothesis under test.

## 3. What would count against it

- A derivation that succeeds only by smuggling the target into the signature of *S* or into the definition of the distinguishing relation.
- A counter-model: a structure rich enough for the relevant third-person relations in which an independently specified, automorphism-invariant property cleanly isolates the target.
- Reduction of the argument to the already-recorded Constructions A and B (identity) or to the dissolved Bradley regress (truth) without new force.
- Scope error: treating the target as an ordinary element of *S* when the target is higher-order.

## 4. Method constraints (from the framework)

- Independent specification of any candidate distinguishing relation *before* testing.
- Circularity check and target-shift check applied at every step.
- Language-dependence fork (§1.4) must be tracked: results may differ under broad vs. restricted readings of “property.”
- No status upgrade by resemblance alone.

## 5. First domain selected: Diachronic identity

Closest formal analogue to the Cut’s orbit argument. The document already records:

- Construction A: non-identity relations (temporal order, causal continuity, memory content, informational relations) leave genuine and counterfeit past in the same automorphism orbit.
- Construction B: adding an explicit “same-self” relation breaks the symmetry only by inserting the target.

**Task for this track:** Strengthen or generalize Construction A into a form that can be seen as forced by *Z(S)* itself, or show why no such strengthening exists.

### 5.1 Explicit counterfeit model

Let the genuine biography be a sequence of stages:

G = {g₀, g₁, g₂, …, gₙ}

with relations:
- gᵢ ≤ gⱼ for i ≤ j (temporal order)
- Causal links C(gᵢ, gᵢ₊₁)
- Memory/content relations M(gⱼ, gᵢ) holding when later stage gⱼ carries accurate content about gᵢ

Now construct a counterfeit rival F = {f₀, f₁, …, fₙ} that is relationally isomorphic:

- Identical temporal order and causal pattern.
- For every memory/content relation that holds in G, a matching relation holds in F (the implant copies both content and the apparent causal-history markers).
- No residual relational difference expressible in the allowed vocabulary.

Define the combined structure S = (G ∪ F, R), where R contains only the allowed third-person relations (temporal, causal, memory/content, finite similarity).

**Claim:** There exists an automorphism φ of S that swaps each gᵢ with the corresponding fᵢ (and fixes nothing relevant).  
**Reason:** By construction, every relation in R is preserved under the swap. Therefore Aut(S) acts transitively on the pair {gₖ, fₖ} for each k. No automorphism-invariant property can hold of the genuine stages and fail of the counterfeit stages.

This is now fully explicit. The underdetermination is forced once the vocabulary is restricted to relations that the implant can copy.

### 5.2 Attempted generalization to a corollary of Z(S)

Can the above be restated as: “If Aut(S) is transitive on the relevant pairs, then *Z(S)* fails for those pairs, and therefore no intrinsic particularity of the genuine past is available”?

Yes, but this is almost tautological. It says: when the structure is symmetric between genuine and counterfeit, there is no intrinsic particularity separating them. That is just the original theorem applied to this S. It does **not** show that every possible third-person vocabulary *must* produce such a symmetric S. It only shows that the vocabularies so far considered do.

To turn this into a structural consequence of the Cut itself, one would need a further claim: that any vocabulary capable of describing biographies *without already containing an identity or “genuine-past” primitive* will admit such an isomorphic counterfeit. That further claim has not been proved; it is a universal quantification over possible vocabularies and remains open.

### 5.3 Language-dependence check (§1.4 fork)

- **Restricted reading** (first-order or finitary properties): the counterfeit construction works. The genuine past is not expressibly particular.
- **Broad reading** (any automorphism-invariant property, including “belongs to the orbit of the actual causal origin”): the converse of the Cut holds, but only by treating orbit membership itself as a property. In the presence of the counterfeit, the genuine and counterfeit stages share orbits, so even the broad reading fails to separate them unless an additional primitive is added that breaks the symmetry first.

Thus the language-dependence fork does not rescue a non-circular recovery of the genuine past. Both readings leave the target underdetermined once a perfect relational copy exists.

### 5.4 Does an ambient Exceptional Zero help?

Suppose the larger world already contains many instances of *Z* (asymmetries elsewhere). Does that help isolate the genuine biographical chain?

No. An ambient Zero supplies asymmetry somewhere; it does not automatically privilege one of two relationally isomorphic chains inside the biographical substructure. To make the ambient Zero relevant to identity, one would have to add a relation that links the biographical stages to that Zero in a way that distinguishes genuine from counterfeit — which again inserts a distinguishing relation tuned to the target.

### 5.5 Result of this round

The explicit model confirms and sharpens Construction A. The underdetermination is forced for the tested class of vocabularies. However, the step from “these vocabularies fail” to “the failure is a structural consequence of the Exceptional Zero itself” still requires an unproved universal claim about all possible non-identity vocabularies. That claim has not been established. The candidate formulation therefore remains unproven.

**No status change.**

## 6. Next pressure steps for Track 1

1. Attempt to prove (or refute) the universal claim: any vocabulary that does not already contain an identity-like primitive admits a perfect relational counterfeit for biographies.
2. Explore whether modal or counterfactual relations (“would have produced different content if the implant had been absent”) can be added without smuggling. (Risk: the counterfactuals themselves may presuppose which history is actual.)
3. Parallel test on a different domain (truth or for-this) to see if the same orbit logic can be forced there.

## 7. Provisional status of the meta-claim

**Open.** The recurring signature is robust for the vocabularies examined; a derivation from the Cut as a general structural consequence has not been secured.

---

*This investigation does not alter the canonical framework. Results will be proposed for incorporation only after both tracks have reported and adversarial review is complete.*
