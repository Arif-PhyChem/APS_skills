---
name: aps-prfluids
description: Evaluate a manuscript's fit for Physical Review Fluids — all aspects of fluid dynamics research.
journal: Physical Review Fluids
abbreviation: PRFluids
journal_code: prfluids
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

# Physical Review Fluids — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for nearly every submission** — governing equations, boundary conditions, and dimensionless groups are the problem statement. See §Mathematical presentation profile below for this journal's
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

PRFluids is "a trusted journal for high-quality, significant developments in
fluid dynamics," welcoming "both traditional and novel research topics,
including bio-related fluid dynamics, micro and nanoscale flows, fluid mechanics
of complex fluids and soft materials, and geophysical and environmental flows."

It is strongly supported by the APS **Division of Fluid Dynamics (DFD)**, hosts
the **François Frenkiel Award** for a young investigator, and publishes invited
papers from the annual DFD meeting and winning entries from the **Gallery of
Fluid Motion**. It interacts closely with the DFD board to expand scope into
emerging areas.

## 2. Scope `[OFFICIAL]`

All aspects of fluid dynamics, including: biological and biomedical flows;
combustion fluid mechanics and reacting flows; complex and non-Newtonian fluids;
compressible and rarefied flows, kinetic theory; convection; drops, bubbles,
capsules and vesicles; electrokinetic phenomena, electrohydrodynamics, and
magnetohydrodynamics; geophysical, geological, urban and ecological flows;
instability, transition, and control; interfacial phenomena and flows; laminar
and viscous flows; micro- and nanofluidics; multiphase, granular, and
particle-laden flows; nonlinear dynamical systems; transport and mixing;
turbulent flows; vortex dynamics; wave dynamics, free surface flows, stratified
and rotating flows; and **Methods for New Experiments, Algorithms, and Theory
(NEAT)**.

> `[HEURISTIC]` **NEAT** is a distinctive, explicitly methodological section.
> Route method-centric fluids work there rather than forcing it into a physics
> narrative.

## 3. Acceptance criteria `[OFFICIAL]`

Submitted manuscripts should:

- Add to the existing knowledge related to flow physics that contributes to
  - the fundamental understanding of the subject; **and/or**
  - presents a new methodology, **and its validation**, that demonstrates potential for substantial discovery in fluid dynamics.
- Represent an authoritative and substantive addition to the body of literature.

> `[INFERENCE]` PRFluids is unusual in the portfolio: it names methodology as a
> first-class contribution route — but binds it to **validation** and to
> **demonstrated discovery potential**. A new solver without validation fails
> the criterion as written.

## 4. Editorial positioning `[INFERENCE]`

Flow physics for the fluids community. Two legitimate entry routes: fundamental
understanding, or validated methodology. Choose one and argue it directly.

## 5. Strong-fit profile `[INFERENCE]`

- New flow phenomena or instability mechanisms with clear physical explanation.
- Turbulence results with well-resolved statistics and scaling arguments.
- Complex/non-Newtonian fluid mechanics linking rheology to flow behavior.
- Validated numerical or experimental methodology enabling new measurements.
- Bio-, geo-, or micro-scale flows treated as fluid dynamics.

## 6. Weak-fit patterns `[HEURISTIC]`

- CFD parameter studies of a configuration with no flow-physics insight.
- New solver claims without validation against benchmarks.
- Engineering performance studies (→ an engineering venue or PRApplied).
- Soft-matter results where the fluid is incidental (→ PRE).
- ML surrogates for flows with no validation or physical interpretation
  (→ strengthen validation, or PRX Intelligence).

## 7. Evaluation framework

**A. Scope fit** · **B. Route** (understanding vs. validated methodology) ·
**C. Novelty** · **D. Resolution/convergence and experimental uncertainty** ·
**E. Validation against benchmarks** · **F. Generality** ·
**G. Positioning vs. PRE / PRApplied / PRL / PRX Intelligence.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Significant flow-physics understanding, or a validated method with demonstrated discovery potential; rigorous |
| **Strong** | Clearly in scope; solid contribution on one route |
| **Moderate** | In scope; resolution, validation, or physical interpretation incomplete |
| **Borderline** | Better served by PRE's general framing or PRApplied's device framing |
| **Poor** | Configuration study or unvalidated method |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRE** | The result is a general statistical/nonlinear/soft-matter principle rather than flow physics for the fluids community |
| **PRApplied** | The claim is a device or application (e.g. a microfluidic technology) |
| **PRL / PRX** | Pivotal or field-defining fluid-dynamics advance |
| **PRX Life** | The work is quantitative biology where flow is one ingredient |
| **PRX Intelligence** | The AI/ML method is the central, exceptional contribution |
| **PRResearch** | Solid in-scope work where gold OA is wanted |

