# Phase 4 — Stage 3: Red-Team Adversarial Challenge
## Continuum Trilogy: Ontological Closure Program

**Date:** 2026-07-29  
**Depends on:** Stage 2 Assumption Audit (`artifacts/phase4-assumption-audit.md`)  
**Status:** STAGE 3 COMPLETE — 5 adversary roles × 5 candidates = 25 challenge responses

---

## Role 1: Null-Hypothesis Defender
**Position:** "Nothing new here — status quo explains everything."

### vs Candidate #1 (ℝ_c Continuum)
**Challenge:** "Physicists already know measurements produce rational numbers. They already use floating-point arithmetic. They already accept that `all models are wrong, some are useful`. The claim that non-computable reals are `physically vacuous` adds zero operational value beyond what pragmatists already accept. You're relabeling a consensus as a revolution."

**Response:** Partially valid. The pragmatic consensus does NOT extend to the ontological claim. A physicist using ℝ for calculations while knowing only ℝ_c matters for measurement is holding inconsistent positions — they use ℝ's mathematical convenience but deny its physical reality when pressed. The trilogy makes this implicit tension explicit and proposes resolving it. The value-add is coherence, not novelty of practice.

**Severity: MEDIUM.** Does not threaten the claim's truth — only its framing as "new." Mitigation: recognize the pragmatic consensus in the paper's framing and distinguish "novel ontology" from "novel practice."

---

### vs Candidate #2 (p-adic Quantum Numbers)
**Challenge:** "The Standard Model ALREADY explains spin, color, and flavor via gauge group representations. SU(2) gives spin, SU(3) gives color — these are well-understood. Mapping p=2 to SU(2) and p=3 to SU(3) is numerology dressed in Bruhat-Tits formalism. You can ALWAYS map small primes to small Lie groups — there are only so many small numbers."

**Response:** Stronger challenge. The mapping p→gauge group must be systematic, not coincidental. If 2→SU(2) and 3→SU(3) are just pattern-matching on small numbers, the trilogy hasn't added anything beyond: "hey, these numbers match." The Z_2 invariant prediction partially addresses this by making a concrete, falsifiable prediction that doesn't depend on the prime→gauge mapping. But the structural claim (Bruhat-Tits geometry IS the origin of quantum numbers) remains unproven until a third independent mapping is found.

**Severity: HIGH.** The "coincidence of small numbers" objection is the most damaging to this candidate. Fixed only by a third confirmed prime→quantum number mapping (not just 2 and 3).

---

### vs Candidate #3 (CH Physically Inert)
**Challenge:** "This is obviously true and nobody disputes it. No physicist has ever claimed their measurements depend on |ℝ|. The Continuum Hypothesis has been known to be independent of ZFC since 1963. Claiming this as a 'paradigm shift' or even a 'candidate' is padding. It's like proving the Axiom of Choice has no physical consequences — a valid result, but not a discovery."

