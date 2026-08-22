# Diachronic Identity: Candidate `G*_1` — Typed Physical Causal History

**Status:** Candidate tested; concrete construction fails the independent membership-boundary / representation-equivalence conjunction in its present form  
**Scope:** Attack the first concrete selective common structure proposed after the abstract AR-1 / AR-6 usefulness test  
**Depends on:** `diachronic-identity-representation-invariance.md`; `2026-08-21-gstar-selective-usefulness-test.md`; fixed `J_cut`; no `Σ` introduced

---

## 1. Candidate under attack

The first concrete selective candidate was:

\[
G^*_{\mathrm{phys}}=(V,E,\tau)
\]

where:

- `V` contains physically instantiated events or states;
- `E` contains directed physical causal relations among members of `V`;
- `\tau` types those relations, including at minimum process continuity and material provenance, without privileging either as the identity-bearing relation.

The candidate excludes semantic annotations, observer-relative labels, target-bearing predicates, and non-physical descriptive layers that are not themselves physical causal relations.

Its intended projection property is:

\[
G_P \leftarrow G^*_{\mathrm{phys}} \rightarrow G_M,
\]

so that both process-continuity and material-provenance descriptions remain recoverable without either becoming fundamental.

The candidate was deliberately constructed only to be attacked. No survival was assumed.

---

## 2. What the candidate initially earned

The first attack pass established several genuine positive results.

### 2.1 Theseus neutrality

`G*_phys` retains both process continuity and material provenance. It therefore does not decide the Ship-of-Theseus question merely by construction.

### 2.2 Perfect-counterfeit preservation

The physical provenance difference between a genuine continuation and an externally implanted informational counterfeit remains representable. The candidate therefore preserves the robust distinction that motivated UCL in the first place.

### 2.3 Junction neutrality

Fission and fusion remain structural branch/merge phenomena rather than being assigned an identity-bearing predecessor or successor. `J_cut` can remain the separate partition rule.

### 2.4 Resistance to hidden `Σ`

The candidate does not, on its face, collapse into the later identity-selection principle. Retaining both causal families is precisely what prevents it from silently choosing process over matter or matter over process.

These results remain earned. The present test does not revoke them.

---

## 3. The decisive remaining conjunction

The candidate must satisfy all three of the following:

\[
\boxed{
\text{independently bounded membership}
\;\land\;
\text{representation invariance}
\;\land\;
\text{refinement/coarse-graining stability}
}
\]

The central question is whether the phrase **physical causal relation** supplies a sufficiently precise boundary to make those properties hold simultaneously.

The answer for the candidate as currently specified is **no**.

This is a failure of the concrete candidate, not a universal negative about selective `G*`.

---

## 4. Pressure point A — What exactly belongs to `E`?

The candidate says that `E` contains directed physical causal relations. That sounds target-independent, but it leaves the membership rule incomplete.

Consider a physical system described at several legitimate levels:

\[
G_{\mu},\qquad G_{\mathrm{meso}},\qquad G_{\mathrm{macro}}.
\]

`G_μ` may represent microscopic interactions; `G_meso` may represent stable assemblies or processes; `G_macro` may represent organism-level or system-level causal organization.

All three can describe physically instantiated structure. Nothing in the candidate's definition specifies which level supplies the members of `V`, which causal dependencies count as edges of `E`, or which descriptions are merely coarse projections of the others.

The problem is not that multiple levels exist. The problem is that the candidate has no independently stated membership rule deciding how they relate inside one common structure.

There are three obvious repairs, and each changes the candidate's status:

1. **Choose a privileged physical level.** This supplies a boundary, but the candidate now depends on an independently defended choice of physical ontology/factorization that has not been supplied.
2. **Include every physically instantiated causal level.** This makes the structure effectively exhaustive with respect to physical causal descriptions, abandoning the intended selective boundary.
3. **Define a quotient or equivalence over levels.** This requires an independently specified representation-equivalence rule, which is precisely the missing object under the representation-invariance investigation.

None of these is available for free.

Therefore the phrase "physical causal relation" does not yet constitute a complete selective membership rule.

**Result:**

