---
name: aps-prmaterials
description: Evaluate a manuscript's fit for Physical Review Materials — APS's multidisciplinary journal for materials research across physics, chemistry, and engineering.
journal: Physical Review Materials
abbreviation: PRMaterials
journal_code: prmaterials
publisher: American Physical Society
access_model: hybrid
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# Physical Review Materials — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` when the submission is modeling-, prediction-, or structure–property-driven.** Skip it for synthesis and characterization work, where added formalism displaces the detail readers need. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

PRMaterials is "a trusted journal for high-quality, significant developments in
materials research," publishing "multidisciplinary research across materials
science, physics, chemistry and engineering." It serves "the expanding community
of physicists, materials scientists, chemists, engineers, and scientists in
related disciplines," and "expands the scope of *Physical Review*'s journals,
providing an explicit focus on materials research."

## 2. Scope `[OFFICIAL]`

- Topological materials
- Two-dimensional materials
- Magnetic, ferroelectric, and multiferroic materials
- Superconducting materials
- Semiconducting materials
- Materials for energy harvesting, storage, and generation
- Materials for quantum technologies
- Nanomaterials, nanostructures, and nanocomposites
- Metamaterials and plasmonic, optical, and photonic materials
- Soft materials, polymers, and self-assembly
- Biomaterials
- Materials for catalysis and electrochemistry, including photocatalysis and electrocatalysis
- Electronic materials, metals, and dielectrics, including organics
- Mechanical properties, materials structure, and phase transformations
- Glasses and amorphous materials
- Prediction, synthesis, design, and modeling of materials
- Crystal growth, film growth, crystallization, and kinetics
- Thin films, interfaces, surfaces, and heterostructures

Section-selection guidelines: `/prmaterials/authors/guidelines-section-selection-physical-review-materials`.

> `[INFERENCE]` Note what PRB's list does not contain and this one does:
> synthesis, growth, processing, kinetics, catalysis, biomaterials, and
> materials *design*. That gap is the PRB/PRMaterials boundary.

## 3. Acceptance criteria `[OFFICIAL]`

- Present important results that significantly advance the field of material research.
- Generate interest for PRMaterials' readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

The organizing question is **materials-centric**, not mechanism-centric:

> Does this advance what the materials community can make, measure, predict, or
> use?

A paper about the physics *of* a material leans PRB. A paper about the material
— its synthesis, structure, processing, design, or functional properties for a
community that works with materials — leans PRMaterials. Both may be excellent.

## 5. Strong-fit profile `[INFERENCE]`

- New material or material class with characterized, significant properties.
- Synthesis, growth, or processing advance that changes what is achievable.
- Structure–property relationships established across a family of materials.
- Predictive design or high-throughput work that produces validated, actionable
  materials outcomes.
- Interface, thin-film, or heterostructure engineering with clear consequences.

## 6. Weak-fit patterns `[HEURISTIC]`

- Screening exercises reporting computed numbers with no interpretation,
  validation, or actionable outcome.
- Single-composition characterization with no wider materials significance.
- Device-performance papers (→ PRApplied).
- Deep mechanism papers where the material is incidental (→ PRB).
- Chemistry-first synthesis with no physical property characterization.
- ML pipelines for materials discovery with no experimentally or computationally
  validated material outcome (→ PRX Intelligence, or strengthen the materials result).

## 7. Evaluation framework

**A. Scope fit** (materials-centric?) · **B. Materials significance** ·
**C. Novelty type** (material / synthesis / property / structure–property /
design method) · **D. Characterization completeness** · **E. Community
relevance** · **F. Validation** · **G. Positioning vs. PRB / PRApplied /
PRX Intelligence / PRE.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Important, well-characterized materials advance with clear consequence for the materials community |
| **Strong** | Clearly in scope; meaningful, well-supported materials result |
| **Moderate** | In scope; characterization, validation, or significance framing incomplete |
| **Borderline** | Materials-adjacent, but the real contribution is mechanism (PRB), device (PRApplied), or method (PRX Intelligence) |
| **Poor** | No materials advance — a screening table, a device metric, or a method demo |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRB** | The contribution is the underlying condensed-matter physics — mechanism, electronic structure, phase behavior — for a condensed-matter readership |
| **PRApplied** | The claim concerns a device, application, or applications-based physical phenomenon |
| **PRX Intelligence** | The contribution is the AI/ML materials-discovery method itself |
| **PRE** | Soft matter, polymers, or granular materials treated as statistical/soft-matter physics |
| **PRX Energy** | Energy is the defining domain and the work is exceptional |
| **PRL / PRX** | The materials advance is pivotal or field-defining and broadly interesting |
| **PRResearch** | Solid materials work where gold OA is wanted |

