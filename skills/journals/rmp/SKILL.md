---
name: aps-rmp
description: Evaluate a manuscript's fit for Reviews of Modern Physics — APS's premier venue for in-depth Reviews and Colloquia across all of physics.
journal: Reviews of Modern Physics
abbreviation: RMP
journal_code: rmp
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

# Reviews of Modern Physics — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for essentially every Review** — a review's unifying notation is one of its main contributions. Colloquia may need it less. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

RMP is "the premier APS venue for publishing in-depth reviews of critical or
timely topics that give context to current research trends in physics and
adjacent fields." Since 1929 it has provided "an unrivaled venue for
authoritative review papers in all fields of physics."

## 2. Article types `[OFFICIAL]`

RMP publishes **two types of essay**, plus Nobel Lectures:

- **Reviews** (article type: *Articles*) — "present the current status of a
  given topic, with historical background, a critical distillation of research
  progress, and a summary of possible future developments." `[OFFICIAL]` Length
  limit **50,000 words**, corresponding to about 50 printed pages.
- **Colloquia** — "communicate results at the frontiers of physics, which may
  impact several subfields." `[OFFICIAL]` Length limit **20,000 words**.
- **Nobel Lectures** — text of the addresses given in conjunction with the awards.

`[OFFICIAL]` RMP asks authors to give considerable attention to presentation, to
make the introduction accessible to graduate students and readers from other
fields, to organize the body economically and thoughtfully, and to follow the
physics notation conventions of graduate-level textbooks unless there is a
compelling reason otherwise. Verified 2026-08-19.

> **Critical distinction** `[OFFICIAL]`: RMP does not publish primary research.
> A manuscript reporting new results does not belong here regardless of quality.

## 3. Scope `[OFFICIAL]`

The full range of applied, fundamental, and interdisciplinary physics topics
covered by the *Physical Review* portfolio. Specific areas of interest include:
applied physics; astronomy and astrophysics; astroparticle physics; atomic,
molecular, and optical physics; biological physics; chemical physics; climate
science; computational physics; condensed matter physics; cosmology and
gravitation; fluids and solids; general physics; geophysics; high-energy
physics, particles, and fields; **machine learning**; materials science;
mathematical physics; nuclear physics; particle-beam and accelerator physics;
plasma physics and fusion; quantum information; and soft matter.

## 4. Editorial positioning `[INFERENCE]`

RMP's currency is **authority and synthesis**. The three demands implicit in the
Review definition are: historical context, *critical* distillation (judgment,
not enumeration), and a forward view. A comprehensive but uncritical survey is
not an RMP Review.

**Review vs. Colloquium** `[INFERENCE]`: a Review is the definitive treatment of
an established topic; a Colloquium is shorter, frontier-facing, and aimed at
cross-subfield readers.

## 5. Strong-fit profile `[INFERENCE]`

- A topic mature enough to review and important enough to warrant one.
- Authors with the standing and breadth to render critical judgments.
- Genuine synthesis: reconciling conflicting results, identifying what is
  settled and what is not.
- Historical development that explains why the field asks its current questions.
- A forward section identifying open problems others can act on.
- For Colloquia: a frontier development that several subfields need explained.

## 6. Weak-fit patterns `[HEURISTIC]`

- A literature enumeration with no critical judgment.
- A review of the authors' own program.
- Topics too young to have a settled core, or too narrow for the readership.
- Primary research results dressed as a review.
- Reviews duplicating a recent authoritative review with no new perspective.

## 7. Practical note on commissioning `[HEURISTIC]`

Review journals commonly work through proposals and invitations. **The current
RMP submission and proposal procedure has not been recorded in this skill** —
fetch `/rmp/authors` before advising an author on whether to propose, submit
directly, or seek an invitation. Do not assert that RMP is invitation-only.

## 8. Evaluation framework

**A. Type test** — review/colloquium, or primary research? (blocking) ·
**B. Topic maturity and importance** · **C. Criticality** — does it judge? ·
**D. Comprehensiveness and balance** · **E. Historical context** ·
**F. Forward view** · **G. Audience breadth** · **H. Author standing and
independence** (competing interests, self-citation balance).

## 9. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Definitive, critical synthesis of an important topic, with context and a forward view; broad readership |
| **Strong** | Authoritative review of a significant topic; balance and criticality good |
| **Moderate** | Useful survey; needs more critical judgment, breadth, or forward analysis |
| **Borderline** | Topic too narrow or too new; or better suited as a Colloquium than a Review (or vice versa) |
| **Poor** | Primary research, or an uncritical or self-focused survey |

## 10. Neighboring APS venues

| Venue | Prefer it when… |
|---|---|
| **PRMaterials / PRApplied / PRAB Review Articles** | The review is domain-specific and aimed at that journal's specialist community |
| **PRX Quantum Perspectives / Tutorials** | The piece is forward-looking commentary or a training tutorial in quantum science |
| **PRApplied Perspectives** | The piece is opinion and direction in applied physics |
| **PRL / PRX / specialist journals** | The manuscript reports new results |

