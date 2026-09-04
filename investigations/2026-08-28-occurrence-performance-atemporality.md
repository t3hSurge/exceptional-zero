# Occurrence, Performance, Supervenience, and Atemporality

**Date:** 2026-08-28  
**Status:** Open continuation of the orientation/transition investigation  
**Depends on:** `2026-08-28-orientation-transition-time.md`  
**Scope:** Whether actual occurrence/performance can be represented without temporal succession, and whether the distinction between atemporal structure and temporal actuality can itself be specified non-circularly  
**Not in scope:** movers, `C_*`, `G*_2`, `Σ`, identity ranking

---

## 1. Why this continuation was opened

The parent investigation established that orientation can be specified without time while orientation is not thereby transition. M1–M18 then showed that tested atemporal enrichments produce static structure or introduce an occurrence primitive rather than deriving actual transition.

The continuation separates several notions that had begun to run together:

\[
O_1=\text{actual/concrete existence of an event token}
\]

\[
O_2=\text{passage/becoming from }A\text{ to }B
\]

and later:

\[
P=\text{actual performance of an event}
\]

The investigation then asks whether performance depends on atemporal structure at all, and whether “atemporal” itself can be specified independently of the temporal content it excludes.

The guiding contrasts remain:

\[
\boxed{\text{possible history}\neq\text{actual happening}}
\]

\[
\boxed{\text{designation}\neq\text{occurrence}}
\]

\[
\boxed{\text{formal succession}\neq\text{temporal succession}}
\]

---

## 2. Atemporal actuality as concreteness — Candidate C

A third model was tested after designation and primitive occurrence:

\[
\mathcal M=(W,E,R,\mathrm{Conc})
\]

where `Conc` is a primitive monadic predicate on states and event tokens meaning concrete/actual rather than merely represented.

This gives a coherent atemporal model of `O_1` if concreteness is admitted as primitive:

\[
\boxed{\text{atemporal concreteness}\Rightarrow O_1}
\]

But a concrete event token carrying orientation does not thereby supply passage:

\[
\boxed{\text{atemporal concreteness}\not\Rightarrow O_2}
\]

The battery therefore split “occurrence” into actual existence of an event token and passage/becoming. The latter remains the unresolved target.

---

## 3. P9–P13 — Passage from concrete structure

Let the atemporal signature be:

\[
\sigma=(W,E,\mathrm{Conc},\prec).
\]

Candidate definitions of `Pass(A,B)` were tested using concrete event tokens, atemporal order, actuality contrast, minimality, and immediate-successor structure.

Every tested definition remained a static relation on the structure. No formula supplied the fact that `A` actually passes into `B`.

Earned bounded result:

\[
\boxed{O_1+\text{atemporal order}\not\Rightarrow O_2}
\]

No impossibility theorem was claimed. Route A remains open in the sense that a richer atemporal language has not been universally excluded.

A primitive `Pass` is coherent as an added semantic fact, but that is a primitive stipulation rather than a reduction. The distinction between formal succession and temporal succession therefore remains open.

---

## 4. P14–P19 — Primitive passage and formal succession

With primitive:

\[
\mathrm{Pass}\subseteq W\times W
\]

formal succession was defined as its finite transitive closure:

\[
S(A,C)\iff\exists n\ge1\;A=A_0,\ldots,A_n=C
\land\bigwedge_{i<n}\mathrm{Pass}(A_i,A_{i+1}).
\]

This is a genuine definitional construction:

\[
\boxed{\mathrm{Pass}\Rightarrow\text{formal succession}}
\]

provided suitable structural axioms such as irreflexivity/asymmetry are imposed when a strict partial order is wanted.

But:

\[
\boxed{\text{formal succession}\neq\text{temporal succession}}
\]

unless the interpretation of `Pass` already carries temporal content.

A primitive passage relation therefore yields a directed occurrence graph and formal order, not automatically time.

---

## 5. S-battery — truth-conditional semantics for actual passage

The next pressure tested whether ordinary truth-conditional semantics could distinguish actual passage from static representation without temporal content.

