---
name: aps-prxenergy
description: Evaluate a manuscript's fit for PRX Energy — APS's highly selective gold open access journal for renewable and sustainable energy research.
journal: PRX Energy
abbreviation: PRX Energy
journal_code: prxenergy
publisher: American Physical Society
access_model: gold open access
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation, aps-reference-format]
---

# PRX Energy — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for device-physics, transport, and any techno-economic or systems submission** — the model behind a projection must be auditable. See §Mathematical presentation profile below for this journal's
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

PRX Energy is "a highly selective open access journal for impactful renewable
and sustainable energy research… highly visible and multidisciplinary,
publishing energy science and technology research from physics and
physics-adjacent fields, including engineering and chemistry."

APS launched it at the forefront of the Society's commitment to a more
sustainable future. It provides a high-impact forum for the interdisciplinary
energy community, connects that community to physics, and maximizes
dissemination of significant, timely results. It builds on PRX's standards with
a focus on the energy research community.

## 2. Scope `[OFFICIAL]`

"All topics relevant to the multidisciplinary energy science and technology
research communities spanning physics, chemistry, materials, engineering,
biology, environmental studies, **and policy**." Coverage: fundamental and
applied; theoretical, experimental, computational, and data-intensive research,
including significant advances in methods and instrumentation; and
interdisciplinary and emerging areas. Full scope: `journals.aps.org/prxenergy/scope`.

> `[HEURISTIC]` Policy is explicitly in scope — unusual in the portfolio. Energy
> policy analysis with rigorous quantitative grounding is a legitimate submission.

## 3. Acceptance criteria `[OFFICIAL]`

Manuscripts should demonstrate exceptional achievements according to **at least
one**:

- **Exceptional advance** — pushing energy research, technology, and/or policy in a new and consequential direction.
- **Exceptional connection** — linking different areas within energy research, or between the field and other scientific disciplines.
- **Exceptional capabilities** — in engineering, computational concepts, techniques, materials, or methodologies allowing major challenges in the journal's topical areas to be solved.
- **Exceptional insight** — addressing a timely topic of high impact and interest across the multidisciplinary energy research community.

## 4. Editorial positioning `[INFERENCE]`

The exceptional tier of energy research. Solid energy-materials or
device work belongs at PRMaterials or PRApplied; PRX Energy wants work that
changes the trajectory of the field, including at system and policy scale.

## 5. Strong-fit profile `[INFERENCE]`

- Breakthroughs in conversion, storage, or transmission with system-level consequence.
- Work connecting materials/device advances to deployment-scale implications.
- Rigorous techno-economic or systems analysis that reframes a choice.
- Methodological advances enabling energy research at new scale or fidelity.
- Quantitatively grounded policy analysis with cross-community relevance.

## 6. Weak-fit patterns `[HEURISTIC]`

- Incremental efficiency improvements in a single device.
- Materials characterization with an energy motivation but no energy consequence.
- Modeling with unstated assumptions or no sensitivity analysis.
- Policy commentary without quantitative grounding.
- Solid work at ordinary significance — route to PRApplied/PRMaterials/PRResearch.

## 7. Evaluation framework

**A. Scope fit** · **B. Criterion match** · **C. System-level consequence** ·
**D. Quantitative rigor** (assumptions, sensitivity, uncertainty) ·
**E. Cross-community relevance** · **F. Benchmarking against incumbents** ·
**G. Positioning vs. PRApplied / PRMaterials / PRResearch / PRX.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Exceptional, well-evidenced advance with consequence beyond the immediate system |
| **Strong** | Meets a criterion; impact real though concentrated |
| **Moderate** | Important work whose exceptional claim needs stronger system-level or quantitative support |
| **Borderline** | Solid energy work at ordinary significance |
| **Poor** | Incremental device/material result, or ungrounded analysis |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRApplied** | Energy device work with physical insight at specialist tier |
| **PRMaterials** | The contribution is the energy material itself |
| **PRResearch** | Significant energy work not reaching "exceptional"; gold OA |
| **PRX** | The advance is a broad physics discovery |
| **PRE / PRFluids** | The core is transport, combustion, or flow physics |
| **PRX Intelligence** | The central contribution is an AI/ML method |

