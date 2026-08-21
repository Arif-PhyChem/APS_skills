---
name: aps-prd
description: Evaluate a manuscript's fit for Physical Review D — particles, fields, gravitation, cosmology, astrophysics, and physics/cosmology-related astronomy.
journal: Physical Review D
abbreviation: PRD
journal_code: prd
publisher: American Physical Society
access_model: hybrid (SCOAP3 for qualifying HEP articles)
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation, aps-reference-format]
---

# Physical Review D — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for essentially every submission here** — PRD's subfields are among the most equation-dense in the portfolio, and the formalism is normally the contribution. See §Mathematical presentation profile below for this journal's
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

PRD is "a trusted journal for high-quality, significant developments in
elementary particle physics, field theory, gravitation, cosmology, astrophysics,
and physics and cosmology-related astronomy." Launched in 1970, it is "one of
the longest-established journals dedicated to serving the high-energy physics
community." As of 1 January 2018 PRD is part of the SCOAP³ consortium: all
high-energy-physics articles meeting SCOAP³ criteria published since that date
are made available open access.

## 2. Scope `[OFFICIAL]`

- Particle physics experiments
- Electroweak interactions
- Strong interactions
- Lattice field theories, lattice QCD
- Beyond the standard model physics
- Phenomenological aspects of field theory, general methods
- Gravity, cosmology, cosmic rays
- Astrophysics, astronomy, and astroparticle physics
- General relativity
- Formal aspects of field theory, field theory in curved space
- String theory, quantum gravity, gauge/gravity duality

Section-selection guidelines: `/prd/authors/guidelines-section-selection-physical-review-d`.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to elementary particle physics, field theory, gravitation, cosmology, and astrophysics.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRD's readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

PRD is the archival venue for HEP, gravitation, and cosmology — breadth of
subfields under one roof, with authority and completeness as the standard.
It absorbs both formal theory (string theory, quantum gravity) and data-driven
analysis (collider, gravitational-wave, cosmological surveys).

## 5. Strong-fit profile `[INFERENCE]`

- New calculations, phenomenological analyses, or constraints with clear
  comparison to data.
- Lattice results with controlled systematics and continuum extrapolation.
- Gravitational-wave or cosmological analyses with rigorous statistical treatment.
- Formal results with concrete consequences for models or observables.
- Definitive, complete treatments others will cite as the reference.

## 6. Weak-fit patterns `[HEURISTIC]`

- Model-building with no distinguishing prediction or constraint.
- Reanalysis with no new data, method, or conclusion.
- Statistical claims without look-elsewhere/systematics treatment.
- Nuclear-structure-first work (→ PRC).
- Instrument/accelerator-technology-first work (→ PRAB).
- Astronomy with no physics or cosmology bearing.

## 7. Evaluation framework

**A. Scope fit** · **B. Significance in the subfield** · **C. Novelty type**
(measurement / constraint / calculation / formalism / method) ·
**D. Systematics and statistics** · **E. Comparison to data and prior results** ·
**F. Completeness** · **G. Positioning vs. PRC / PRL / PRX / PRResearch.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Central PRD topic; substantive, rigorous, complete; reference-quality |
| **Strong** | Clearly in scope; solid significant contribution |
| **Moderate** | In scope; systematics, comparison, or significance framing needs strengthening |
| **Borderline** | Sits at the PRC boundary, or is astronomy with thin physics content |
| **Poor** | Outside scope, or no distinguishing contribution |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRC** | The core is nuclear structure, reactions, or nuclear astrophysics inputs |
| **PRL** | The advance is pivotal and broadly interesting |
| **PRX** | Field-defining discovery or landmark |
| **PRAB** | The core is accelerator and beam science |
| **PRE** | The core is statistical/nonlinear/complex-systems physics |
| **PRResearch** | Solid in-scope work where gold OA is wanted |
| **PRX Intelligence** | The central contribution is an AI/ML method |

Prefer **PRD** when: the contribution is a substantive result in particles,
fields, gravitation, cosmology, or related astrophysics.

## 10. Article types `[OFFICIAL]`

Detailed **research articles** and **Letters** (short papers of particular
importance). Flexible lengths; longer papers welcome. Definitions and limits:
`/prd/authors/editorial-policies-practices#articletypes`.

## 11. Open access note `[OFFICIAL]`

SCOAP³ applies to qualifying high-energy-physics articles published since
1 January 2018 — check eligibility and arXiv primary designation before
choosing a paid OA route.

## 12. Positioning advice `[HEURISTIC]`

- Lead with the constraint, measurement, or theoretical consequence.
- Make the comparison with existing bounds/results explicit and quantitative.
- Report systematics and statistical methodology in full; include priors and
  likelihood choices for inference work.
- For formal work, state the physical consequence or the class of models affected.
- Cite competing analyses fairly, including those reaching different conclusions.

## 13. Submission checklist

- [ ] PRD-domain central claim; PRC boundary checked
- [ ] Article type and section selected
- [ ] Systematics, statistics, and priors documented
- [ ] Comparison against existing results quantitative
- [ ] SCOAP³ eligibility checked
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 14. Decision workflow

1. Central contribution. 2. Domain test. 3. Novelty type. 4. Significance.
5. Statistical/systematic rigor. 6. Comparison to prior results. 7. Neighbor
comparison. 8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 15. Output format

Standard portfolio output block.

## 16. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRD-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Very High. Across field theory,
lattice QCD, gravitation, and cosmology, the mathematics generally *is* the
contribution; formal-theory subfields are among the most equation-dense in the
portfolio.

**Expected equation density:** High to very high for theory; moderate to high
for phenomenology and data analysis, where likelihoods and estimators still
belong in the text.

**Role of equations:** To define the theory, the action or Lagrangian, the
observable, and the inference procedure. Conventions matter: signature, units,
and normalization must be fixed explicitly or results cannot be compared.

**Main-text mathematical content:** The action or Lagrangian; the equations of
motion or evolution equations; the observable's definition; the likelihood,
priors, and estimator for inference work; the principal result; the
approximation or truncation scheme with its regime.

**Supplementary mathematical content:** Long derivations, loop-integral detail,
lattice-artifact and continuum-extrapolation analysis, systematic-error
decomposition, auxiliary limits.

**Recommended derivation depth:** Full — the readership checks derivations, and
completeness is expected. PRD's flexible length policy accommodates it.

**Figure–equation integration:** Exclusion plots and constraint contours should
state the likelihood and assumptions behind them; extrapolations should show the
fit form.

**Recommended presentation strategy:** `[HEURISTIC]` Fix conventions in one
early paragraph and keep them. For inference work, write the likelihood
explicitly — reporting a bound without the statistical model behind it is the
most common reproducibility complaint in this area.

## 17. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Letters | **4500 words** |
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
content. PRD's own guidance is that the appropriate length depends on the
information the article contains.

**Presentation priority:** Conventions and completeness. `[STRATEGY]` Fix signature, units, and normalization early; for inference work state the likelihood and priors in the main text.

## 18. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review D | https://journals.aps.org/prd/about | Official | 2026-08-19 | Identity, scope, criteria, article types, SCOAP3 |
| PRD editorial policies and practices | https://journals.aps.org/prd/authors/editorial-policies-practices | Official | 2026-08-19 | Article types (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prd/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
