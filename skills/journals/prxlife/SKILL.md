---
name: aps-prxlife
description: Evaluate a manuscript's fit for PRX Life — APS's highly selective gold open access journal at the intersection of biology with physics, computer science, mathematics, and engineering.
journal: PRX Life
abbreviation: PRX Life
journal_code: prxlife
publisher: American Physical Society
access_model: gold open access
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# PRX Life — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` whenever a quantitative model carries the biological claim** — which is most of what this journal publishes. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

PRX Life is "a highly selective, multidisciplinary open access journal that
publishes impactful research at the intersection of biology with physics,
computer science, mathematics, and engineering," aiming "to shape the future of
life science." It is described as the **first interdisciplinary journal focused
exclusively on quantitative biological research**.

Distinctive features `[OFFICIAL]`:

- **Highly selective**, showcasing research with lasting and profound impact.
- **Open access** under CC-BY.
- **First *Physical Review* journal with a collaborative review process on all
  papers** — referees see and comment on each other's reports, helping authors
  receive coherent feedback.
- A personalized, responsive editorial process; flexible article lengths and formats.
- Promotion of all published articles, with newsworthy research pushed to media.

> `[HEURISTIC]` The collaborative review process is worth telling authors about:
> reports arrive reconciled rather than contradictory, which changes how a
> response letter should be planned.

## 2. Scope `[OFFICIAL]`

"All topics relevant to the diverse multidisciplinary biological physics
research communities," spanning physics, biology, bioengineering, biochemistry,
materials science, medicine, computer science, and mathematics. Experimental,
theoretical, computational, and data-intensive approaches, advances in methods
and instrumentation, and interdisciplinary/emerging areas are encouraged. Broad
areas include:

- **Molecular and subcellular processes** — nucleic acids and information processes; protein dynamics, structure, function; structural and molecular biology; membranes; genome organization; energy conversion and non-equilibrium phenomena; virology and self-assembly; synthetic biology; single-molecule manipulation.
- **Cellular organization, physiology, and dynamics** — cells, tissue, organoids; mechanobiology; molecular networks and omics; biomaterials; phase condensates; fluid and vascular flows.
- **Organismal, population, evolutionary, and ecological processes** — virus–host interaction and immune responses; development, signaling, pattern formation; collective animal behavior and emergent phenomena; epidemiology and human behavior; living and active matter; evolutionary and population dynamics; molecular evolution; sensing, adapting, and learning without the brain.
- **Neuroscience and artificial intelligence** — including sensory systems.

Fetch `/prxlife/about` or the journal scope page for the complete current list.

## 3. Acceptance criteria

`[OFFICIAL]` PRX Life states that it is highly selective, showcasing
"high-quality, innovative research with lasting and profound impact."

`[HEURISTIC]` **Unknown — a four-bullet "exceptional" criteria list of the kind
PRX Quantum, PRX Energy, and PRX Intelligence publish was not confirmed on the
about page at the access date.** Before advising an author, fetch
`/prxlife/authors` and use the journal's stated criteria verbatim. Until then,
evaluate against the PRX-family standard: impact, innovation, and durability,
with quantitative rigor.

## 4. Editorial positioning `[INFERENCE]`

Quantitative biology at a highly selective tier. The discriminator against PRE's
biological-physics section is selectivity and audience: PRE serves statistical/
soft-matter physicists; PRX Life serves the quantitative life-science community
across disciplines.

## 5. Strong-fit profile `[INFERENCE]`

- Quantitative measurement or theory that changes how a biological process is understood.
- Physical principles governing living matter, established across systems.
- Methods or instrumentation that unlock new biological measurements.
- Work bridging physics/CS/mathematics with an experimental biological question.
- Modeling with predictive, experimentally tested consequences.

## 6. Weak-fit patterns `[HEURISTIC]`

- Simulation of a biological model with no experimental contact or general principle.
- Bioinformatics pipelines with no quantitative biological insight.
- Physics formalism applied to biological language without biological consequence.
- Incremental single-system characterization.
- Clinical/medical results without a quantitative physical or computational core.

## 7. Evaluation framework

**A. Scope fit** · **B. Quantitative core** (is the biology quantitative?) ·
**C. Selectivity tier** (lasting and profound impact?) · **D. Cross-disciplinary
relevance** · **E. Experimental contact** · **F. Reproducibility and data** ·
**G. Positioning vs. PRE / PRApplied / PRX / PRResearch / PRX Intelligence.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | High-impact quantitative biology with cross-disciplinary reach and experimental grounding |
| **Strong** | Clearly in scope; impactful and rigorous |
| **Moderate** | In scope; impact or experimental contact needs strengthening |
| **Borderline** | Good work at PRE or PRResearch tier rather than PRX-family selectivity |
| **Poor** | No quantitative core, or no biological consequence |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRE** | The result is a general statistical/soft-matter/nonlinear principle for a physics readership |
| **PRApplied** | The work is biomedical device or bioelectronics engineering |
| **PRX** | The advance is a physics discovery beyond living systems |
| **PRX Intelligence** | The central contribution is an AI/ML method (including neuroscience-AI methodology) |
| **PRResearch** | Solid quantitative-biology work below the highly selective tier; gold OA |
| **PRL** | Pivotal and broadly interesting across physics |