Prefer **PRFluids** when: the audience is the fluid-dynamics community and the
claim is about flow physics or validated fluids methodology.

## 10. Article types `[OFFICIAL]`

Detailed **research articles** and **Letters** (short papers of particular
importance). Flexible lengths; longer papers welcome. Invited DFD-meeting papers
and Gallery of Fluid Motion entries are also published. Limits: `/prfluids/authors#article`.

## 11. Positioning advice `[HEURISTIC]`

- Declare the route (understanding or methodology) in the abstract.
- For methodology, lead with the validation and the discovery it enables.
- Report resolution, convergence, Reynolds/Weber/other governing parameters, and
  experimental uncertainty explicitly.
- Compare against canonical benchmarks the fluids community recognizes.
- State the regime of validity.

## 12. Submission checklist

- [ ] Route declared and argued
- [ ] Validation against recognized benchmarks
- [ ] Resolution/convergence and uncertainty reported
- [ ] Governing dimensionless parameters stated
- [ ] Correct section (consider NEAT for methods work)
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Route selection. 3. Scope fit. 4. Novelty.
5. Validation and resolution. 6. Generality. 7. Neighbor comparison.
8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Criterion route:** fundamental understanding / validated methodology — with justification.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRFluids-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High. Governing equations, boundary
conditions, and dimensionless groups are the field's shared language and are
expected to be stated.

**Expected equation density:** Moderate to high — high for stability analysis
and theory; moderate for experimental and computational studies, which still
need the governing system and nondimensionalization.

**Role of equations:** To define the problem unambiguously. In fluid dynamics
the governing equations plus boundary conditions plus dimensionless parameters
*are* the problem statement; without them a result cannot be compared to
anything.

**Main-text mathematical content:** The governing equations and boundary
conditions; the nondimensionalization and the resulting dimensionless groups
with their values; the stability or asymptotic analysis where central; the
closure or subgrid model for turbulence work.

**Supplementary mathematical content:** Full derivations, perturbation series,
discretization and numerical-scheme detail, convergence and resolution studies.

**Recommended derivation depth:** Moderate to full for analysis papers; state
and cite for standard formulations.

**Figure–equation integration:** Scaling collapses and stability boundaries must
have their scaling forms and criteria written down; the regime of every figure
should be identifiable from its dimensionless parameters.

**Recommended presentation strategy:** `[HEURISTIC]` State the governing system,
the boundary conditions, and every dimensionless group early and completely —
this is the single most common completeness gap in fluids submissions. For the
methodology route through PRFluids' acceptance criteria, the mathematical
specification of the method and its validation is the contribution.

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
| **Gallery of Fluid Motion** | no length limit |
| Invited Papers | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Full-length by default, with distinctive visual and invited
types.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate to High.

**Recommended main-text figure strategy:** `[CONVENTION]` Fluids is a strongly
visual field; flow visualizations, phase maps, and collapses carry arguments
here. `[STRATEGY]` Every figure should be identifiable by its dimensionless
parameters — a figure whose regime the reader cannot place proves little.
Videos and time-resolved data belong in Supplemental Material.

**Supplementary-material role:** Videos, extended parameter sweeps, resolution
and convergence studies, full numerical-scheme detail.

**Preferred narrative style:** Detailed exposition; governing equations,
boundary conditions, and nondimensionalization stated completely and early.

**Recommended manuscript compactness:** Low to Moderate.

**Presentation priority:** Problem specification. `[STRATEGY]` Incomplete
specification of the governing system and dimensionless groups is the most
common completeness gap in fluids submissions.

> **Gallery of Fluid Motion** entries are a genuinely different presentation
> mode — image- and video-led. Fetch the current requirements before advising.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Fluids | https://journals.aps.org/prfluids/about | Official | 2026-08-19 | Identity, scope (incl. NEAT), criteria, article types, DFD relationship |
| PRFluids Information for Authors | https://journals.aps.org/prfluids/authors | Official | 2026-08-19 | Article types, limits (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prfluids/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
