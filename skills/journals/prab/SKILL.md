---
name: aps-prab
description: Evaluate a manuscript's fit for Physical Review Accelerators and Beams — accelerator science, technology, and applications. Fully open access at no cost to authors.
journal: Physical Review Accelerators and Beams
abbreviation: PRAB
journal_code: prab
publisher: American Physical Society
access_model: gold open access, sponsor-funded (no author charge)
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# Physical Review Accelerators and Beams — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for beam-dynamics and theory submissions**; it matters less for hardware and facility-description papers. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

PRAB is "a trusted open access journal for high-quality, significant
developments in accelerator science, technology, and applications." It is
"sponsored by more than 40 research institutions and companies around the world,
enabling open access publishing to all authors at zero cost" — funded by
laboratories, universities, and industrial sponsors, and provided without charge
to both authors and readers.

The APS **Division of Physics of Beams** and the **European Physical Society
Accelerators Group** share responsibility for the journal.

> `[HEURISTIC]` Zero-cost gold OA is a real practical advantage worth surfacing
> to authors comparing venues, but it is never a fit argument on its own.

## 2. Scope `[OFFICIAL]`

All topics in accelerator science, applications, and technology, including:
low- and intermediate-energy accelerators; pulsed-power accelerators; synchrotron
radiation and free-electron lasers; high-energy accelerators and colliders; new
acceleration techniques; accelerator facilities and design studies; radio
frequency calculations and technology; magnet calculations and technology; beam
control, diagnostics, and feedback; particle and radiation detectors; targets,
collimators, and beam dumps; accelerator materials and surfaces; cryogenics and
vacuum technology; particle-beam sources; single-particle dynamics; low-energy
multiple-particle dynamics; relativistic multiple-particle dynamics;
material–beam interaction; and **computers, machine learning, and algorithms**.

Section-selection guidelines:
`/prab/authors/guidelines-section-selection-physical-review-accelerators-beams`.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to accelerator science, technology, and applications.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRAB's readers.
- Represent an authoritative and substantive addition to the body of literature.
- **Review articles should present the current status of a research field in a form comprehensible and useful to both practitioners and people entering the field.**

## 4. Editorial positioning `[INFERENCE]`

The archival venue for accelerator and beam physics, spanning fundamental beam
dynamics through hardware technology and facility design. Practitioner utility
matters: results that other accelerator groups can apply carry weight.

## 5. Strong-fit profile `[INFERENCE]`

- Beam-dynamics theory or simulation validated against machine measurements.
- Novel acceleration or beam-manipulation techniques with demonstrated performance.
- Technology advances — RF, magnets, cryogenics, vacuum, sources, diagnostics —
  with characterization.
- Facility design studies with complete parameter analysis.
- Machine-learning applications to accelerator control or optimization with
  validation on real machines.
- Reviews that orient both practitioners and newcomers.

## 6. Weak-fit patterns `[HEURISTIC]`

- Simulation studies with no validation and no machine relevance.
- Component descriptions with no performance characterization.
- Incremental design variants without an analysis of consequence.
- ML control schemes tested only in simulation with no baseline controller.
- Particle-physics results where the accelerator is incidental (→ PRD).

## 7. Evaluation framework

**A. Scope fit** · **B. Practitioner utility** · **C. Novelty type** (dynamics /
technique / technology / design / algorithm) · **D. Validation against
measurement** · **E. Completeness of parameters** · **F. Reproducibility** ·
**G. Positioning vs. PRD / PRC / PRApplied / PRE / PRX Intelligence.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Significant, validated accelerator/beam advance with clear practitioner value |
| **Strong** | Clearly in scope; solid contribution |
| **Moderate** | In scope; validation or parameter completeness needs work |
| **Borderline** | Physics result where the accelerator is incidental, or an application better placed elsewhere |
| **Poor** | Unvalidated simulation or undocumented component report |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRD** | The physics result — particle physics, cosmology — is the point |
| **PRC** | The core is nuclear physics |
| **PRApplied** | The claim is a device or application outside accelerator science |
| **PRE** | The core is general beam/plasma statistical or nonlinear dynamics |
| **PRX Intelligence** | The central contribution is an exceptional AI/ML method |
| **PRL / PRX** | Pivotal or field-defining advance |

