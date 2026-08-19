---
name: aps-prxquantum
description: Evaluate a manuscript's fit for PRX Quantum — APS's highly selective gold open access journal for quantum information science and technology.
journal: PRX Quantum
abbreviation: PRX Quantum
journal_code: prxquantum
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

# PRX Quantum — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for essentially every submission here** — resource scaling, thresholds, and bounds are what make an "exceptional" claim checkable. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

PRX Quantum is "a highly selective journal in quantum science and technology…
an open access venue with high visibility," publishing "influential research
from a broad range of disciplines, shaping the future of quantum science."

It "showcases research in core areas of quantum information science and
technology that are milestone achievements in techniques, experiment, and
theory, or that represents an important leap in understanding," and publishes
"creative, impactful research that brings together multiple interdisciplinary
fields."

It builds on standards established by PRX, with a personalized, responsive
editorial process and flexible article lengths and formats.

## 2. Scope `[OFFICIAL]`

"All topics relevant to the diverse multidisciplinary quantum information
science and technology research communities spanning physics, computer science,
mathematics, chemistry, materials, engineering, and technology." Coverage
comprises fundamental and applied; theoretical and experimental, including
significant advances in methods and instrumentation; and interdisciplinary and
emerging areas. Full scope statement: `journals.aps.org/prxquantum/scope`.

## 3. Acceptance criteria `[OFFICIAL]`

Manuscripts should demonstrate exceptional achievements according to **at least
one**:

- **Exceptional advance** — pushing the field of quantum science and technology in a new and consequential direction.
- **Exceptional connection** — linking different areas within quantum science and technology, or between the field and other scientific disciplines.
- **Exceptional capabilities** — in engineering, computational concepts, techniques, materials, or methodologies allowing major challenges in the journal's topical areas to be solved.
- **Exceptional insight** — addressing a timely topic of high impact and interest across the multidisciplinary quantum science and technology community.

## 4. Editorial positioning `[INFERENCE]`

PRX Quantum takes the **exceptional subset** of what PRA, PRApplied, and PRB
would otherwise carry. The word "exceptional" appears in all four criteria and
is the operative filter. Solid, correct, useful quantum work is *not* the target
— that is PRA or PRResearch.

## 5. Strong-fit profile `[INFERENCE]`

- Milestone experimental demonstrations that change what is achievable.
- Theory that reframes a problem the community has been working on.
- Architectures, error-correction schemes, or protocols with major consequences.
- Work bridging quantum science with computer science, chemistry, or materials.
- Techniques and instrumentation that unlock a class of experiments.

## 6. Weak-fit patterns `[HEURISTIC]`

- Incremental protocol variants with modest resource improvements.
- Simulations of small systems with no scaling argument.
- Platform demonstrations that reproduce known results.
- "Quantum advantage" claims without honest classical baselines.
- Solid, publishable quantum work whose significance is ordinary — route to PRA.

## 7. Evaluation framework

**A. Scope fit** · **B. Criterion match** (which "exceptional", with evidence) ·
**C. Milestone test** (what is now possible that was not?) · **D. Scaling and
resource analysis** · **E. Baselines, including classical** ·
**F. Cross-community relevance** · **G. Positioning vs. PRA / PRApplied / PRB /
PRX / PRL / PRResearch / PRX Intelligence.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Clear exceptional achievement on a named criterion; milestone-level; well evidenced |
| **Strong** | Meets a criterion; impact real though somewhat concentrated |
| **Moderate** | Important work whose "exceptional" claim depends on framing or missing analysis |
| **Borderline** | Solid quantum work at ordinary significance — PRA is the better home |
| **Poor** | Incremental, or claims unsupported by baselines |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRA** | Solid, significant quantum-science or AMO work at specialist tier |
| **PRApplied** | The claim is a quantum device or application with physical insight |
| **PRB** | The system is condensed matter — qubit materials, solid-state platforms as materials physics |
| **PRX** | The advance is a broad physics discovery beyond quantum information |
| **PRL** | Pivotal, broadly interesting, compressible |
| **PRX Intelligence** | The central contribution is AI/ML methodology (including ML for quantum) |
| **PRResearch** | Significant work not reaching "exceptional"; gold OA wanted |

Prefer **PRX Quantum** when: the work is exceptional in a named dimension and
speaks across the quantum science and technology communities.

## 10. Article types `[OFFICIAL]`

