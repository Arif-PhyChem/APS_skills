---
name: aps-pre
description: Evaluate a manuscript's fit for Physical Review E — statistical, nonlinear, complex systems, biological, soft matter, fluids, plasma, and computational physics including machine learning and AI.
journal: Physical Review E
abbreviation: PRE
journal_code: pre
publisher: American Physical Society
access_model: hybrid
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation, aps-reference-format]
---

# Physical Review E — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for essentially every submission here** — scaling forms and governing stochastic equations are how a PRE result becomes general. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

**Load `aps-reference-format` whenever building, reviewing, or auditing the
reference list** — numbering and citation mechanics apply portfolio-wide; check
this journal's own skill only for a journal-specific addition (PRL's
titles-in-references convention is the only one on record).

## 1. Identity `[OFFICIAL]`

PRE is "a trusted and interdisciplinary journal for high-quality, significant
developments in the interrelated areas of statistical, nonlinear, complex
systems, biological, soft matter, fluids, plasma and computational physics,
**including machine learning and artificial intelligence**." Established in
1993, it is "distinguished by the breadth of the subject areas it covers and its
wide distribution and readership."

## 2. Scope `[OFFICIAL]`

- Statistical physics
- Nonlinear dynamics and chaos
- Networks and complex systems
- Biological physics
- Soft matter including polymers, liquid crystals, and granular materials
- Mechanics, interfaces, and films
- Fluid dynamics
- Plasma physics
- **Computational physics, machine learning, and artificial intelligence**

Section-selection guidelines: `/pre/authors/guidelines-section-selection-physical-review-e`.

> `[OFFICIAL]` PRE carries a named section for computational physics, machine
> learning, and artificial intelligence. `[INFERENCE]` This makes PRE a genuine
> alternative to PRX Intelligence for ML work — the difference is tier and
> framing, not scope. PRE asks for a significant contribution in a research
> area; PRX Intelligence asks for an *exceptional* achievement plus a validation
> gate.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to statistical, nonlinear, biological, and soft matter physics.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRE's general readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

PRE prizes **generality and mechanism**. Its readership crosses subfields, so
work framed as a general principle — a scaling law, a universality class, a
dynamical mechanism, a model that transfers — sits better than a one-system
report. PRE also hosts the **Irwin Oppenheim Award** for early-career authors
`[OFFICIAL]`.

## 5. Strong-fit profile `[INFERENCE]`

- New statistical-mechanical results, scaling behavior, or universality.
- Nonlinear-dynamics mechanisms with general applicability.
- Network/complex-systems results with analytical grounding.
- Soft-matter or active-matter physics with mechanism.
- Biological-physics work where physics is the explanatory frame.
- Computational or ML methodology that advances physics computation, with
  validation and interpretation.

## 6. Weak-fit patterns `[HEURISTIC]`

- Single-model simulation with no general lesson.
- Network analysis of a dataset with no physics or general principle.
- ML applied to a physics dataset with metric improvements only.
- Fluid-dynamics work better served by PRFluids' specialist readership.
- Condensed-matter-specific results (→ PRB).
- Biological work with no quantitative physical framing (→ PRX Life).

## 7. Evaluation framework

**A. Scope fit** · **B. Generality** (does it transfer?) · **C. Mechanism vs.
observation** · **D. Novelty type** · **E. Analytical/numerical rigor** ·
**F. Cross-subfield interest** · **G. Positioning vs. PRFluids / PRX Life /
PRB / PRX Intelligence / PRResearch.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | General, mechanistic result of interest across PRE's subfields; rigorous |
| **Strong** | Clearly in scope; significant contribution within an area |
| **Moderate** | In scope; needs stronger generality, mechanism, or validation |
| **Borderline** | A specialist neighbor (PRFluids, PRX Life, PRB) fits the readership better |
| **Poor** | Application report with no physics principle |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRFluids** | Fluid dynamics is the subject and the fluids community is the audience |
| **PRX Life** | The work is quantitative biology/living systems at a highly selective tier |
| **PRB** | The physics is specifically condensed-matter |
| **PRMaterials** | The subject is soft materials as materials — synthesis, processing, function |
| **PRX Intelligence** | The AI/ML contribution is central and exceptional, with SOTA validation |
| **PRL / PRX** | Pivotal or field-defining |
| **PRResearch** | Solid in-scope work where gold OA is wanted |
| **PRE (prefer)** | The result is a general physical principle across statistical, nonlinear, soft, or complex systems |