Prefer **PRX Life** when: the work is high-impact quantitative life science
speaking to multiple communities.

## 10. Article types and requirements `[OFFICIAL]`

Flexible article lengths and formats. Fetch `/prxlife/authors` for current
article types, criteria, and requirements. Gold open access under CC-BY; APC applies.

## 11. Positioning advice `[HEURISTIC]`

- Lead with the biological insight, expressed quantitatively.
- Make experimental contact explicit; state which predictions were tested.
- Define terms for both audiences — physicists and biologists will both referee.
- Report data, code, and analysis pipelines fully.
- Plan the response letter for a collaborative review process: referees will
  have seen each other's reports.

## 12. Submission checklist

- [ ] Quantitative biological core
- [ ] Impact argued against the journal's stated criteria (fetched, not assumed)
- [ ] Experimental contact or testable predictions
- [ ] Accessible to both physics and biology referees
- [ ] Data/code/pipeline availability per APS open-science policy
- [ ] APC/funding or waiver eligibility settled
- [ ] Alternatives (PRE, PRResearch) considered
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Scope fit. 3. Quantitative-core test.
4. Selectivity tier. 5. Cross-disciplinary relevance. 6. Experimental contact.
7. Neighbor comparison. 8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Quantitative core:** what is measured/predicted quantitatively.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRX Life-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Moderate to High — the journal is
defined by *quantitative* biological research, so a mathematical or statistical
model is usually the quantitative core.

**Expected equation density:** Moderate. Density is constrained by a readership
spanning physics and biology; clarity outranks completeness in the main text.

**Role of equations:** To make a biological claim quantitative and testable —
kinetic and reaction models, stochastic dynamics, mechanical and elastic models,
population and evolutionary dynamics, or inference models for high-dimensional
data.

**Main-text mathematical content:** The model and its biological interpretation;
parameter definitions with units and measured values; the predicted observable;
the statistical model used for inference.

**Supplementary mathematical content:** Derivations, parameter-estimation
detail, sensitivity analysis, alternative models considered and rejected.

**Recommended derivation depth:** Low to moderate in the main text — biologists
must be able to follow the argument; put the algebra in supplementary material.

**Figure–equation integration:** Model predictions should be overlaid on
measured data, with parameters stated and clearly marked as fitted or
independently measured.

**Recommended presentation strategy:** `[HEURISTIC]` Define every symbol in
biological terms as well as mathematical ones — both communities referee here.
State which parameters were fitted and which were measured independently; a
model with many free parameters and no independent constraint is a standard
objection. Say what the model predicts that would falsify it.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Perspectives | **2500 words** |
| Reviews | **6000 words** |
| Tutorials | **6000 words** |
| Roadmaps | no length limit |
| Comments / Replies | **1500 words** |

**No figure limit is stated.**


**Article format:** Flexible article lengths and formats.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate — constrained by a dual physics/
biology readership.

**Recommended main-text figure strategy:** `[STRATEGY]` Keep figures overlaying
model predictions on measured data, with fitted and independently measured
parameters distinguished. Move raw imaging series, additional replicates, and
pipeline outputs to Supplemental Material.

**Supplementary-material role:** Replicates, imaging data, parameter-estimation
detail, alternative models considered, analysis pipelines.

**Preferred narrative style:** Detailed exposition legible to both physicists
and biologists — define every symbol biologically as well as mathematically.

**Recommended manuscript compactness:** Moderate.

**Presentation priority:** Quantitative claims with visible uncertainty, and an
explicit statement of what would falsify the model.

> `[OFFICIAL]` PRX Life runs a **collaborative review process on all papers** —
> referees see and comment on each other's reports. `[STRATEGY]` Plan the
> response letter as one coherent document rather than separate rebuttals.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About PRX Life | https://journals.aps.org/prxlife/about | Official | 2026-08-19 | Identity, scope, selectivity, collaborative review |
| PRX Life Information for Authors | https://journals.aps.org/prxlife/authors | Official | 2026-08-19 | Article types and stated criteria — **must be fetched before advising** |

**Unknown — not stated in official sources at access date:** the explicit
acceptance-criteria bullet list, acceptance rate, length limits, timelines.

**Format facts above verified from** `https://journals.aps.org/prxlife/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