**Response:** Largely correct. The null-hypothesis defender wins this round. CH Inert IS essentially a corollary of the OC criterion. Its EV score (5.10, #1 ranking) reflects certainty, not novelty. The candidate should be REFRAMED: downgrade from "paradigm-shift candidate" to "supporting lemma" or "consistency check." Its role is to clear the ground for Candidates #1 and #2 — it proves that uncountability's most famous implication (CH) is physically inert, which removes the strongest objection to "we don't need uncountability in physics."

**Severity: LOW for truth, HIGH for framing.** The candidate is true; it's just not a candidate. Reclassify as Lemma 1 of the OC program.

---

### vs Candidate #4 (QEC Valuation Gaps)
**Challenge:** "QEC code families are numerically optimized. The parameters (n, k, d) are integers bounded by known inequalities (quantum Singleton bound, etc.). Finding that optimal codes' parameters have higher p-adic valuations than random ones is like finding that optimal codes have larger distance — it's a property of optimization, not of number theory. You're rediscovering that parameters get larger under optimization and calling it 'p-adic valuation gaps.'"

**Response:** Partially valid BUT testable. If the valuation gap is purely an artifact of parameter magnitude, the null hypothesis should hold: controlling for (n, k, d), the valuation distribution of optimal vs random codes should be indistinguishable. If a statistically significant gap remains after controlling for parameter magnitude, the number-theoretic explanation gains weight. This is exactly what the proposed empirical test checks. The null-hypothesis defender's objection IS the null hypothesis of the test — and the test is designed to reject it.

**Severity: LOW.** The objection is the null hypothesis of the empirical test. This is healthy — the candidate IS falsifiable.

---

### vs Candidate #5 (SM Gauge = Prime Factors)
**Challenge:** "SU(3), SU(2), U(1) → 3, 2, 1. These happen to be the first three numbers. U(1) isn't even a prime! You're fitting 3 data points to 3 parameters and claiming a structural discovery. This is p-hacking at the level of theoretical physics. Show me the gauge group at p=5, p=7, or any other prime, and I'll take this seriously. Until then, it's confirmation bias dressed in number theory."

**Response:** This is the MOST VALID challenge of the entire red-team exercise. The mapping rule is underspecified: WHY does p=3 → SU(3)? Why not p=3 → SO(3) or p=3 → G_2? Why does p=∞ → U(1)? The number-of-parameters argument is devastating: 3 known gauge factors → 3 primes/places → zero degrees of freedom for a structural claim.

**Severity: CRITICAL.** Candidate #5 is not yet a candidate — it's an observation that 3 and 2 appear in the SM gauge group and 3 and 2 are primes. This needs major theoretical development (a principled mapping rule) before it can be treated as a paradigm-shift candidate.

**Verdict: DOWNGRADE Candidate #5 to "observation" status.** Keep as a direction-setting insight, not an EV-scored candidate. Remove from portfolio allocation.

---

## Role 2: Methodology Skeptic
**Position:** "Your method is flawed — here's why."

### vs Candidate #1 (ℝ_c Continuum)
**Challenge:** "You prove that non-computable reals are measurement-indistinguishable FROM each other, but you don't prove they're indistinguishable FROM computable reals. A measurement that 'approximates π with error ε' is measuring the equivalence class of reals within ε — which includes BOTH the computable π and uncountably many non-computable reals π + δ. You didn't prove the measurement is measuring THE computable real rather than a halo of non-computable reals."

**Response:** Valid methodological concern. Theorem 4.3 of Paper I needs strengthening: the proof must show that the measurement CANNOT distinguish the equivalence class containing a computable real from the class containing a non-computable real, OR it must show that no measurement protocol can isolate a single non-computable real within its halo. The current proof shows pairwise indistinguishability among non-computable reals — the extension to "indistinguishable from computable shadows" is implied but not rigorously proven.

**Severity: HIGH.** This is a gap in Paper I's central theorem. Needs a lemma: "If x ∈ ℝ_c and y ∈ ℝ \ ℝ_c agree on all rational approximations with computable error bound, they are measurement-indistinguishable." The proof sketch is: any measurement's output is a rational; the rational is determined by the equivalence class of reals within ε; the class contains both computable and non-computable members. This should be explicit.

---

### vs Candidate #2 (p-adic Quantum Numbers)
**Challenge:** "You use Bruhat-Tits buildings — highly abstract, niche mathematical objects with essentially zero physics community literacy — to 'explain' quantum numbers. This is the classic 'explaining obscurum per obscurius' fallacy. Quantum numbers ARE well-explained by representation theory, which every physicist learns. Bruhat-Tits buildings are known to maybe 100 people worldwide. This is not an explanation; it's a translation into a less accessible formalism."

**Response:** Valid communication criticism, not a truth criticism. The mathematics being obscure does not make the claim false — it makes it hard to evaluate. However, the trilogy has a COMMUNICATION burden: if the formalism is inaccessible to the physics community, the claim cannot gain traction regardless of its truth. Mitigation: Paper II should include a "translation table" mapping Bruhat-Tits concepts to familiar physics concepts (vertex = quantum number value, edge = possible transition, boundary = measurement outcome space).

**Severity: MEDIUM.** Does not threaten truth — threatens adoption. The trilogy needs a pedagogical bridge.

---

### vs Candidate #3 (CH Inert)
**Challenge:** "You argue CH has no physical consequences because all measurements output rationals. But physical theories make CONTINUOUS predictions — the prediction might be a real-valued function f(t), not a single rational. If CH affects which real-valued functions exist, and physical theories predict specific functions, then CH could affect which predictions are possible. You haven't ruled out CH affecting the set of admissible physical laws."

**Response:** Stronger than the null-hypothesis challenge. The argument must be extended: not only are measurement OUTPUTS rational, but physical LAWS must be expressible in terms that don't depend on CH. Any "law" whose predictions change depending on |ℝ| would be making different predictions for two mathematically indistinguishable (by measurement) situations — which is operationally incoherent. The trilogy argues this via OC criterion (laws must be Turing-computable functionals), but the chain from OC→CH-Inert could be made more rigorous.

**Severity: LOW-MEDIUM.** The argument is solid but needs one additional step: explicit proof that any CH-dependent theory contradicts the OC criterion.

---

### vs Candidate #4 (QEC Valuation Gaps)
**Challenge:** "The ~7× figure is from 'known families' — how many families? Which ones? Was this a pre-registered test or a post-hoc observation? If you looked at known optimal codes, noticed their valuations were higher, and reported the ratio, you've committed the garden of forking paths: there are many ways to measure 'valuation gap' (max, mean, median; which primes; normalized by what), and selecting the one that gives the largest effect size is p-hacking."

**Response:** CRITICAL methodological concern. The empirical claim needs:
1. A pre-registered metric: "We will compute v_2^{max}, v_3^{max}, ..., v_p^{max} for the top-10 known code families and compare to random codes matched on (n, k, d)."
2. A Bonferroni correction for testing multiple primes.
3. Publication of the full dataset (not just the 7× summary).
4. A null distribution generated by permutation test, not asymptotic approximation.

Without this, the 7× figure is an anecdote, not evidence.

**Severity: HIGH.** The empirical claim is currently unvalidated. This is fixable (pre-register the test, run the survey) but has not been fixed yet.

---

### vs Candidate #5 (SM Gauge = Prime Factors)
**Challenge:** "Even WITH a principled mapping rule, you have a degrees-of-freedom problem. The SM has 3 gauge group factors. There are infinitely many primes. You're selecting 3 primes from infinitely many and claiming they correspond to the 3 gauge factors. The probability that ANY 3 primes 'match' ANY 3 Lie groups by some mapping rule is high by multiple comparisons — you're cherry-picking the primes that match and ignoring the ones that don't."

**Response:** The methodology skeptic joins the null-hypothesis defender in CRITICAL assessment. The finite-S hypothesis (Candidate #6) partially addresses this: only primes whose Bruhat-Tits buildings encode observed quantum numbers are "active." But this is circular — you're defining "active primes" as "primes that correspond to observed gauge groups" and then claiming the active primes correspond to observed gauge groups.

**Severity: CRITICAL.** Candidate #5 cannot survive this challenge without a predictive (not post-hoc) mapping rule. Until a rule exists that PREDICTS "p=5 → gauge group G" without already knowing G, this is not a scientific claim.

---

## Role 3: Better-Alternative Proposer
**Position:** "X already does this better."

### vs Candidate #1 (ℝ_c Continuum)
**Challenge:** "Smooth infinitesimal analysis (SIA) and synthetic differential geometry already provide a rigorous foundation for physics on a `computable' continuum without invoking Turing machines. SIA uses the smooth real line R (with nilpotent infinitesimals), which is constructive, avoids classical logic's excesses, and has been developed for physics applications (Kock, Moerdijk-Reyes). Why reinvent this with Turing computability when a well-developed alternative exists?"

**Response:** SIA is a valid alternative with some advantages (smoothness built in, no need for ε-δ) but different goals. SIA restricts logic (intuitionistic, no excluded middle), while the OC program restricts ontology (computability of entities, not logic). The OC approach has two advantages: (a) it works uniformly for ℝ AND ℚ_p (SIA is inherently Archimedean), and (b) it makes direct contact with measurement theory (Turing machines ≈ measurement protocols). The trilogy should acknowledge SIA as a parallel program using different methods toward a similar goal.

**Severity: LOW-MEDIUM.** SIA is complementary, not competing. Acknowledge it in the related-work section.

---

### vs Candidate #2 (p-adic Quantum Numbers)
**Challenge:** "Connes' noncommutative geometry (NCG) already derives the Standard Model gauge group and particle content from a spectral triple (Connes-Lott 1990, Connes-Marcolli 2008). NCG gives SU(3)×SU(2)×U(1) + the correct fermion representations + the Higgs — FAR more than p-adic Bruhat-Tits buildings. And NCG doesn't need primes — it works with spectral data. The trilogy's p-adic approach is less predictive than NCG, which has been developed for 30+ years."

**Response:** Strong challenge. NCG IS more developed and more predictive than the p-adic approach. However, NCG and the Bruhat-Tits approach may be COMPATIBLE: Connes' spectral triple uses the adele class space, which naturally involves all completions of ℚ. The trilogy's contribution could be reframed as providing the computable restriction (A_ℚ^c rather than A_ℚ) to NCG, making its ontology physically well-defined. This is a synthesis opportunity, not a competition.

**Severity: MEDIUM.** NCG is more developed; the trilogy should position itself as complementary (adding the computability constraint to adelic NCG) rather than competing.

---

### vs Candidate #3 (CH Inert)
**Challenge:** "Woodin's Ω-logic program (2001-2010) provides a coherent argument that CH is FALSE — that |ℝ| = ℵ_2. If Woodin is right and CH is objectively false, then a theory claiming CH-inertness is true but uninteresting — it's like proving the Axiom of Choice has no physical consequences. Correct, but not a 'candidate.' The better alternative is to not talk about CH at all and focus on candidates that make positive predictions."

**Response:** Agreed. As the null-hypothesis defender noted, CH Inert is a lemma, not a candidate. The better-alternative proposer reinforces: spend zero research resources on CH and redirect to Candidates #2 and #4 which make testable predictions.

**Severity: LOW.** This challenge confirms the reframing: downgrade CH Inert to Lemma 1.

---

### vs Candidate #4 (QEC Valuation Gaps)
**Challenge:** "The QEC community already has well-established optimality criteria: quantum Hamming bound, quantum Singleton bound, quantum Gilbert-Varshamov bound. These are information-theoretic, rigorous, and widely used. Adding p-adic valuations as a 'new' optimality criterion is like adding a numerological test to a well-understood statistical problem. If p-adic valuation correlates with optimality, it's because optimal codes push against the known bounds, not because of number theory."

**Response:** The correlation-vs-causation objection is valid (see Candidate #4's own assumptions audit, A4.3). But the better-alternative proposer is actually HELPING: the known bounds provide the NULL DISTRIBUTION for the empirical test. If optimal codes' valuations exceed what the known bounds predict (controlling for n,k,d), the number-theoretic explanation gains support. If they don't, the candidate fails cleanly.

**Severity: LOW.** The known bounds are the null model, not a competing explanation.

---

### vs Candidate #5 (SM Gauge = Prime Factors)
**Challenge:** "Grand Unified Theories (GUTs) — SU(5), SO(10), E₆, E₈ — provide a UNIFIED explanation of the SM gauge group structure. SU(5) contains SU(3)×SU(2)×U(1) as a subgroup. SO(10) gives a spinor representation containing one full generation of fermions. This is structural, predictive (proton decay, gauge coupling unification), and testable. The trilogy's p-adic 'explanation' has zero unifications, zero new predictions at accessible energies, and is not even wrong — it's unfalsifiable until a mapping rule exists."

**Response:** The best challenge so far. GUTs ARE more developed, more predictive, and more testable than the p-adic gauge hypothesis. However, GUTs have their own problems: proton decay not observed (Super-Kamiokande limits exclude minimal SU(5)), no gauge coupling unification without SUSY (and no SUSY at LHC), and the hierarchy problem unresolved. The trilogy's approach, if developed, would be COMPLEMENTARY: GUTs explain unification of gauge groups at high energy; the trilogy constrains WHICH gauge groups can appear at any energy. This is a different question.

**Severity: CRITICAL.** GUTs and NCG both provide better-developed alternatives. The trilogy should position against a different question — not "what unifies the gauge groups" but "what constrains the possible gauge groups in the first place."

---

## Role 4: Scaling Pessimist
**Position:** "Can't scale past N."

### vs Candidate #1 (ℝ_c Continuum)
**Challenge:** "Reformulating ALL of physics on ℝ_c instead of ℝ is a generational project. Every textbook, every graduate course, every numerical method paper would need updating. The arXiv contains ~2 million papers using real numbers. You're proposing to touch all of them. This is a 50+ year project with zero funding and zero institutional support. Even if true, it's not actionable."

**Response:** Valid concern about SCALE, not truth. The trilogy should NOT propose "rewriting all of physics" — that's a straw man. Instead: (1) the criterion is for ONTOLOGY, not for rewriting — physicists can keep using ℝ as a calculational tool while accepting ℝ_c as the physical arena, just as they use complex Hilbert spaces while accepting only normalized vectors are states; (2) the actionable claim is narrower: for theories where the distinction matters (foundations of QFT, quantum gravity, measurement theory), the OC criterion provides a principled constraint. The scaling challenge is addressed by limiting scope.

**Severity: LOW.** Make the scope limitation explicit.

---

### vs Candidate #2 (p-adic Quantum Numbers)
**Challenge:** "Bruhat-Tits buildings for SL_n(ℚ_p) are well-understood for n=2 (trees) and partially for n=3 (buildings of dimension 2). For larger n, they are combinatorially intractable. The Standard Model involves groups up to SU(3), but extensions (GUTs, flavor symmetries) involve larger groups. If the theory cannot handle these — and Bruhat-Tits buildings become exponentially complex — it cannot 'explain' gauge structure beyond the simplest cases."

**Response:** Legitimate scalability concern. Bruhat-Tits buildings become computationally unwieldy for rank > 2. The trilogy should acknowledge this: the approach works best for the low-rank groups relevant to current physics (SU(2), SU(3)), and scalability to larger groups is an open problem. This limits the theory to explaining what we ALREADY observe, which is the Candidate #5 problem again.

**Severity: MEDIUM.** Limits the theory's predictive scope but does not falsify it.

---

### vs Candidate #3 (CH Inert)
**Challenge:** "No scaling problem — this is a one-line proof that needs no resources. Move on."

**Severity: NONE.** Agreed. No scaling challenge exists for a lemma.

---

### vs Candidate #4 (QEC Valuation Gaps)
**Challenge:** "The space of QEC codes is astronomical. A 'comprehensive survey' of optimal code families means: for each (n,k,d) triple where n ≤ ~15 (beyond which exhaustive search is impossible), enumerate all codes, compute valuations, compare. Even this small subspace has billions of codes. A 'statistically significant' result requires thousands of data points. The compute cost of a rigorous survey exceeds available academic HPC resources by orders of magnitude."

**Response:** Partially valid but addressable. The survey doesn't need exhaustive enumeration — it needs INFORMED SAMPLING. Focus on (a) known optimal code families (Steane, Shor, surface codes — ~50 families), (b) random codes from standard constructions (CSS, stabilizer — ~500 samples per n), and (c) matched-parameter controls. A well-designed sampling strategy can achieve statistical significance with O(10^4) code evaluations, which is feasible on a workstation cluster. The scaling pessimist is right that EXHAUSTIVE search is impossible; but INFORMED sampling is tractable.

**Severity: MEDIUM.** Addressable with good experimental design.

---

### vs Candidate #5 (SM Gauge = Prime Factors)
**Challenge:** "This doesn't scale past n=3. You can't derive E₈ from p=something. You can't derive SO(10) from p=something. The theory is inherently limited to low-rank Lie groups that happen to correspond to small primes. If physics beyond the SM involves larger groups, the theory is silent. That's not a theory — it's a coincidence at small n."

**Response:** This is the scaling pessimist joining the methodology skeptic and better-alternative proposer in CRITICISM. The theory works only for the groups we ALREADY KNOW. It cannot predict new ones. This is the definition of a non-predictive theory.

**Severity: CRITICAL.** Candidate #5 is unfalsifiable — it can only "predict" what we already observe.

---

## Role 5: Resource Realist
**Position:** "Would cost $Y and take Z years — nobody will fund it."

### vs Candidate #1 (ℝ_c Continuum)
**Challenge:** "Foundations-of-physics research on continuum ontology has essentially zero funding. The NSF, ERC, and national funding agencies fund 'physics' — experiments, computations, theory with testable predictions within a 3-5 year horizon. 'What is the physical continuum?' is a question for philosophers, not physicists. The OC program will never receive grant funding at a level that sustains a research group."

**Response:** Partially true but missing the point. The trilogy's core insights (ℝ_c preserves physics, ℝ\ℝ_c is vacuous, ℚ_p encode quantum numbers) are intellectual contributions that don't require funding — they require (a) one clean paper, (b) public dissemination (Zenodo, arXiv, Buffer), and (c) time. The empirical test (QEC valuation gaps) needs modest computational resources (a workstation, not a grant). The grant-funded "adelic QFT" program is decades away, but the core claims are viable with zero funding.

**Severity: LOW.** Zero-funding viability is a feature, not a bug.

---

### vs Candidate #2 (p-adic Quantum Numbers)
**Challenge:** "The number of physicists who understand both Bruhat-Tits buildings AND Majorana zero modes is approximately zero. The number of condensed matter experimentalists who can test the Z_2 invariant is approximately zero. The number of theorists who can build on this work is approximately zero. Even if it's correct, the field is too small to sustain a research program."

**Response:** The resource realist misses that SMALL fields can GROW if the idea is compelling. The Z_2 invariant test CAN be framed in terms a condensed matter experimentalist understands: "Do Majorana zero modes in this platform carry a topological invariant that distinguishes them from Dirac modes? Here's how to measure it." The trilogy needs to translate its predictions into the LANGUAGE of the target experimental community. This is a communication burden (see Methodology Skeptic), not a resource constraint.

**Severity: MEDIUM.** Addressable through better communication and community-building.

---

### vs Candidate #3 (CH Inert)
**Challenge:** "Zero cost, zero years, zero funding needed. This is fine."

**Severity: NONE.** The resource realist has no objection to a free lemma.

---

### vs Candidate #4 (QEC Valuation Gaps)
**Challenge:** "A computational survey of QEC code families with p-adic valuation analysis: ~50 known optimal families + ~500 random codes × 10 primes × parameter extraction and valuation computation = ~50,000 code evaluations. At ~1 second per evaluation (conservative), that's ~14 hours of compute. Not expensive, but who does this work? A PhD student? A postdoc? This is a niche project that won't produce a PhD thesis by itself and won't justify a postdoc position. It falls between the cracks of 'too small for a grant, too big for a side project.'"

**Response:** The resource realist is RIGHT about the funding gap but WRONG about feasibility. This is EXACTLY the kind of project that can be done by an LLM-assisted researcher: write the code, run it on cloud compute (~$50 on AWS/Cloudflare Workers), produce the table, publish. No PhD student, no postdoc, no grant needed. This is a weekend project with the right automation.

**Severity: LOW.** Feasible with zero institutional resources — an LLM + cloud compute project.

---

### vs Candidate #5 (SM Gauge = Prime Factors)
**Challenge:** "Developing a principled prime→gauge-group mapping rule is a multi-year theoretical physics project requiring deep expertise in both number theory (adelic geometry, Langlands program) and quantum field theory (gauge theory, BRST, anomalies). This is a tenure-track professor's research program, not a paper. Nobody will fund it until Candidates #1 and #2 are established — and those need years themselves. This is a 2040 project, not a 2026 project."

**Response:** The resource realist delivers the final blow to Candidate #5. Even if a mapping rule exists (which is uncertain), finding it requires expertise, time, and resources far beyond the trilogy's current scope. This should be reframed as a "frontier question" — not a near-term research program.

**Severity: CRITICAL for actionability.** Candidate #5 is not actionable in the near term.

---

## Stage 3 Synthesis: Red-Team Verdicts

| Candidate | Null-Hyp | Method | Better-Alt | Scale | Resources | **Overall** |
|:----------|:--------:|:------:|:----------:|:-----:|:---------:|:-----------:|
| **#1 ℝ_c** | MEDIUM | HIGH | LOW-MED | LOW | LOW | **PASS** — gap in Theorem 4.3 needs strengthening; otherwise robust |
| **#2 p-adic QNs** | HIGH | MEDIUM | MEDIUM | MEDIUM | MEDIUM | **CONDITIONAL PASS** — needs Z_2 invariant test + third prime mapping |
| **#3 CH Inert** | LOW* | LOW-MED | LOW | NONE | NONE | **DOWNGRADE → Lemma 1** — true but not a candidate |
| **#4 QEC Gaps** | LOW | HIGH | LOW | MEDIUM | LOW | **CONDITIONAL PASS** — needs pre-registered empirical test |
| **#5 SM Gauge** | CRITICAL | CRITICAL | CRITICAL | CRITICAL | CRITICAL | **REJECT** — unfalsifiable, underspecified, non-predictive |

*Framing criticism only — truth not in dispute.

### Revised Portfolio (Post-Red-Team)

| Rank | Candidate | EV | Allocation | Change |
|:----:|:----------|:--:|:----------:|:------:|
| 1 | #2 p-adic QNs | 2.48 | **35%** | ↑5% |
| 2 | #1 ℝ_c | 2.84 | **30%** | ↑5% |
| 3 | #4 QEC Gaps | 1.40 | **25%** | ↑5% |
| 4 | #6 Finite S | 0.23 | **5%** | — |
| 5 | #7 Adelic QFT | 0.06 | **3%** | — |
| 6 | #8 Measurement | 0.02 | **2%** | — |
| ~~3~~ | ~~#3 CH Inert~~ | — | — | **→ Lemma 1** |
| ~~5~~ | ~~#5 SM Gauge~~ | — | — | **→ Observation** |

**Key changes:** Candidate #5 is demoted from the portfolio entirely — it is not yet a scientific claim. Candidate #3 is recategorized as a supporting lemma. Resources reallocated to Candidates #2 (most novel) and #4 (most testable).

---

## Stage 3 Gate — PASS

| Gate | Status |
|:-----|:-------|
| 5 adversary roles applied to top 5 candidates | ✅ PASS (25 challenge responses) |
| Verdicts rendered for each candidate | ✅ PASS |
| Portfolio reallocation reflects red-team findings | ✅ PASS |
| Stage 3 committed to artifacts/ | Pending (same-turn commit below) |
