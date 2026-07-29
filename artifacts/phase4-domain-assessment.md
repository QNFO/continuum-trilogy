# Phase 4 — Stage 0: Domain Assessment
## Continuum Trilogy: Ontological Closure Program

**Date:** 2026-07-29  
**Project:** QNFO/continuum-trilogy (tag: v1.1.1-encoding-fix)  
**Papers:** 3 (~8,500 words total, 30 pages combined PDF)  
**Status:** STAGE 0 COMPLETE — ready for Stage 1  

---

## 1. Domain Topology Map

The Continuum Trilogy operates at the intersection of six domains. Below is the topology map showing active paradigms, open questions, and the trilogy's position within each.

### 1.1 Foundations of Physics — Ontology & Measurement

| Aspect | Status |
|:-------|:-------|
| **Core question** | What mathematical structure is physically real vs. purely descriptive? |
| **Active paradigm** | Operationalism (Bridgman), structural realism (Worrall/Ladyman), QBism (Fuchs) |
| **Trilogy position** | **Ontological Closure (OC):** physically real = Turing-approximable with computable modulus of convergence. Sharp, falsifiable, operational criterion. |
| **Key tension** | ZFC set theory provides uncountable ℝ; all measurement protocols produce rational-valued outputs. The trilogy resolves this not by rejecting ZFC but by declaring the excess reals *physically vacuous*. |
| **Predecessors** | Gisin (2019) "Real numbers are the hidden variables of classical mechanics"; constructivist mathematics (Bishop, Bridges); quantum Bayesianism operationalism |
| **Trilogy's novel contribution** | Generality — the OC criterion applies uniformly to ℝ and ℚ_p; it is not a "quantum-specific" or "classical-specific" restriction. |

### 1.2 Number Theory — p-adic Analysis & Adelic Constructions