\[
\boxed{\text{independent formal boundary: fails as specified}}
\]

---

## 5. Pressure point B — Directness is representation-sensitive

A natural attempt to sharpen `E` is to retain only **direct** physical causal relations.

That does not solve the problem.

Suppose one description contains:

\[
A\rightarrow B.
\]

A refinement exposes:

\[
A\rightarrow x_1\rightarrow x_2\rightarrow B.
\]

If `A→B` was a direct relation in the coarse graph, it is no longer a direct edge in the refined graph. Conversely, if the coarse edge is treated as the composite representation of the refined path, then directness is not a representation-invariant property of the underlying history.

The same problem occurs with material provenance: a coarse material-ancestry edge can conceal the intermediate transfers, transformations, or storage events that become explicit under refinement.

Thus a definition of `E` based on graph-theoretic directness cannot independently stabilize the candidate under refinement.

**Result:**

\[
\boxed{\text{direct-edge sharpening fails representation invariance}}
\]

This is not a failure of causal graphs generally. It is a failure of this proposed membership rule to identify which graph edges are fundamental to `G*_phys` independently of representation resolution.

---

## 6. Pressure point C — All physical causal dependence is too broad

The opposite repair is to define `E` as every physical causal dependence.

That avoids the directness problem, but it destroys the selective boundary.

Once every physically instantiated causal dependency is admitted, the candidate retains:

- microphysical dependence;
- macroscopic process dependence;
- material ancestry;
- functional organization;
- information-bearing physical states;
- side-effects;
- redundant causal pathways;
- and other physically realized dependencies.

This may be a legitimate **exhaustive** common structure. It is not the proposed selective `G*_phys` anymore.

The Test B trilemma explicitly leaves exhaustive `G*` open. That branch must be tested separately rather than quietly importing it into the selective candidate.

Therefore:

\[
\boxed{\text{exhaustive physical causation does not rescue }G^*_1\text{ as a selective candidate}}
\]

It also does not refute the exhaustive branch.

---

## 7. Pressure point D — Refinement

Take a coarse physical history:

\[
A\xrightarrow{\mathrm{process}}B.
\]

Refine it into a detailed physical history containing both process steps and material transfers.

A valid representation-invariant `G*` must treat the refinement as a redescription when the additional nodes merely expose structure already implicit in the original transition.

But `G*_phys` has no rule determining whether the newly exposed nodes and edges are:

- genuinely new physical causal structure;
- merely finer representation of existing structure;
- or a change of causal vocabulary.

Any answer requires an independent criterion for what counts as the same physical causal history under refinement.

That criterion is not supplied by the words "physical" or "causal."

If the criterion is defined by preserving whichever relations a later `Σ` needs, the selection problem has returned upstream. If it preserves every relation, the structure becomes exhaustive. If it preserves only a chosen subset, the missing exclusion rule has simply been restated.

**Result:**

\[
\boxed{\text{refinement stability is unearned}}
\]

---

## 8. Pressure point E — Coarse-graining

The converse problem appears under coarse-graining.

Suppose a detailed history contains both process and material relations. Compressing it may produce a single transition that no longer explicitly contains both.

For the coarse representation to remain equivalent, `G*_phys` must specify what information is preserved by the abstraction and what information may be discarded.

But the candidate provides no identity-independent information-loss rule.

Three outcomes recur:

- preserve all structure: drift toward exhaustiveness;
- discard selected structure: require an independent exclusion rule;
- discard whatever later proves irrelevant to identity: hidden `Σ`.

Therefore coarse-graining exposes the same missing object from the opposite direction.

**Result:**

\[
\boxed{\text{coarse-graining stability is unearned}}
\]

---

## 9. Pressure point F — Is "physical" itself representation-invariant?

The deepest problem is now visible.

A physical state can be represented by different coordinate systems, variable factorizations, state-space decompositions, and levels of description without changing the underlying physical system.

If `G*_phys` is to be representation-independent, its membership cannot depend on one arbitrary factorization of the physical state space.

But if the candidate refuses all factorization choices, then it must specify a deeper structure from which the different causal descriptions are projections.

That returns directly to the architecture:

\[
G_P,G_M\rightarrow [\sim]\rightarrow G^*\rightarrow \Sigma.
\]

`G*_phys` was supposed to instantiate the `G*` slot. Instead, its definition still presupposes the unresolved answer to what counts as the same physically represented causal structure.

This is the concrete realization of the upstream problem isolated by Test A.

---

## 10. Pressure point G — The causal-counterfeit boundary

The candidate also faces the previously open causal-counterfeit burden.

Suppose a counterfeit is constructed so that its entire retained physical causal history is isomorphic to the genuine history under `G*_phys`.

Then:

\[
G^*_{\mathrm{phys}}(P)\cong G^*_{\mathrm{phys}}(R).
\]

At that point `G*_phys` cannot itself distinguish them.

That is not by itself a defect: `G*` is not supposed to be `Σ`.

The problem is that if the omitted distinction is physically real and would later be needed by `Σ`, then the candidate was too selective. If it is omitted because it is thought not to matter to identity, AR-6 is violated.

The candidate therefore cannot yet show that its boundary is sufficient for all legitimate later selections while remaining identity-neutral.

**Result:**

\[
\boxed{\text{causal-counterfeit sufficiency remains unearned}}
\]

This compounds, but does not independently create, the membership-boundary failure.

---

## 11. What survives the attack

The failure should be kept narrow.

The following claims remain intact:

1. A common structure can, in principle, retain process and material continuity without selecting between them.
2. Representation-useful selectivity need not be identity-selective.
3. A physical causal structure can preserve the perfect-counterfeit provenance distinction.
4. Fission and fusion can remain identity-neutral at the common-structure layer.
5. The exhaustive `G*` branch has not been tested and is not refuted by this candidate's failure.
6. No candidate `Σ` has been introduced.

What fails is specifically the claim that the concrete structure

\[
G^*_{\mathrm{phys}}=(V,E,\tau)
\]

has already supplied an independently bounded, representation-invariant selective membership rule.

It has not.

---

## 12. Exact failure classification

| Requirement | Result for `G*_1` |
|---|---|
| Identity neutrality | **Survives** |
| Theseus neutrality | **Survives** |
| Perfect-counterfeit preservation | **Survives** |
| Junction neutrality | **Survives** |
| Independent membership boundary | **Fails as specified** |
| Representation invariance | **Fails to be established; direct-edge repair fails** |
| Refinement stability | **Unestablished** |
| Coarse-graining stability | **Unestablished** |
| Causal-counterfeit sufficiency | **Unestablished** |
| Selective existence claim | **Fails** |

The important distinction is between **candidate failure** and **branch failure**.

\[
\boxed{G^*_1\text{ fails} \neq \text{selective }G^*\text{ is impossible}}
\]

The abstract selective branch remains open exactly as the previous usefulness test established.

---

## 13. Why a replacement is not generated here

The failure is informative enough that immediately constructing `G*_2` would obscure what was learned.

The first candidate has shown that the phrase "typed physical causal history" does not itself solve the membership problem. In particular, the following apparent repairs each move into a different branch:

- privileged physical factorization → an unprovided ontology-selection rule;
- all physical causal dependence → exhaustive `G*`;
- direct causal edges → representation-sensitive membership;
- quotient across representations → the unresolved `G\sim H` problem;
- identity-motivated exclusion → hidden `Σ`.

These are diagnoses, not invitations to choose one and continue.

No `G*_2` is constructed.

---

## 14. Current status

The concrete candidate `G*_1` is **failed as a concrete selective survivor**.

The broader selective branch remains **Open** because its abstract viability was not refuted. The exhaustive branch remains **Open and untested**.

The earned state is:

\[
\boxed{
\text{representation-useful}\neq\text{identity-useful}
}
\]

and separately:

\[
\boxed{
G^*_1\text{ does not supply the independently bounded representation-invariant structure required.}
}
\]

No Boundary against all selective `G*` has been earned.

No replacement candidate is generated.

No `Σ` is introduced.

No process/material preference is established.

The next legitimate work is to decide how the **selective existence question** and the separately open **exhaustive branch** should be attacked, without treating the failure of `G*_1` as a failure of the entire selective class.
