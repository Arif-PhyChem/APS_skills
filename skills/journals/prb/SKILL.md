---
name: aps-prb
description: Evaluate a manuscript's fit for Physical Review B (condensed matter and materials physics), compare it against neighboring APS journals, and advise on positioning.
journal: Physical Review B
abbreviation: PRB
journal_code: prb
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

# Physical Review B — Journal Skill

Load `aps-common` alongside this skill. Claims are tagged `[OFFICIAL]`
(stated by APS), `[INFERENCE]` (editorial reading of official text), or
`[HEURISTIC]` (agent decision rule, not APS policy).

**Load `aps-mathematical-presentation` for any theoretical or computational submission** — that is most of PRB. Skip it only for purely experimental characterization work. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

**Load `aps-reference-format` whenever building, reviewing, or auditing the
reference list** — numbering and citation mechanics apply portfolio-wide; check
this journal's own skill only for a journal-specific addition (PRL's
titles-in-references convention is the only one on record).

## 1. Purpose

Decide whether a manuscript's central contribution belongs in PRB, why PRB
rather than a neighbor, and what would have to change for it to be well
positioned.

## 2. Identity `[OFFICIAL]`

PRB is APS's journal for condensed matter and materials physics, published
since 1970. It describes itself as a trusted venue for "high-quality,
significant developments in condensed matter and materials physics," reaching a
wide audience and emphasizing "a rigorous, fair, and constructive review process
to present results that stand the test of time." It is the portfolio's
high-volume specialist venue for the field: authoritative rather than
headline-seeking, archival rather than breaking.

Readership: condensed-matter and materials physicists — theorists,
experimentalists, and computational researchers.

## 3. Scope `[OFFICIAL]`

PRB covers the full range of condensed matter, materials physics, and related
subfields, including:

**Core areas**
- Structure and phase transitions
- Ferroelectrics and multiferroics
- Disordered systems and alloys
- Magnetism
- Superconductivity
- Electronic structure, photonics, and metamaterials
- Semiconductors and mesoscopic systems
- Surfaces, nanoscience, and two-dimensional materials
- Topological states of matter

The authoritative section list is the section-selection guideline page
(`/prb/authors/guidelines-section-selection-physical-review-b`); fetch it when
the correct section matters for a submission.

**Interdisciplinary/emerging** `[INFERENCE]` — computational, data-driven, and
AI/ML work is in scope when the delivered result is a condensed-matter or
materials-physics result. The method is the vehicle; the physics is the cargo.

## 4. Scope boundaries

| Verdict | Pattern |
|---|---|
| Clearly in scope | The central claim is about the physical properties, structure, excitations, or phases of condensed matter |
| Possibly in scope `[INFERENCE]` | Method-led work that nonetheless delivers a specific condensed-matter result |
| Generally out of scope `[INFERENCE]` | The central contribution is an ML architecture, a code release, a device engineering result, a chemistry synthesis result, or a materials-screening exercise with no physical interpretation |

> `[HEURISTIC]` Containing a material is not sufficient. Ask: strip the material
> away and state the claim — is what remains a statement about condensed-matter
> physics, or about a method, a device, or a workflow?

## 5. Editorial criteria `[OFFICIAL]`

Submitted manuscripts should meet the following criteria:

- Add to the existing knowledge related to condensed matter and materials physics.
- Make a high-quality, significant contribution in a specific research area and generate interest for PRB's readers.
- Represent an authoritative and substantive addition to the body of literature.

`[INFERENCE]` Note what this bar does *not* require: breadth beyond the
subfield, or a paradigm shift. "Significant within a specific research area" is
the operative standard. PRB's distinguishing demand is **authority and
substance** — completeness, rigor, and durability — not novelty theater.

## 6. Editorial positioning `[INFERENCE]`