### S1. Truth-conditional extension

`Pass(A,B)` is true iff `(A,B)` belongs to the extension of the relation. This supplies an extension, not passage.

### S2. Actuality contrast

Requiring a non-concrete source and concrete target remains a static distribution of properties.

### S3. Selection-function semantics

An atemporal function `f(A)=B` gives deterministic dependence or selection. Interpreting it as “what becomes actual” imports the target.

### S4. Realization semantics

“Actualization” is either atemporal static dependence or temporal becoming. No third tested interpretation appeared.

### S5. Dynamic-update semantics

An abstract update operation can be represented without being executed. The execution gap therefore remains.

**S-battery result:**

\[
\boxed{\text{No tested truth-conditional atemporal semantics yields actual passage.}}
\]

The stronger meta-hypothesis that passage therefore requires non-static semantics remains unproven; genuinely dynamic semantics has not been exhaustively characterized.

---

## 6. N-battery — non-static semantics

The next pressure distinguished a model containing an evolution relation from a semantic framework whose own state changes.

Tested constructions:

- meta-level rewrite,
- designated actual semantic state,
- operational semantics,
- complete execution trace,
- primitive execution predicate,
- semantic operation as primitive act.

All either remained static representations, reduced to selection, or relocated the unexplained residue into primitive actual performance.

Earned result:

\[
\boxed{
\text{No tested non-static semantics distinguishes actual model evolution from represented evolution without a primitive of actual performance.}
}
\]

This does not prove that performance is primitive. It isolates the performance residue in the tested semantic constructions.

---

## 7. U-battery — actual unfolding

A further candidate primitive was:

\[
\mathrm{Unfold}\subseteq W\times W.
\]

Interpretations through bare relation, concreteness, actualization, primitive process, atemporal generation, and meta-level operation were tested.

Each either reduced to static structure or imported actual performance/temporal succession.

Earned:

\[
\boxed{\text{No tested atemporal semantics for actual unfolding has been produced.}}
\]

Not earned:

\[
\boxed{\text{actual unfolding is temporal succession}}
\]

The latter remains collapse pressure, not a theorem.

---

## 8. P-battery — actual performance predicate

Let:

\[
P(e)=\text{“event }e\text{ is actually performed.”}
\]

Tested interpretations included distinguished performance sets, concreteness, selected actual histories, actuality contrast, rule application, semantic update, primitive stipulation, and truthmaker semantics.

None supplied all four desired properties simultaneously:

1. atemporal,
2. non-static,
3. genuinely performance-bearing,
4. non-temporal.

Earned:

\[
\boxed{
\text{No tested atemporal interpretation of }P\text{ yields actual performance distinct from temporal succession.}
}
\]

A primitive `P` remains coherent only as an unreduced primitive or by importing the target into its interpretation.

The investigation explicitly avoids the universal claim that every possible atemporal semantics must fail.

---

## 9. D-battery — non-definability relative to a fixed signature

Fix the atemporal signature:

\[
\sigma=(W,E,\mathrm{Conc},\prec,H_*).
\]

Construct two interpretations with identical `\sigma`-structure but opposite values of `P(e^*)`.

Then:

\[
\mathcal A_1\equiv_\sigma\mathcal A_2
\quad\land\quad
P(\mathcal A_1)\neq P(\mathcal A_2).
\]

Therefore:

\[
\boxed{P\text{ is not definable from the tested }\sigma.}
\]

Equivalently, relative to this fixed signature, performance does not supervene on the tested structural theory.

The limitation is explicit: the construction puts `P` outside `\sigma`, so it does not establish non-definability from every richer atemporal vocabulary.

The pair therefore formalizes rather than closes the primitive-performance fork.

---

## 10. SUp-battery — supervenience and admissible atemporal enrichment

### Phase 1 — fixed atemporal languages

For any language restricted to the tested atemporal structural vocabulary, isomorphic structures agree on every sentence of that language. The stipulated performance difference therefore remains invisible.

\[
\boxed{P\text{ does not supervene on the tested atemporal language.}}
\]