Prefer **PRAB** when: the contribution is accelerator or beam science,
technology, or applications for that community.

## 10. Article types `[OFFICIAL]`

Detailed **research articles**, **review articles**, and **Letters** (short,
accessible papers of particular importance). Flexible lengths; longer papers
welcome. Reviews carry the additional criterion in §3.

## 11. Positioning advice `[HEURISTIC]`

- Give complete machine and beam parameters; other groups need to reproduce.
- Validate simulation against measured data wherever a machine exists.
- For control/ML work, compare against the operational baseline controller.
- State applicability across machine classes.
- For reviews, address both practitioners and newcomers explicitly, as the
  criterion requires.

## 12. Submission checklist

- [ ] Accelerator/beam central claim
- [ ] Article type chosen (Article / Letter / Review)
- [ ] Section selected from PRAB guidelines
- [ ] Machine and beam parameters complete
- [ ] Validation against measurement where possible
- [ ] Baselines for control/optimization work
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Scope fit. 3. Novelty type. 4. Practitioner utility.
5. Validation. 6. Completeness. 7. Neighbor comparison. 8. Vulnerabilities.
9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Practitioner utility:** who can apply this, and how.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRAB-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High for beam dynamics and theory;
moderate for technology and facility-design papers.

**Expected equation density:** Moderate to high — single- and multi-particle
dynamics work is equation-driven; hardware and diagnostics papers are less so.

**Role of equations:** To define the beam dynamics, the lattice, and the
figures of merit precisely enough that another group can reproduce the result on
a different machine.

**Main-text mathematical content:** The equations of motion or map; the lattice
and optics functions; emittance, luminosity, impedance, or wakefield definitions
as relevant; the scaling of performance with machine parameters.

**Supplementary mathematical content:** Long derivations, full lattice files and
parameter tables, tracking-code configuration, convergence studies.

**Recommended derivation depth:** Moderate — state the formalism and derive what
is specific to this machine or regime.

**Figure–equation integration:** Simulation results should be traceable to the
model and parameter set; measured-versus-predicted comparisons should show the
predictive expression.

**Recommended presentation strategy:** `[HEURISTIC]` Give complete machine and
beam parameters alongside the formalism — PRAB's practitioner readership
reproduces and adapts results, and a formalism without its parameters is not
reusable. For control and optimization work, state the objective function
mathematically and name the baseline controller it is compared against.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Letters | **4500 words** |
| Research Articles | **no length limit** |
| Review Articles | **no length limit** |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Full-length by default; reviews uncapped.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate to High.

**Recommended main-text figure strategy:** `[STRATEGY]` Lattice plots, tracking
results, and measured-vs-predicted comparisons carry the argument. Keep the
comparison figures in the main text and move parameter scans to Supplemental
Material.

**Supplementary-material role:** Full lattice files, parameter tables, tracking
configurations, extended scans.

**Preferred narrative style:** Detailed exposition aimed at practitioners who
will adapt the result to their own machine.

**Recommended manuscript compactness:** Low to Moderate.

**Presentation priority:** Reusability. `[STRATEGY]` Complete machine and beam
parameters are what make a PRAB paper useful; a formalism without its parameters
cannot be applied elsewhere. `[REQUIREMENT]` Review Articles must present the
field's current status usefully for both practitioners and newcomers.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Accelerators and Beams | https://journals.aps.org/prab/about | Official | 2026-08-19 | Identity, sponsorship model, scope, criteria, article types |
| PRAB section selection | https://journals.aps.org/prab/authors/guidelines-section-selection-physical-review-accelerators-beams | Official | 2026-08-19 | Sections (fetch) |
| PRAB sponsors | https://journals.aps.org/prab/sponsors | Official | 2026-08-19 | Zero-cost OA model |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prab/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
