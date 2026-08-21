---
name: aps-prc
description: Evaluate a manuscript's fit for Physical Review C — APS's journal for experimental and theoretical nuclear physics.
journal: Physical Review C
abbreviation: PRC
journal_code: prc
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

# Physical Review C — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for theory submissions, and for experiments whose extraction formalism carries the result** — which is most of PRC. See §Mathematical presentation profile below for this journal's
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

PRC is "a trusted journal for high-quality, significant developments in nuclear
physics." Established in 1970, it describes itself as "The Home of Nuclear
Physics" — "a trusted, essential resource for nuclear physics researchers,
nuclear data aggregators and evaluators, and others who use nuclear science
research results."

> `[INFERENCE]` The explicit mention of **nuclear data aggregators and
> evaluators** is distinctive: PRC's readership includes people who consume
> results as data. Completeness, tabulated results, and uncertainty reporting
> carry unusual weight here.

## 2. Scope `[OFFICIAL]`

Experimental and theoretical results in all aspects of nuclear physics:

- Nucleon-nucleon interaction, few-body systems
- Nuclear structure
- Nuclear reactions
- Relativistic nuclear collisions
- Hadronic physics and QCD
- Electroweak interaction, symmetries
- Nuclear astrophysics

Section-selection guidelines: `/prc/authors/guidelines-section-selection-physical-review-c`.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to nuclear physics.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRC's readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

Archival authority for nuclear physics. PRC explicitly notes a **flexible
approach to article lengths** and welcomes longer papers "that provide depth and
authority" — a signal that thoroughness is rewarded rather than penalized.
PRC also **fully supports structured abstracts** (background, purpose, methods,
results, conclusions) `[OFFICIAL]`.

## 5. Strong-fit profile `[INFERENCE]`

- New measurements of nuclear structure, reactions, or decay with full
  uncertainty analysis.
- Theoretical calculations benchmarked against data with quantified accuracy.
- Systematic studies across isotopic or energy ranges.
- Results usable by data evaluators — tabulated, complete, reproducible.
- Nuclear-astrophysics results connecting nuclear inputs to observables.

## 6. Weak-fit patterns `[HEURISTIC]`

- Model calculations with no benchmark against data or other models.
- Single measurements without systematic-uncertainty treatment.
- Parameter refits of established models with no new physics.
- Particle/field-theory-first work (→ PRD).
- Detector/accelerator-technology-first work (→ PRAB or an instrumentation venue).

## 7. Evaluation framework

**A. Scope fit** · **B. Significance in the nuclear community** ·
**C. Novelty type** (measurement / method / theory / systematics) ·
**D. Uncertainty and systematics** · **E. Data usability and completeness** ·
**F. Benchmarking** · **G. Positioning vs. PRD / PRL / PRAB / PRResearch.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Central nuclear-physics result, complete, authoritative, fully characterized |
| **Strong** | Clearly in scope; solid significant contribution |
| **Moderate** | In scope; uncertainty treatment, benchmarking, or significance framing needs work |
| **Borderline** | Sits at the PRD or PRAB boundary |
| **Poor** | Not nuclear physics, or contribution is not substantive |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRD** | The core is particle physics, field theory, gravitation, cosmology, or astroparticle physics |
| **PRL** | The advance is pivotal and broadly interesting across physics |
| **PRAB** | The core is accelerator/beam science or technology |
| **PRE** | The core is statistical or computational physics in general form |
| **PRX** | Field-defining discovery |
| **PRResearch** | Solid in-scope work where gold OA is wanted |
| **PRX Intelligence** | The central contribution is an AI/ML method |

Prefer **PRC** when: the contribution is a substantive nuclear-physics result
for the nuclear community, including data-consuming users.

## 10. Article types `[OFFICIAL]`

Detailed **research articles** and **Letters** (short, length-restricted papers
of particular importance). Flexible lengths; longer papers welcome. Structured
abstracts supported. Limits: `/prc/authors#article`.

## 11. Open access note `[OFFICIAL]`

Since 1 January 2018, PRC participates in SCOAP³: high-energy-physics articles
posted on arXiv under one of the four `hep` primary designations are made open
access under a CC-BY license.

## 12. Positioning advice `[HEURISTIC]`

- Use the structured abstract when the work is measurement- or method-heavy.
- Report full uncertainty budgets; separate statistical and systematic.
- Tabulate results so evaluators can use them; put full tables in supplemental
  material if long.
- Benchmark theory against existing data and competing models explicitly.
- State the nuclear-physics consequence, not just the number.

## 13. Submission checklist

- [ ] Nuclear-physics central claim
- [ ] PRD/PRAB boundary checked
- [ ] Article type and section selected
- [ ] Uncertainties complete and separated
- [ ] Results tabulated and reusable
- [ ] Benchmarks against data/models included
- [ ] SCOAP³ eligibility considered (arXiv `hep` designation)
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 14. Decision workflow

1. Central contribution. 2. Domain test. 3. Novelty type. 4. Significance.
5. Uncertainty/benchmarking rigor. 6. Data usability. 7. Neighbor comparison.
8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 15. Output format

Standard portfolio output block, plus:
**Data usability:** are results complete and reusable by evaluators?

## 16. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRC-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High — interaction models,
transition operators, reaction formalisms, and statistical decay treatments are
generally stated explicitly.

**Expected equation density:** High for theory; moderate for experiment, where
the extraction formalism linking yields to observables still belongs in the text.

**Role of equations:** To define the model and to make the extraction chain from
raw measurement to reported quantity auditable. PRC's readership includes data
evaluators, so the formalism is part of the data's usability.

**Main-text mathematical content:** The interaction or reaction model; the
observable's definition; the extraction formalism and its assumptions; the
principal result; uncertainty propagation expressions where they matter.

**Supplementary mathematical content:** Full derivations, angular-momentum
algebra, extended parameter tables, auxiliary corrections.

**Recommended derivation depth:** Moderate to full; PRC welcomes longer papers
providing depth and authority.

**Figure–equation integration:** Cross sections, spectra, and distributions
should be tied to the defining expressions; theory curves should name the
equation and parameter set that produced them.

**Recommended presentation strategy:** `[HEURISTIC]` Make uncertainty
propagation explicit rather than reporting a final error bar with no expression —
evaluators need to know what was propagated and how. Where the journal's
structured-abstract format is used, the methods field should name the formalism.

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
| Comments / Replies | 1500 words |

**No figure limit is stated.** Appendixes are used here — **not** PRL's End Matter.


**Article format:** Full-length by default; Letters available for short,
important results.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** High (see §Mathematical presentation profile).

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
content. PRC's own guidance is that the appropriate length depends on the
information the article contains.

**Presentation priority:** Data usability. `[STRATEGY]` Tabulate results so nuclear-data evaluators can reuse them; long tables belong in Supplemental Material, but the extraction formalism belongs in the main text. `[CONVENTION]` PRC supports structured abstracts.

## 18. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review C | https://journals.aps.org/prc/about | Official | 2026-08-19 | Identity, scope, criteria, article types, SCOAP3, structured abstracts |
| PRC section selection | https://journals.aps.org/prc/authors/guidelines-section-selection-physical-review-c | Official | 2026-08-19 | Sections (fetch) |
| PRC structured abstracts announcement | https://journals.aps.org/prc/edannounce/PhysRevC.84.030001 | Official | 2026-08-19 | Structured abstract support |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prc/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