### Phase 2 — richer atemporal enrichment

Several candidate admissibility rules were tested:

- syntactic ban on temporal words,
- definability from raw structure,
- permutation/isomorphism invariance,
- semantic-neutrality criteria.

The first three fail to control interpretation; the fourth has genuine bite but remains informal and recursive.

The resulting meta-problem is:

\[
\boxed{\text{The class of “admissible atemporal facts” has not been given a non-circular formal boundary.}}
\]

Therefore the strongest global supervenience claim remains open.

---

## 11. AT-battery — can “atemporal” itself be specified?

Candidate definitions were tested.

### AT1. Vocabulary absence

No temporal words does not guarantee atemporal semantics.

\[
\boxed{\text{vocabulary absence}\neq\text{semantic atemporality}}
\]

### AT2. Structural invariance

Fixed/static structure does not determine whether an interpretation is temporal.

\[
\boxed{\text{structural invariance}\neq\text{semantic atemporality}}
\]

### AT3. Model-theoretic definability

Isomorphism invariance characterizes formal definability, not the semantic kind “atemporal.”

\[
\boxed{\text{isomorphism invariance}\neq\text{atemporality}}
\]

### AT4. Identical static structure, differing interpretations

The same static structure can be paired with different external interpretations, one temporal and one not, showing that static structure alone does not fix semantic temporality.

### AT5. Positive semantic boundary

Attempts based on “no dynamics,” static truth conditions, absence of tense/indexicality, or fixed-model extensionality fail to yield a non-circular positive criterion.

**AT-battery result:**

\[
\boxed{
\text{No tested non-circular criterion for atemporality has been found.}
}
\]

This is a constructive failure across the tested families, not a theorem that no criterion exists.

---

## 12. Current locked results

\[
\boxed{\text{Atemporal concreteness can model actual existence of event tokens.}}
\]

\[
\boxed{O_1+\text{atemporal order}\not\Rightarrow O_2\quad\text{in every construction tested}.}
\]

\[
\boxed{\text{No tested truth-conditional or non-static semantic construction yields actual passage.}}
\]

\[
\boxed{\text{No tested atemporal predicate yields actual performance distinct from temporal succession.}}
\]

\[
\boxed{P\text{ is not definable or supervenient relative to the tested atemporal vocabulary.}}
\]

\[
\boxed{\text{The admissibility class of genuinely atemporal structure remains undefined.}}
\]

\[
\boxed{\text{The Cut still has no demonstrated dynamical consequence.}}
\]

---

## 13. What is not earned

The investigation does **not** establish:

- performance is primitive;
- passage is primitive;
- performance is identical to temporal succession;
- transition is irreducibly temporal;
- time is primitive;
- time is generated by the Cut;
- actual unfolding is temporal succession;
- the Cut causes occurrence;
- a universal non-supervenience theorem over every conceivable atemporal ontology.

---

## 14. Live frontier

The latest pressure moved the problem one level upstream of performance:

> **Can “atemporal” be specified without presupposing the temporal/performance content it is meant to exclude?**

Until that domain is independently bounded, a full supervenience theorem cannot be cleanly stated.

The current conceptual map is:

\[
\mathrm{Cut}
\to
\mathrm{distinction}
\to?
\mathrm{orientation}
\to?
\mathrm{concreteness}
\to?
\mathrm{passage}
\to?
\mathrm{formal\ succession}
\to?
\mathrm{temporal\ succession}
\to?
\mathrm{time}
\]

with the additional meta-condition:

\[
\boxed{\text{admissibility of “atemporal” remains open}}
\]

Identity investigations remain downstream and parked. No mover, `G*_2`, `L`, or `Σ` is introduced by this continuation.

---

## 15. Next pressure

Do not add another synonym for passage, performance, or unfolding.

The next legitimate work is either:

1. construct a genuinely non-circular criterion for atemporality and then rerun the supervenience question over that domain; or
2. attempt a bounded exhaustion argument showing why every semantic criterion strong enough to distinguish actual performance necessarily imports temporal/performance content.

Neither result is currently earned.