| Aspect | Status |
|:-------|:-------|
| **Core question** | Do p-adic completions have any physical significance, or are they purely mathematical artifacts? |
| **Active paradigm** | Adelic physics (Volovich, Vladimirov, Zelenov 1990s-2000s); ultrametric dynamics in spin glasses (Mezard, Parisi, Virasoro); p-adic string theory (V.S. Vladimirov, I.Ya. Aref'eva) |
| **Trilogy position** | p-adic completions are **physically real as information carriers** (valuation-theoretic dimensions), not as geometric dimensions. Ostrowski's theorem partitions completions into one Archimedean place (∞, giving depth/continuity/causality) and infinitely many non-Archimedean places (p, giving discrete quantum numbers). |
| **Key tension** | Traditional adelic physics treats ALL places symmetrically. The trilogy breaks symmetry: only finitely many primes are physically relevant (those whose Bruhat-Tits buildings encode known quantum numbers). The "adelic ring" A_ℚ^c is the restricted product, not the full product. |
| **Predecessors** | Dragovich (2002) p-adic path integrals; Spiry (2017-2023) G-ultrametric physics; p-adic Wilson loops for confinement (Gubser 2010) |
| **Trilogy's novel contribution** | Linking specific primes to specific quantum numbers via Bruhat-Tits tree geometry: p=2 ↔ spin, p=3 ↔ color charge. This gives a *structural* (not mystical) reason why the Standard Model has the gauge group it does. |

### 1.3 Quantum Field Theory — Gauge Structure & Adelic Reformulation

| Aspect | Status |
|:-------|:-------|
| **Core question** | Is the Standard Model's gauge group SU(3)×SU(2)×U(1) arbitrary or structurally determined? |
| **Active paradigm** | GUT unification (SU(5), SO(10), E₈); string theory compactifications; anthropic landscape |
| **Trilogy position** | The gauge group decomposes by prime factors: SU(3)_C ↔ p=3, SU(2)_L ↔ p=2, U(1)_Y ↔ p=∞ (the Archimedean place). New gauge symmetries, if any, would correspond to additional primes — NOT to larger simple Lie groups containing the SM. This is a **number-theoretic constraint on BSM model building.** |
| **Key tension** | The trilogy proposes reformulating QFT over A_ℚ^c (computable adeles), not ℝ^4. This is a radical proposal — QFT is canonically formulated over ℝ^{3,1} (or ℝ^D for D-dimensional theories). The Archimedean projection of the adelic theory recovers familiar QFT; the non-Archimedean projection generates discrete structure currently modeled phenomenologically. |
| **Predecessors** | Adelic QFT programs (Volovich, Vladimirov); Connes' noncommutative geometry approach to the SM (Connes-Lott, Connes-Marcolli) |
| **Trilogy's novel contribution** | The *computable* restriction (A_ℚ^c, not the full adele ring A_ℚ) is unique to this program. Prior adelic physics treats the full adele ring as the arena; the trilogy's OC program restricts it to the computable subset, simultaneously solving the "uncountably many adeles" problem and the "which primes are physical" problem in one stroke. |

### 1.4 Computability Theory — Turing-Approximability as Physical Criterion

| Aspect | Status |
|:-------|:-------|
| **Core question** | Can Turing-approximability serve as a demarcation criterion for physical reality? |
| **Active paradigm** | Church-Turing thesis (effective computability captures "what is calculable"); algorithmic information theory (Chaitin); constructive analysis (Bishop, Beeson) |
| **Trilogy position** | **OC Criterion:** A quantity q is physically real iff ∃ a finite Turing-machine protocol that produces a sequence {q_n} with a computable modulus of convergence |q_n − q_{n+m}| < ε(m) where ε is computable. This is operational, measurement-theoretic, and domain-independent. |
| **Key tension** | The criterion *agrees with and extends* the Church-Turing thesis: if "physically measurable" = "computable by a physical device," then OC is simply making the measurement-theoretic claim explicit. It also shows that the Continuum Hypothesis is physically inert (no measurement can depend on CH). |
| **Predecessors** | Turing (1936) "On Computable Numbers"; Gandy (1980) physical Church-Turing thesis; Kieu (2003) quantum adiabatic computation and Hilbert's tenth problem |
| **Trilogy's novel contribution** | Extending computability from ℝ to ℚ_p and showing that p-adic approximation is structurally analogous (Turing machines over p-adic fields exist). The unified criterion across ALL completions of ℚ is new. |

### 1.5 Quantum Information — Error-Correcting Codes & Valuation Gaps

| Aspect | Status |
|:-------|:-------|
| **Core question** | Do p-adic valuation gaps provide a structural, non-design-level explanation for why certain QEC codes are optimal? |
| **Active paradigm** | Surface codes, toric codes (Kitaev); topological QEC; subsystem codes |
| **Trilogy position** | Optimal QEC codes exhibit p-adic valuation gaps (v_p^{max}) that are 7× higher for known optimal families than random codes. This is testable: construct code families, measure valuations. The prediction is structural — it follows from the Bruhat-Tits tree representation, not from an ansatz. |
| **Key tension** | This is an empirical prediction that has not yet been verified against a comprehensive dataset of QEC code parameters. The 7× figure is from "known families" — the calibration register entry (Stage 5) should track this. |
| **Predecessors** | Gromov hyperbolic groups and CAT(0) spaces; Bruhat-Tits buildings in representation theory |
| **Trilogy's novel contribution** | Linking a purely number-theoretic invariant (p-adic valuation) to a metric of physical performance (QEC code optimality) via Bruhat-Tits geometry. The Z_2 invariant (Dirac vs Majorana) is another concrete prediction. |

### 1.6 Philosophy of Mathematics — Physical Relevance of Set Theory

| Aspect | Status |
|:-------|:-------|
| **Core question** | If ZFC proves things about ℝ that are physically vacuous, what does that imply about the relationship between mathematics and physics? |
| **Active paradigm** | Platonism: mathematical objects exist independently; nominalism: they are linguistic conventions; structuralism: they exist as structure-placeholders |
| **Trilogy position** | **Operational structuralism:** ZFC proves true things about ℝ, but truth ≠ physical relevance. The continuum hypothesis is a legitimate mathematical question with no physical consequences. The dark continuum (ℝ \ ℝ_c) is a mathematically well-defined, physically vacuous object. This is NOT a rejection of ZFC — it is a demarcation between mathematical and physical existence. |
| **Key tension** | A hard-line Platonist would object: "If ℝ exists in the mathematical universe, how can parts of it be 'not physically real'?" The trilogy answers: the same way Hilbert space has non-normalizable vectors (mathematically well-defined, physically not states). Existence in the mathematical universe is not the same as participation in physical dynamics. |
| **Predecessors** | Wigner (1960) "The Unreasonable Effectiveness of Mathematics"; Tegmark's Mathematical Universe Hypothesis (opposite position); Ellis' epistemological realism |
| **Trilogy's novel contribution** | The OC criterion provides a **principled** (not ad hoc) demarcation. It does not say "we don't need uncountability" — it says "here is a falsifiable criterion, and uncountability fails it." A theory whose predictions change depending on |ℝ| = ℵ_1 vs |ℝ| > ℵ_1 is not a physical theory. |

---

## 2. Active Paradigm Landscape

| Paradigm | Proponents | Relationship to Continuum Trilogy |
|:---------|:-----------|:----------------------------------|
| **Standard Model EFT** | Mainstream HEP | The trilogy constrains (not contradicts) BSM model-building: new gauge groups at new primes |
| **String Theory** | Witten, Polchinski, et al. | Complementary: string theory is a candidate UV completion; the trilogy is a candidate IR constraint |
| **Adelic Physics** | Volovich, Vladimirov, Dragovich | Direct predecessor; trilogy adds computability restriction + specific prime assignments |
| **Ontological Closure (OC)** | QNFO (this project) | The trilogy is an OC instantiation and validation case |
| **Constructive Mathematics** | Bishop, Bridges, Richman | Overlapping methodology; trilogy is more permissive (accepts ZFC as a reasoning tool, only restricts physical domain) |
| **Quantum Bayesianism** | Fuchs, Schack, Mermin | Operationalist spirit aligned; trilogy extends operationalism beyond quantum foundations to continuum ontology |
| **Loop Quantum Gravity / Causal Sets** | Rovelli, Sorkin, et al. | Potential cross-test: if spacetime is fundamentally discrete, p-adic ultrametric structures may be more natural than real manifolds |

---

## 3. Key Research Questions (Domain-Level)

| # | Question | Urgency | Trilogy Addresses? |
|:--|:---------|:--------|:-------------------|
| RQ1 | What is the physical continuum? | High | **Yes — core claim of all 3 papers** |
| RQ2 | Are p-adic completions physically real? | Medium | **Yes — Paper II, Paper III §4-5** |
| RQ3 | Is the Standard Model gauge group structurally determined? | High | **Yes — Paper III §6.2, implicative claim** |
| RQ4 | What constrains beyond-Standard-Model physics? | High | **Yes — Paper III §6.2, prime-factor constraint** |
| RQ5 | Can the measurement problem be resolved number-theoretically? | Medium | **Yes — Paper III §6.3, speculative but falsifiable** |
| RQ6 | What is the role of uncountability in physics? | Low-Medium | **Yes — Paper I, the core negative result** |
| RQ7 | Does the Continuum Hypothesis have any physical consequences? | Low | **Yes — Paper III §5.2, definitive "no"** |
| RQ8 | What makes a QEC code optimal? | Medium | **Partially — Paper II §5, Paper III §6.1 (predictive)** |

---

## 4. Methodological Landscape

| Method | Used in Trilogy? | Notes |
|:-------|:-----------------|:------|
| **Mathematical proof** | Yes (Paper I — measurement indistinguishability theorem) | Theorem 4.3: non-computable reals are physically indistinguishable |
| **Empirical falsifiability** | Yes (all 3 papers list falsifiable predictions) | Valuation gaps, Z_2 invariant, gauge group decomposition |
| **Ontological argument** | Yes (OC criterion as demarcation) | Operational definition of physical reality |
| **Structural correspondence** | Yes (Bruhat-Tits ↔ quantum numbers) | p=2 ↔ spin, p=3 ↔ color |
| **Computational experiment** | Proposed but not executed | QEC code valuation measurements |
| **Literature synthesis** | Yes (34 papers classified in Phase 2) | Due diligence report at artifacts/literature-search.md |

---

## 5. Stage 0 Gate — PASS

| Gate | Status | Evidence |
|:-----|:-------|:---------|
| Domain topology mapped | ✅ PASS | 6 domains, each with paradigm analysis |
| Key research questions identified | ✅ PASS | 8 RQs, all relevant |
| Active paradigms inventoried | ✅ PASS | 7 paradigms, relationship analysis |
| Methodological landscape | ✅ PASS | 6 methods, with trilogy usage noted |
| No domain collisions detected | ✅ PASS | No QNFO-internal duplicate research found |

**Stage 0 is COMPLETE.** Proceed to Stage 1: Paradigm-Shift Candidate Identification.

---

## 6. Dependency on External Literature

See `artifacts/literature-search.md` (Phase 2 deliverable — 34 papers, KIF-18 symmetry template). Phase 2 classified 5 Core, 10 Supporting, 5 Background, 12 External, 2 Reject. The existing literature search is sufficient for Stage 1. No additional external search is required before proceeding.