Regular **research articles**, plus:

- **Perspectives** — forward-looking articles highlighting the significance of recent results, their possible reach and current limitations. `[OFFICIAL]` 7500 words.
- **Tutorials** — hands-on guides for newcomers, covering well-established concepts of particular relevance on timely topics. `[OFFICIAL]` 37,500 words.
- **Roadmaps** — `[OFFICIAL]` no length limit.

`[OFFICIAL]` Research Articles have no length limit; Comments/Replies are 3500
words. Verified 2026-08-19. Gold open access; APC applies.

## 11. Positioning advice `[HEURISTIC]`

- Name the criterion in the abstract and support it with a result.
- Quantify the milestone: resources, fidelity, scale, error rates — with
  comparison to the previous best.
- Give honest classical/conventional baselines.
- Provide scaling analysis; a demonstration without scaling reads as a
  proof-of-concept.
- For cross-disciplinary claims, deliver results both communities need.

## 12. Submission checklist

- [ ] Named "exceptional" criterion with supporting evidence
- [ ] Milestone quantified against previous best
- [ ] Classical/conventional baselines included
- [ ] Scaling and resource analysis present
- [ ] Article type chosen (Article / Perspective / Tutorial)
- [ ] PRA alternative considered and reason for PRX Quantum stated
- [ ] APC/funding or waiver eligibility settled
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Scope fit. 3. Criterion match. 4. Milestone test.
5. Baselines and scaling. 6. Cross-community relevance. 7. Neighbor comparison
(PRA first). 8. Vulnerabilities. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Criterion claimed:** advance / connection / capabilities / insight — justification.
**Why not PRA:** …

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRX Quantum-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High. Protocols, codes,
architectures, and error models require formal specification to be assessed as
"exceptional."

**Expected equation density:** Moderate to high, with a wide range across a
scope spanning physics, computer science, and mathematics.

**Role of equations:** To specify the protocol and its guarantees. At this tier
the mathematics substantiates the claim: resource scaling, error thresholds,
fidelity bounds, and complexity statements are what make a milestone claim
checkable rather than asserted.

**Main-text mathematical content:** The model of the system and its noise; the
protocol or code definition; resource counts and their scaling; the principal
theorem or bound; the assumptions under which it holds.

**Supplementary mathematical content:** Full proofs, numerical benchmarking
detail, alternative noise models, auxiliary lemmas.

**Recommended derivation depth:** State theorems and assumptions in the main
text; proofs may go to appendices. Flexible article lengths accommodate either.

**Figure–equation integration:** Scaling plots should show the analytically
predicted scaling alongside the numerics; threshold and fidelity claims should
plot the quantity as defined.

**Recommended presentation strategy:** `[HEURISTIC]` Separate **proven**,
**numerically demonstrated**, and **conjectured** explicitly — at this
selectivity the distinction is scrutinized. State the noise model and the
assumptions on which any advantage claim rests, and give the classical or
conventional baseline in comparable mathematical terms.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Perspectives | **7500 words** |
| **Tutorials** | **37,500 words** |
| **Roadmaps** | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Flexible lengths and formats.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate to High.

**Recommended main-text figure strategy:** `[STRATEGY]` Scaling plots, threshold
curves, and resource comparisons carry milestone claims; each should show the
analytic prediction alongside the numerics and name the baseline it is measured
against.

**Supplementary-material role:** Full proofs, noise-model variants, calibration
and benchmarking detail.

**Preferred narrative style:** Detailed exposition for a readership spanning
physics, computer science, and engineering — define terms across those
conventions.

**Recommended manuscript compactness:** Moderate.

**Presentation priority:** Making the "exceptional" claim checkable — proven vs.
numerically demonstrated vs. conjectured, marked explicitly.

> **Tutorials** (37,500 words) and **Roadmaps** are substantial, distinct
> formats. `[STRATEGY]` A Tutorial is a training document for newcomers, not a
> long research paper; do not propose one as a way around a length constraint.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About PRX Quantum | https://journals.aps.org/prxquantum/about | Official | 2026-08-19 | Identity, scope, criteria, article types |
| PRX Quantum scope | https://journals.aps.org/prxquantum/scope | Official | 2026-08-19 | Subject areas (fetch) |
| APS APCs | https://journals.aps.org/authors/apcs | Official | 2026-08-19 | Gold OA charges |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prxquantum/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