Prefer **RMP** when: the piece is an authoritative, critical synthesis for the
whole physics community.

## 11. Positioning advice `[HEURISTIC]`

- Decide Review vs. Colloquium first; they are different pieces, not different lengths.
- Make judgments: say which results have held up and which have not, and why.
- Balance citation across groups; check self-citation proportion.
- Structure so a non-specialist physicist can enter and a specialist still gains.
- Give the open-problems section real content — it is the most-read part.
- Declare competing interests, including commercial involvement in the topic.

## 12. Submission checklist

- [ ] Piece is a review/colloquium, not primary research
- [ ] Type chosen deliberately (Review vs. Colloquium)
- [ ] Current submission/proposal procedure fetched from `/rmp/authors`
- [ ] Topic maturity and importance argued
- [ ] Critical judgments present throughout
- [ ] Historical context included
- [ ] Open problems and future directions section
- [ ] Citation balance and self-citation checked
- [ ] Figure permissions cleared for reproduced material
- [ ] Competing interests declared per APS policy
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Type test (blocking). 2. Topic maturity and importance. 3. Criticality test.
4. Comprehensiveness and balance. 5. Historical and forward coverage.
6. Audience breadth. 7. Author standing and independence. 8. Alternative venues.
9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, adapted:
**Piece type:** Review / Colloquium — with justification.
**Criticality:** evidence that the piece judges rather than enumerates.
**Topic maturity:** …

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. RMP-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Very High for Reviews in theoretical
areas; moderate for Colloquia, which address several subfields at once.

**Expected equation density:** High — but the function differs from a research
paper. Here mathematics is **pedagogical and unifying**: it establishes a common
notation in which a scattered literature can be compared.

**Role of equations:** To give the field one consistent formalism. A review's
distinctive contribution is often translating incompatible conventions from
different groups into a single notation, then showing what the results have in
common.

**Main-text mathematical content:** The unifying framework; definitions with a
clearly stated convention; the key results of the reviewed literature restated
in that common notation; the relationships between competing formulations.

**Supplementary mathematical content:** Appendices for derivations, convention
translation tables, and technical background the main narrative does not need.

**Recommended derivation depth:** Selective but substantial — derive what
illuminates, cite what is routine. A review that reproduces every derivation
becomes a textbook; one that reproduces none cannot compare results.

**Figure–equation integration:** Figures reproduced from the literature should be
re-expressed in the review's notation where possible, with units and conventions
reconciled and sources credited.

**Recommended presentation strategy:** `[HEURISTIC]` Fix notation and
conventions in an early section and hold them throughout — this is among a
review's most valuable services to the field. Say explicitly where the
literature's conventions conflict and which one this review adopts. For
Colloquia, keep the formalism light enough that readers from neighboring
subfields can follow the argument.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| **Articles** (Reviews) | **50,000 words** — about 50 printed pages |
| **Colloquia** | **20,000 words** |

**No figure limit is stated.**


**Article format:** Long-form review. The largest length allowance in the
portfolio.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** High — pedagogical and unifying rather than
result-producing.

**Recommended main-text figure strategy:** `[STRATEGY]` Figures reproduced from
the literature should be re-expressed in the review's notation and units where
possible, with sources credited and permissions cleared. A review's most
valuable figures are often synthetic — comparisons across studies that no
single original paper contains.

**Supplementary-material role:** Convention-translation tables, technical
background, extended derivations the narrative does not need.

**Preferred narrative style:** `[REQUIREMENT]` RMP asks authors to "give
considerable attention to the presentation of their material" and to **make the
introduction accessible to graduate students and readers from other fields**;
the body should be "economically and thoughtfully organized"; and **notation
should follow the physics conventions established in graduate-level textbooks
unless there is a compelling reason to do otherwise**. These are stated
requirements, not style suggestions.

**Recommended manuscript compactness:** Low — but "economically organized" means
50,000 words is a ceiling, not a target.

**Presentation priority:** Accessibility at the entry point, critical judgment
throughout, and a genuinely useful open-problems section.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Reviews of Modern Physics | https://journals.aps.org/rmp/about | Official | 2026-08-19 | Identity, article types, scope |
| RMP Information for Authors | https://journals.aps.org/rmp/authors | Official | 2026-08-19 | Submission/proposal procedure — **must be fetched before advising** |
| Scope of APS Journal Portfolio | https://journals.aps.org/scope | Official | 2026-08-19 | Portfolio coverage |

**Unknown — not stated in official sources at access date:** submission vs.
invitation procedure, length expectations, acceptance rate, timelines.

**Format facts above verified from** `https://journals.aps.org/rmp/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