Prefer **PRMaterials** when: the audience is the multidisciplinary materials
community and the result is about the material.

## 10. Article types `[OFFICIAL]`

PRMaterials publishes **Review Articles**, **Research Updates**, detailed
**Research Articles**, and **Letters** (short papers of particular significance
and/or topical interest).

`[OFFICIAL]` Verified limits (2026-08-19): Regular Articles — no length limit;
Letters — 4500 words; Research Updates — 10,000 words; Review Articles — 30,000
words; Comments/Replies — 3500 words. Re-verify at
`/prmaterials/authors` before advising.

> `[HEURISTIC]` **Research Update** is distinctive to this journal — useful when
> a project has a significant but not full-length increment. Fetch the official
> definition before recommending it.

## 11. Positioning advice `[HEURISTIC]`

- Title and abstract should name the material/material class and the functional
  or structural advance.
- Report characterization completely — structure, composition, purity,
  reproducibility of synthesis.
- For computational materials work, validate against experiment where possible
  and state the accuracy of the level of theory.
- For discovery pipelines, close the loop: at least one validated candidate.
- Say who can use this result and for what.

## 12. Submission checklist

- [ ] Materials-centric central claim
- [ ] Correct journal vs. PRB / PRApplied / PRX Intelligence
- [ ] Article type chosen (Article / Letter / Research Update / Review)
- [ ] Section selected from PRMaterials guidelines
- [ ] Characterization and synthesis details complete and reproducible
- [ ] Validation of computational predictions addressed
- [ ] Prior materials literature compared (including non-physics venues)
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Materials-centric test. 3. Novelty type.
4. Characterization completeness. 5. Community relevance. 6. Validation.
7. Neighbor comparison (PRB first). 8. Vulnerabilities. 9. Fit class,
positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Materials vs. mechanism:** why PRMaterials rather than PRB.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRMaterials-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Moderate. Materials research is
often carried by synthesis, structure, and characterization; the mathematics
supports rather than constitutes the claim.

**Expected equation density:** Low to moderate — higher for modeling and
prediction papers, low for growth and characterization studies.

**Role of equations:** To define computed quantities, structure–property
relations, and thermodynamic or kinetic models precisely enough to be reused and
compared across materials.

**Main-text mathematical content:** Definitions of computed descriptors and
figures of merit; the thermodynamic or kinetic model where one is used; the
level of theory and its parameters; any structure–property relation claimed.

**Supplementary mathematical content:** Derivations, full computational
parameters, convergence tests, extended property tables.

**Recommended derivation depth:** Low to moderate — state models and cite
standard derivations rather than reproducing them.

**Figure–equation integration:** Phase diagrams and property trends should name
the model and parameters behind them; a computed quantity plotted across a
materials family should be defined once, unambiguously.

**Recommended presentation strategy:** `[HEURISTIC]` Do not add formalism to
raise apparent rigor — in this journal it displaces the characterization detail
readers actually need. Conversely, a structure–property claim asserted only in
prose is weaker than one written as a relation and tested across the family.

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
| **Research Updates** | **10,000 words** |
| Review Articles | **30,000 words** |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Full-length by default, with an unusually rich type menu.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Low to Moderate.

**Recommended main-text figure strategy:** `[CONVENTION]` Materials papers are
figure-heavy by nature — structure, characterization, property trends — and this
is appropriate here. `[STRATEGY]` Ensure each characterization figure supports a
claim; a panel included because the measurement was taken is padding.

**Supplementary-material role:** Full characterization datasets, synthesis
protocols in detail, extended property tables, additional compositions.

**Preferred narrative style:** Detailed exposition, with complete synthesis and
characterization detail — the readership needs to reproduce the material.

**Recommended manuscript compactness:** Low to Moderate.

**Presentation priority:** Reproducibility of the material itself.

> `[STRATEGY]` **Research Update** (10,000 words) is distinctive to this journal
> and under-used: it suits a significant increment that does not warrant a full
> Regular Article. Fetch the official definition before recommending it.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Materials | https://journals.aps.org/prmaterials/about | Official | 2026-08-19 | Identity, scope, criteria, article types |
| PRMaterials section selection | https://journals.aps.org/prmaterials/authors/guidelines-section-selection-physical-review-materials | Official | 2026-08-19 | Sections (fetch) |
| PRMaterials editorial policies and practices | https://journals.aps.org/prmaterials/authors/editorial-policies-practices | Official | 2026-08-19 | Article-type definitions (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prmaterials/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