## 10. Article types `[OFFICIAL]`

Detailed **research articles** and **Letters** (short papers of particular
importance). Flexible lengths; longer papers welcome. Limits: `/pre/authors#article`.

## 11. Positioning advice `[HEURISTIC]`

- Frame the result as a principle, then demonstrate it on the system.
- State the universality/transferability claim explicitly and test it on at
  least a second system where feasible.
- Provide analytical support or scaling arguments alongside simulation.
- For ML work, include physical interpretation and non-ML baselines; decide
  deliberately between PRE and PRX Intelligence and say why.
- Report finite-size effects, convergence, and statistical error.

## 12. Submission checklist

- [ ] General principle identified, not just a system report
- [ ] Correct journal vs. PRFluids / PRX Life / PRB / PRX Intelligence
- [ ] Article type and section selected (note the computational/ML/AI section)
- [ ] Finite-size, convergence, and statistical errors reported
- [ ] Analytical grounding where possible
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Scope fit. 3. Generality test. 4. Mechanism test.
5. Rigor. 6. Cross-subfield interest. 7. Neighbor comparison. 8.
Vulnerabilities. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Generality:** what transfers beyond the studied system.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRE-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Very High for statistical physics,
nonlinear dynamics, and stochastic-process work; high for soft matter and
networks; moderate for computational and ML-focused submissions.

**Expected equation density:** High. Master equations, Langevin and Fokker–
Planck equations, free-energy functionals, scaling forms, and correlation
functions are the field's native language.

**Role of equations:** To express **generality**. PRE's readership crosses
subfields, and a scaling relation or universality argument is what makes a
single-system result transferable. The equation is how a specific model becomes
a general claim.

**Main-text mathematical content:** The model definition; the governing
stochastic or kinetic equation; the scaling ansatz or free-energy functional;
the principal analytical result; exponent definitions and the relations among
them.

**Supplementary mathematical content:** Derivations, perturbative expansions,
finite-size-scaling analysis, numerical implementation details.

**Recommended derivation depth:** Moderate to full — analytical support
alongside simulation materially strengthens a PRE submission.

**Figure–equation integration:** Data collapse is the characteristic PRE figure
and is meaningless without the scaling form written down. Every exponent plotted
should be defined mathematically.

**Recommended presentation strategy:** `[HEURISTIC]` Write the general relation
first and the specific system second. For work in the computational/ML/AI
section, still provide a mathematical statement of what is being learned or
approximated — a physics-free architecture description reads as a weak fit here.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Regular Articles | **no length limit** |
| Letters | **4500 words** |
| Perspectives | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.** Appendixes are used here — **not** PRL's End Matter.


**Article format:** Full-length by default; Letters available for short,
important results.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Very High (see §Mathematical presentation profile).

**Recommended main-text figure strategy:** `[STRATEGY]` Derived from the
argument. With no length limit on the full-length type, there is no format
pressure to remove evidence from the main text; the discipline required is
against *padding*, not against completeness.

**Supplementary-material role:** Extended derivations, robustness and
convergence analysis, secondary results, full parameter and data tables,
implementation detail.

**Preferred narrative style:** Detailed exposition with systematic development
and complete methodology.

**Recommended manuscript compactness:** Low to Moderate — length should follow
content. PRE's own guidance is that the appropriate length depends on the
information the article contains.

**Presentation priority:** Generality. `[STRATEGY]` Lead with the principle and use the system as demonstration; a data collapse needs its scaling form in the main text.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review E | https://journals.aps.org/pre/about | Official | 2026-08-19 | Identity, scope (incl. ML/AI), criteria, article types, Oppenheim Award |
| PRE section selection | https://journals.aps.org/pre/authors/guidelines-section-selection-physical-review-e | Official | 2026-08-19 | Sections (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/pre/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