Prefer **PRX Energy** when: the work is exceptional and speaks to the
multidisciplinary energy community, including at system or policy scale.

## 10. Article types and requirements `[OFFICIAL]`

Original research articles and special content. Fetch `/prxenergy/authors` for
current article types and requirements. Gold open access; APC applies.

## 11. Positioning advice `[HEURISTIC]`

- Name the criterion; support it with the system-level consequence.
- Quantify against incumbent technology, not only against the authors' baseline.
- State assumptions and run sensitivity analysis for any techno-economic claim.
- Connect the physics/chemistry result to deployment implications explicitly.
- Avoid sustainability framing that the results do not support.

## 12. Submission checklist

- [ ] Named criterion with supporting evidence
- [ ] System-level consequence argued
- [ ] Assumptions, sensitivity, and uncertainty documented
- [ ] Benchmarked against incumbent technology
- [ ] Alternatives (PRApplied, PRMaterials, PRResearch) considered
- [ ] APC/funding or waiver eligibility settled
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Scope fit. 3. Criterion match. 4. System-level
consequence. 5. Quantitative rigor. 6. Cross-community relevance.
7. Neighbor comparison. 8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Criterion claimed:** advance / connection / capabilities / insight — justification.
**System-level consequence:** …

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRX Energy-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Moderate. The scope spans device
physics through systems and policy, so the appropriate formalism varies more
than in most titles.

**Expected equation density:** Low to moderate — higher for transport, kinetics,
and device modeling; lower for systems and policy analysis, where the rigor
lives in model assumptions and sensitivity analysis instead.

**Role of equations:** To define efficiency, loss, and cost models, and to make
system-level projections auditable. An energy claim rests on the model behind
it, so the model must be visible.

**Main-text mathematical content:** Efficiency or conversion definitions; the
loss budget; the transport or kinetic model where central; for techno-economic
work, the cost model with its assumptions and boundaries stated explicitly.

**Supplementary mathematical content:** Derivations, full parameter sets,
sensitivity and Monte-Carlo analysis, scenario definitions.

**Recommended derivation depth:** Low to moderate; state and validate models
rather than deriving standard results.

**Figure–equation integration:** Projections and scenario plots must identify
the model, its assumptions, and the sensitivity ranges behind them.

**Recommended presentation strategy:** `[HEURISTIC]` For any system-level or
techno-economic claim, state the model, its boundary conditions, and a
sensitivity analysis. An unstated assumption set is the most common weakness in
energy-systems submissions, and it undercuts exactly the system-level
consequence the journal's criteria reward.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Perspectives | **3000 words** |
| Tutorials | no length limit |
| **Reviews** | **7000 words** |
| Roadmaps | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.** Note the Review limit here (7000) is far shorter
than at PRMaterials/PRApplied (30,000) — do not generalize across journals.


**Article format:** Flexible, with short commentary formats.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Low to Moderate.

**Recommended main-text figure strategy:** `[STRATEGY]` Keep the benchmark
comparison against incumbent technology and the sensitivity analysis in the main
text; move scenario enumerations to Supplemental Material. A projection figure
without visible assumptions is not evidence.

**Supplementary-material role:** Full parameter sets, scenario definitions,
Monte-Carlo and sensitivity output, techno-economic model detail.

**Preferred narrative style:** Detailed exposition accessible across physics,
chemistry, engineering, and policy audiences.

**Recommended manuscript compactness:** Moderate.

**Presentation priority:** Auditable assumptions. `[STRATEGY]` State the model,
its boundaries, and its sensitivities where a reader will see them.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About PRX Energy | https://journals.aps.org/prxenergy/about | Official | 2026-08-19 | Identity, scope, criteria |
| PRX Energy scope | https://journals.aps.org/prxenergy/scope | Official | 2026-08-19 | Subject areas (fetch) |
| PRX Energy Information for Authors | https://journals.aps.org/prxenergy/authors | Official | 2026-08-19 | Article types (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prxenergy/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
