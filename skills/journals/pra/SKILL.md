---
name: aps-pra
description: Evaluate a manuscript's fit for Physical Review A — atomic, molecular, and optical physics, foundations of quantum mechanics, and quantum science.
journal: Physical Review A
abbreviation: PRA
journal_code: pra
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

# Physical Review A — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for essentially every submission here** — Hamiltonians, master equations, and protocol definitions are AMO and quantum science's working vocabulary. See §Mathematical presentation profile below for this journal's
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

PRA is "a trusted journal for high-quality, significant developments in atomic,
molecular, and optical physics and quantum science." Established in 1970, it is
"the journal of choice for the publication of research in AMO physics and
quantum science," bridging traditional and recent research areas so that authors
and readers "benefit from the widespread synergies between these fields."

## 2. Scope `[OFFICIAL]`

- Fundamental concepts
- Quantum information science
- Quantum technologies
- Atomic and molecular structure and dynamics; high-precision experiments; chemical physics
- Light-induced processes in atomic-scale systems
- Ultracold systems and matter waves
- Photonics, nonlinear optics, and optomechanics
- Quantum optics

Section-selection guidelines: `/pra/authors/guidelines-section-selection-physical-review-a`.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to atomic, molecular, and optical physics and quantum science.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRA's readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

PRA is the **archival specialist venue** for AMO and quantum science:
significance within a research area, authority, and completeness — not breadth
or paradigm shift. Its defining tension is with PRX Quantum: PRA carries the
full range of solid quantum-science work; PRX Quantum takes the exceptional
subset.

## 5. Strong-fit profile `[INFERENCE]`

- New AMO phenomena, precision measurements, or spectroscopic determinations.
- Theoretical frameworks for atomic/molecular structure, dynamics, or quantum optics.
- Quantum-information theory and protocols with rigorous analysis.
- Ultracold-atom and matter-wave results with careful characterization.
- Photonics/optomechanics results where the physics, not the device, is the claim.
- Thorough, definitive treatments that will be cited as references.

## 6. Weak-fit patterns `[HEURISTIC]`

- Incremental variations of standard quantum protocols with no new capability or insight.
- Numerical studies of a model with no physical interpretation or benchmark.
- Device- or platform-engineering results (→ PRApplied).
- Condensed-matter systems framed as quantum optics (→ PRB).
- Claims of quantum advantage without complete error and baseline analysis.

## 7. Evaluation framework

**A. Scope fit** (AMO/quantum science?) · **B. Significance within area** ·
**C. Novelty type** · **D. Theory/experiment rigor** · **E. Completeness and
authority** · **F. Evidence** · **G. Positioning vs. PRX Quantum / PRL / PRB /
PRApplied / PRE.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Central AMO/quantum-science topic; significant, complete, authoritative |
| **Strong** | Clearly in scope; solid meaningful advance |
| **Moderate** | In scope; needs stronger interpretation, validation, or completeness |
| **Borderline** | Overlaps PRA but PRX Quantum, PRB, or PRApplied is a more natural home |
| **Poor** | Outside AMO/quantum science, or contribution is a device/implementation result |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRX Quantum** | The work is *exceptional* in advance, connection, capabilities, or insight within quantum science and technology |
| **PRL** | The advance is pivotal and of broad interest across physics |
| **PRB** | The system is condensed matter — solids, correlated electrons, materials |
| **PRApplied** | The claim is about a device, sensor, or application |
| **PRE** | The core is statistical physics, nonlinear dynamics, or complex systems |
| **PRD** | The topic is gravitation, cosmology, or particle physics (including precision tests framed there) |
| **PRX Intelligence** | The central contribution is an AI/ML method |
| **PRResearch** | Solid in-scope work where gold OA is wanted |

Prefer **PRA** when: the contribution is a significant, complete AMO or
quantum-science result for that specialist readership.

## 10. Article types `[OFFICIAL]`

Detailed **research articles** and **Letters** (short papers of particular
importance). Flexible lengths; longer papers welcome. Limits: `/pra/authors#article`.

## 11. Positioning advice `[HEURISTIC]`

- State the AMO/quantum-science question in the first two sentences.
- For quantum-information work, be explicit about assumptions, resource counts,
  and what is proven vs. numerically observed.
- For experiments, report systematics and uncertainty budgets fully.
- Compare against the standard methods and competing platforms.
- If the work is exceptional, say why in the cover letter and consider PRX Quantum.

## 12. Submission checklist

- [ ] AMO/quantum-science central claim
- [ ] PRX Quantum considered and reason for PRA stated
- [ ] Article type and section selected
- [ ] Uncertainty/systematics or proof assumptions complete
- [ ] Prior work and competing platforms compared
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Domain test. 3. Novelty type. 4. Significance in
area. 5. Rigor and completeness. 6. Neighbor comparison (PRX Quantum first).
7. Vulnerabilities. 8. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Why PRA rather than PRX Quantum:** …

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRA-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High to Very High. Much of AMO and
quantum science is formulated mathematically by default — Hamiltonians, master
equations, density matrices, response and correlation functions, and protocol
definitions are the working vocabulary.

**Expected equation density:** High for theory; moderate for experimental
papers, which still typically need the model connecting observables to
parameters.

**Role of equations:** To define the system and the protocol unambiguously. In
quantum information especially, the equation *is* the specification: assumptions,
resource counts, and error models must be stated formally to be checkable.

**Main-text mathematical content:** The Hamiltonian or master equation; the
state and measurement definitions; the principal analytical result; the
approximation regime (rotating-wave, Markovian, weak-coupling) with its
condition of validity.

**Supplementary mathematical content:** Full derivations, perturbative orders,
numerical convergence, auxiliary bounds and proofs.

**Recommended derivation depth:** Moderate to full — PRA's flexible length
supports complete treatments, and the readership expects them.

**Figure–equation integration:** Plot quantities that are mathematically
defined; state which equation each panel tests.

**Recommended presentation strategy:** State assumptions formally and early.
`[HEURISTIC]` For protocol and advantage claims, separate what is **proven**
from what is **numerically observed** — conflating them is a standard referee
objection in this field.

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

**Typical mathematical density:** High to Very High (see §Mathematical presentation profile).

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
content. PRA's own guidance is that the appropriate length depends on the
information the article contains.

**Presentation priority:** Formal precision — assumptions, protocols, and uncertainty budgets stated explicitly.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review A | https://journals.aps.org/pra/about | Official | 2026-08-19 | Identity, scope, criteria, article types |
| PRA section selection | https://journals.aps.org/pra/authors/guidelines-section-selection-physical-review-a | Official | 2026-08-19 | Sections (fetch) |
| PRA Information for Authors | https://journals.aps.org/pra/authors | Official | 2026-08-19 | Article types, limits (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/pra/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
