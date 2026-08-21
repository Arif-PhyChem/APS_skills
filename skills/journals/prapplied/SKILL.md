---
name: aps-prapplied
description: Evaluate a manuscript's fit for Physical Review Applied — applied physics at the interfaces with engineering, materials science, chemistry, biology, and medicine.
journal: Physical Review Applied
abbreviation: PRApplied
journal_code: prapplied
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

# Physical Review Applied — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` when the manuscript needs to establish a mechanism** — which is the journal's stated criterion, and usually the difference between a PRApplied paper and an engineering report. See §Mathematical presentation profile below for this journal's
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

PRApplied is "a trusted and multidisciplinary journal for high-quality,
significant developments in applied science," publishing "work at the interfaces
of physics with engineering, materials science, chemistry, biology, and
medicine." It aims to be "a welcoming hub for work from diverse communities in
physics and beyond."

## 2. Scope `[OFFICIAL]`

- Biophysics, bioelectronics, and biomedical engineering
- Device physics
- Electronics
- Technology to harvest, store, and transmit energy, focusing on renewable energy
- Magnetism and spintronics
- Metamaterials
- Microfluidics
- Nanoscience and nanotechnology
- Optics, optoelectronics, photonics, and photonic devices
- Quantum information science and technology

## 3. Acceptance criteria `[OFFICIAL]`

- **Present fresh insight into applications-based physical phenomena.**
- Make a high-quality, significant contribution in a specific research area and generate interest for PRApplied's readers.
- Represent an authoritative and substantive addition to the body of literature.

> `[HEURISTIC]` The first criterion is the discriminator and it is easy to
> misread. PRApplied asks for **insight into applications-based physical
> phenomena** — not merely a better device number. A performance record with no
> physical understanding of why satisfies the engineering reading of the
> criterion but not the stated one.

## 4. Editorial positioning `[INFERENCE]`

PRApplied sits between physics and engineering and demands both: an application
context *and* physical insight. Work that is pure engineering optimization
belongs in an engineering venue; work with no application framing belongs in a
core *Physical Review* journal.

## 5. Strong-fit profile `[INFERENCE]`

- A device or application result explained by identified physical mechanisms.
- Physical limits, loss channels, or noise mechanisms of a technology characterized.
- New device concepts grounded in physics with demonstrated function.
- Measurement or fabrication techniques that unlock applied capabilities.
- Cross-disciplinary work where the physics explains the applied behavior.

## 6. Weak-fit patterns `[HEURISTIC]`

- Incremental performance improvement with no mechanism.
- Parameter-sweep optimization studies.
- Simulation-only device studies with no validation or physical analysis.
- Core condensed-matter physics with an application sentence bolted on (→ PRB).
- Materials-first work aimed at the materials community (→ PRMaterials).
- Energy-technology work at an exceptional tier (→ PRX Energy).

## 7. Evaluation framework

**A. Application context** · **B. Physical insight** (the gate) ·
**C. Novelty type** (concept / mechanism / technique / performance) ·
**D. Demonstration and validation** · **E. Community relevance** ·
**F. Reproducibility of fabrication/measurement** ·
**G. Positioning vs. PRB / PRMaterials / PRX Quantum / PRX Energy / PRL.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Applications-relevant result with genuine, demonstrated physical insight |
| **Strong** | Clearly in scope; solid applied contribution with mechanism |
| **Moderate** | In scope; physical insight underdeveloped relative to the engineering result |
| **Borderline** | Really a physics paper (PRB), materials paper (PRMaterials), or an engineering paper |
| **Poor** | Performance optimization only; no physical insight |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRB** | The claim is the condensed-matter physics, not the application |
| **PRMaterials** | The claim is about the material |
| **PRX Quantum** | Quantum technology work meeting an "exceptional" criterion |
| **PRX Energy** | Energy research/technology at a highly selective tier |
| **PRA** | The core is AMO/quantum-optics physics |
| **PRFluids** | Microfluidics treated as fluid dynamics |
| **PRX Life** | Biomedical work framed as quantitative life science |
| **PRL / PRX** | Pivotal or field-defining applied advance |
| **PRX Intelligence** | The central contribution is an AI/ML method |

Prefer **PRApplied** when: an application is the frame *and* the paper explains
the physics behind it.