| Dimension | PRB's demand |
|---|---|
| Novelty | Real but need not be transformative |
| Significance | Significant *within a specific research area* |
| Breadth | Specialist readership is acceptable and expected |
| Conceptual advance | Valued, not mandatory |
| Methodological advance | Counts when it yields physics |
| Evidence | High bar — "stand the test of time" implies convergence tests, error bars, controls |
| Completeness | High — the flexible length policy exists so papers can be thorough |

The animating question is not *is this exciting?* but:

> **Does this durably add to what is known about condensed matter, and is the
> evidence good enough that it will still be worth citing in ten years?**

## 7. Strong-fit profile `[INFERENCE]`

- Identifies a new physical mechanism in a condensed-matter system.
- Reveals previously unknown properties of a material or material class.
- Establishes a theoretical framework with concrete physical consequences.
- Provides convincing evidence for a new phase, excitation, or phenomenon.
- Resolves a standing theoretical or experimental disagreement.
- Delivers a thorough, definitive study of a system of established interest.
- Develops computational methodology that enables a new physical result — with
  the physical result actually presented.

## 8. Weak-fit patterns `[HEURISTIC]`

- Incremental parameter variation over an established calculation.
- Rich computation, thin physical interpretation ("we computed X for 40
  compounds" with no mechanism).
- Single-system result with no argument for wider relevance.
- Claims outrunning evidence (no convergence tests, no uncertainty, no baseline).
- Heavy ML methodology, marginal physics content → check PRX Intelligence.
- Device-performance framing → check PRApplied.
- Materials-discovery framing aimed at a materials-science readership → check
  PRMaterials.
- Missing comparison with established methods or prior literature.

## 9. Evaluation framework

Score each; none alone decides.

- **A. Scope fit** — Is the central question condensed-matter/materials physics?
- **B. Significance** — Does it matter within its research area?
- **C. Novelty** — Separate: new method / new material / new phenomenon / new mechanism / new interpretation. Name which.
- **D. Conceptual contribution** — New understanding, or new implementation?
- **E. Methodological contribution** — Does the method itself advance capability?
- **F. Breadth** — Who cites this? A subfield is enough for PRB.
- **G. Evidence** — Convergence, controls, error bars, reproducibility, baselines.
- **H. Positioning** — Why PRB rather than PRL, PRX, PRResearch, PRMaterials, PRApplied, PRX Intelligence?

## 10. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Central PRB topic; substantial, well-evidenced advance with clear physical significance; authoritative treatment |
| **Strong** | Clearly in scope; meaningful advance; evidence solid; significance specialized but real |
| **Moderate** | Subject appropriate; needs stronger physical interpretation, broader validation, or clearer framing before it reads as substantive |
| **Borderline** | Overlaps PRB but a neighbor offers a more natural readership; or physics content is thin relative to method content |
| **Poor** | Central contribution is outside condensed matter/materials physics, or is a method/device/workflow result wearing a materials costume |

## 11. Neighboring APS journals

| Journal | Prefer it when… | Prefer PRB when… |
|---|---|---|
| **PRL** | The result meets a PRL criterion — opens a new area/avenue, takes an essential step on a critical problem, introduces a highly impactful technique, or has unusual intrinsic interest to a broad physics audience — and survives as a short paper | The contribution needs full-length development, or its significance is real but confined to the subfield |
| **PRX** | Fundamental discovery, landmark in a fast-moving area, paradigm shift, or a high-impact community tool/database | The advance is significant but not field-defining |
| **PRResearch** | Sound, in-scope work where gold open access matters, or the topic sits between fields | The natural readership is specifically condensed matter |
| **PRMaterials** | The contribution is materials research — synthesis, growth, processing, design, materials discovery — aimed at the broader multidisciplinary materials community | The contribution is the underlying condensed-matter physics |
| **PRApplied** | The claim is about a device, application, or applications-based physical phenomenon | The claim is about the physics, not the application |
| **PRX Intelligence** | The central contribution is the AI/ML method, tool, dataset, or insight into AI/ML behavior | AI/ML is instrumentation and the claim is a physics claim |
| **PRA** | The system is atomic, molecular, optical, or quantum-science rather than condensed matter | The system is a solid/condensed phase |
| **PRE** | The core is statistical mechanics, nonlinear dynamics, soft matter, or complex systems in general form | The physics is specifically condensed-matter |

## 12. Article types `[OFFICIAL]`

- **Article** — full-length research paper. PRB states a flexible approach to
  article lengths and welcomes longer papers providing depth and authority.
- **Letter** — short, length-restricted paper of particular importance.

`[OFFICIAL]` Verified limits (2026-08-19): Regular Articles — **no length
limit**; Letters — **4500 words**; Perspectives — no length limit;
Comments/Replies — 3500 words. `[OFFICIAL]` Letters receive priority handling,
and authors should justify the need for the short format in the submission
letter; a Letter may be followed by a fuller account as a Regular Article.
Re-verify at `/prb/authors` before advising.

> A PRB Letter is *not* a *Physical Review Letters* paper. Do not conflate them
> in advice to authors.

## 13. AI/ML and computational manuscripts `[HEURISTIC]`

Answer these separately and in writing:

1. What is novel about the **method**?
2. What is novel about the **physics result**?
3. What physical insight did the method **enable** that was previously inaccessible?
4. How **general** is the method beyond the studied systems?
5. Would the physics result stand if obtained by conventional means?

Decision rule: if (2) and (3) are weak while (1) is strong, PRB is the wrong
venue — route to PRX Intelligence. If (2) and (3) are strong, PRB is a good
home even when (1) is modest. Architecture sophistication is not physical
significance; equally, the use of ML is not a defect.

For any computational manuscript also require: convergence/robustness evidence,
comparison against established methods, honest error characterization,
reproducibility information, and an explicit physical interpretation section.

## 14. Positioning advice (well-fitting but poorly framed) `[HEURISTIC]`

- **Title** — name the physics result, not the technique.
- **Abstract** — lead with the physical finding; the method belongs in the
  second sentence, not the first.
- **Introduction** — state the condensed-matter question the field has, then
  the gap, then this work. Not: "ML is popular in materials science."
- **Novelty claims** — one precise sentence on what was not previously known.
  Never inflate.
- **Comparison with prior work** — explicit, quantitative, and fair.
- **Discussion** — mechanism, not metrics. Explain *why* the system behaves so.
- **Figures** — at least one figure carrying physical insight, not only
  performance curves or parity plots.
- **Generality** — say plainly which conclusions transfer beyond the studied
  systems and which do not.

## 15. Submission checklist

- [ ] Central claim is a condensed-matter/materials-physics claim
- [ ] Correct journal chosen over PRL/PRX/PRResearch/PRMaterials/PRApplied/PRX Intelligence
- [ ] Article type chosen (Article vs. Letter); length limits fetched if Letter
- [ ] Section selected from the PRB section-selection guidelines
- [ ] Novelty stated explicitly and defensibly
- [ ] Evidence: convergence, uncertainties, baselines, controls
- [ ] Prior work cited and compared, including competing methods
- [ ] Figures legible, captioned, physically informative
- [ ] Supplemental material scoped per APS policy
- [ ] Data/code availability statement per APS open-science policy
- [ ] Author list, affiliations, funding, competing interests complete
- [ ] Any AI/ML tool use disclosed per current APS ethics policy

## 16. Decision workflow

1. State the primary physics question in one sentence.
2. State the central contribution in one sentence.
3. Name what is genuinely new (use the type list in §9C).
4. Classify the scientific domain.
5. Test scope fit (§4) — reject keyword-only matches.
6. Assess novelty, significance, conceptual and methodological contribution separately.
7. Assess breadth and evidence.
8. Run the neighbor table (§11) in both directions.
9. List editorial vulnerabilities.
10. Assign a fit class (§10) with reasons.
11. Give concrete positioning changes.
12. State confidence and what evidence would change it.

## 17. Output format

**Journal:** Physical Review B
**Fit:** Excellent / Strong / Moderate / Borderline / Poor
**Scope fit:** …
**Primary contribution:** …
**Novelty:** … (type: mechanism / phenomenon / material / method / interpretation)
**Scientific significance:** …
**Conceptual advance:** …
**Methodological contribution:** …
**Breadth of interest:** …
**Evidence and validation:** …
**Major strengths:** …
**Potential editorial concerns:** …
**Why this journal:** …
**Why not the closest alternatives:** …
**Recommended positioning changes:** …
**Submission considerations:** …
**Confidence:** High / Medium / Low — and why

Never state or imply that the manuscript will be accepted.

## 18. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRB-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High for theory and computation;
moderate for experimental papers, which still generally need the model linking
measurement to mechanism.

**Expected equation density:** Moderate to high, by section — many-body and
electronic-structure theory sit at the top of the range; growth and
characterization work at the bottom.

**Role of equations:** To define the model and make the mechanism explicit.
PRB's bar is authority and durability, so the formulation should be complete
enough that a later reader can reproduce and extend it, not merely follow it.

**Main-text mathematical content:** The model Hamiltonian or functional; the
approximation scheme (mean field, DFT functional, perturbative order,
diagrammatic truncation) with its validity regime; the principal analytical
result; definitions of any new quantity or order parameter; anything plotted.

**Supplementary mathematical content:** Derivations, symmetry analysis tables,
convergence studies, parameter tables, benchmark comparisons.

**Recommended derivation depth:** Moderate to full — PRB's flexible length
policy exists so papers can be thorough, and thoroughness is rewarded here.

**Figure–equation integration:** Band structures, phase diagrams, and response
functions should be tied to the equations defining them; a mechanism claim needs
a figure that tests it, not only one that displays it.

**Recommended presentation strategy:** `[HEURISTIC]` The most common PRB
weakness in computational work is a rich calculation with no mathematical
statement of the mechanism. If the paper claims a mechanism, write the relation
that expresses it — an effective Hamiltonian, a scaling form, a sum rule — and
test that relation in a figure. A parity plot is not a mechanism.

## 19. Presentation profile

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

**Typical mathematical density:** Moderate to High (see §Mathematical
presentation profile).

**Recommended main-text figure strategy:** `[STRATEGY]` Figure count follows the
argument; PRB's no-limit Regular Article format means there is no reason to
compress evidence out of the paper. Each figure should establish something the
text asserts — for a mechanism claim, at least one figure must *test* the
mechanism, not merely display data.

**Supplementary-material role:** Convergence studies, full parameter tables,
extended benchmarks, secondary systems, symmetry-analysis detail. Keep anything
required to evaluate the central claim in the main text.

**Preferred narrative style:** Detailed exposition. PRB rewards authority and
durability, so systematic development, complete methodology, and thorough
comparison with prior work are appropriate — this is a venue where being
thorough is a virtue rather than a length problem.

**Recommended manuscript compactness:** Low to Moderate — favor completeness.

**Presentation priority:** Rigor, reproducibility, and physical interpretation.

> `[REQUIREMENT]` For a **Letter**, PRB states that authors should justify the
> need for the short format in the submission letter, and that Letters receive
> priority handling. `[REQUIREMENT]` Authors may follow a Letter with a fuller
> account as a Regular Article.

## 20. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review B | https://journals.aps.org/prb/about | Official | 2026-08-19 | Identity, scope, acceptance criteria, article types |
| PRB section selection | https://journals.aps.org/prb/authors/guidelines-section-selection-physical-review-b | Official | 2026-08-19 | Section list (referenced, fetch for detail) |
| PRB editorial policies and practices | https://journals.aps.org/prb/authors/editorial-policies-practices | Official | 2026-08-19 | Article types (fetch for length limits) |
| APS Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Common policy |
| Scope of APS Journal Portfolio | https://journals.aps.org/scope | Official | 2026-08-19 | Portfolio subject coverage |

**Unknown — not stated in official sources:** acceptance rate, numeric length
limits (must be fetched), review timelines.

**Format facts above verified from** `https://journals.aps.org/prb/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