## 10. Article types `[OFFICIAL]`

PRApplied publishes traditional **Research Articles**; short **Letters** of
particular significance or topical interest; **Review Articles** surveying the
literature; and **Perspectives**, offering opinion and direction at the cutting
edge. The Letters section is "intended for accelerated publication of important
new results, at approximately the level of *Physical Review Letters*," and
Letters are given priority in editorial processing and production.

> `[HEURISTIC]` That PRL-level statement is a real bar, not marketing. Route a
> routine result to a Research Article rather than a Letter.

`[OFFICIAL]` Verified limits (2026-08-19): Regular Articles — no length limit;
Letters — 4500 words; Review Articles — 30,000 words; Perspectives — no length
limit; Comments/Replies — 3500 words.

## 11. Positioning advice `[HEURISTIC]`

- Open with the applied problem and the physical question it raises.
- Devote a section to mechanism: why does the device behave this way?
- Benchmark against the state of the art honestly, including commercial baselines.
- Report fabrication and measurement details sufficient for replication.
- State limits — scaling, stability, cost, manufacturability — plainly.

## 12. Submission checklist

- [ ] Applications-based framing with explicit physical insight
- [ ] Article type chosen (Article / Letter / Review / Perspective)
- [ ] Benchmark against state of the art
- [ ] Fabrication/measurement reproducibility details
- [ ] Limits and failure modes stated
- [ ] Alternatives (PRB, PRMaterials, PRX Quantum, PRX Energy) considered
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Application framing. 3. Physical-insight gate.
4. Novelty type. 5. Validation/benchmarking. 6. Neighbor comparison.
7. Vulnerabilities. 8. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Physical insight:** what mechanism is established (gate check).

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRApplied-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Moderate — but strategically
important, because PRApplied's stated criterion asks for **insight into
applications-based physical phenomena**, and a mechanism is most convincingly
expressed as a model.

**Expected equation density:** Low to moderate; higher for device-physics and
noise-analysis work.

**Role of equations:** To turn a performance result into a physical
explanation. The model that predicts the device's behavior, the loss or noise
budget, and the scaling of performance with a physical parameter are what
distinguish a PRApplied paper from an engineering report.

**Main-text mathematical content:** The device or transport model; the loss,
noise, or efficiency budget; the scaling relation for performance; definitions
of the reported figures of merit.

**Supplementary mathematical content:** Derivations, full simulation parameters,
fabrication-tolerance analysis, calibration procedures.

**Recommended derivation depth:** Low to moderate — state and validate the
model; derive only what is not standard.

**Figure–equation integration:** Performance data should be accompanied by the
model curve, with deviations discussed physically rather than fitted away.

**Recommended presentation strategy:** `[HEURISTIC]` The highest-leverage
addition to a borderline PRApplied manuscript is usually a mathematical model
that explains *why* the device performs as it does and predicts how the
performance scales. That converts a metric into the physical insight the
criterion asks for.

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
| Review Articles | **30,000 words** |
| Perspectives | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Full-length by default; Letters intended for accelerated
publication of important results.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Low to Moderate.

**Recommended main-text figure strategy:** `[STRATEGY]` Device papers accumulate
characterization figures; keep in the main text those that establish the
*mechanism* and the benchmark comparison, and move process-development series to
Supplemental Material. A performance plot without a model curve is a weaker
figure than one with it.

**Supplementary-material role:** Fabrication detail, calibration, tolerance
analysis, additional devices, full measurement series.

**Preferred narrative style:** Applied framing with physical explanation —
engineering results carried by physics reasoning.

**Recommended manuscript compactness:** Moderate.

**Presentation priority:** The mechanism. `[STRATEGY]` The journal's stated
criterion asks for insight into applications-based physical phenomena; the
manuscript's structure should make that insight prominent rather than burying it
after the performance results.

> `[OFFICIAL]` PRApplied states its Letters section is for accelerated
> publication of important new results "at approximately the level of *Physical
> Review Letters*", with priority processing.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Applied | https://journals.aps.org/prapplied/about | Official | 2026-08-19 | Identity, scope, criteria, article types |
| PRApplied Information for Authors | https://journals.aps.org/prapplied/authors | Official | 2026-08-19 | Requirements, limits (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prapplied/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
