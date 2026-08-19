---
name: aps-prresearch
description: Evaluate a manuscript's fit for Physical Review Research — APS's broad, multidisciplinary gold open access journal covering all topics with a connection to physics.
journal: Physical Review Research
abbreviation: PRResearch
journal_code: prresearch
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

# Physical Review Research — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` when the submission is theoretical or computational**, and calibrate density against the manuscript's subfield rather than against PRResearch as a whole. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

PRResearch is "a trusted and multidisciplinary open access journal reporting
high-quality, significant developments in all areas of science with a connection
to physics." It is peer-reviewed, international, and covers all research topics
of interest to physicists and researchers in related fields.

It "complements other titles in the portfolio by offering an option for authors
across the physics community who value and trust the publishing experience and
quality of *Physical Review* journals, and also want or need to publish in a
fully open access publication."

Stated aims include broad dissemination to a global audience, "initiating
conversations across traditional boundaries," facilitating collaboration, and
enabling future discoveries.

## 2. Scope `[OFFICIAL]`

"The full spectrum of research topics of interest to the physics community."
Coverage comprises:

- fundamental **and** applied;
- theoretical **and** experimental, including technical and methodological advances;
- interdisciplinary and newly emerging areas.

Full scope statement: `journals.aps.org/prresearch/scope`.

> `[INFERENCE]` PRResearch has the widest scope in the portfolio after PRL/PRX.
> Scope-based rejection is rare; the discriminator is §3 plus the existence of a
> better-matched specialist home.

## 3. Acceptance criteria `[OFFICIAL]`

- Add to the existing knowledge related to a particular field of research with a connection to physics.
- Make a high-quality, significant contribution and generate interest for readers with a connection to physics.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

| Dimension | PRResearch's demand |
|---|---|
| Novelty | Real, need not be pivotal |
| Significance | High-quality and significant; not field-defining |
| Breadth | Interest to readers "with a connection to physics" — wide but not required to be universal |
| Access | Gold OA — an APC applies |
| Interdisciplinarity | Actively welcomed, including topics that fall between specialist journals |

Two distinct reasons to choose PRResearch `[INFERENCE]`:

1. **Fit reason** — the work sits between or outside the specialist journals'
   natural territories, or is deliberately interdisciplinary.
2. **Access reason** — the work would fit a hybrid specialist journal, but the
   authors need or want fully open access (funder mandate, dissemination goals).

Both are legitimate. State which applies; do not dress an access reason as a
scope reason.

## 5. Strong-fit profile `[INFERENCE]`

- Solid, complete, significant work whose audience spans more than one community.
- Emerging-topic work with no established specialist home.
- Methodological or technical advances of genuine utility.
- Work that would be a good specialist-journal paper where OA is required.

## 6. Weak-fit patterns `[HEURISTIC]`

- Thin or preliminary results — "open access" is not a lower quality bar; the
  criteria still demand a substantive, authoritative contribution.
- Work with an obvious, better-matched specialist home and no OA rationale
  (the specialist journal's focused readership usually serves the author better).
- Manuscripts previously rejected elsewhere resubmitted without addressing the
  substantive criticism.
- Connection to physics asserted rather than present.

## 7. Evaluation framework

- **A. Connection to physics** — real and central, or decorative?
- **B. Significance** — substantive addition, or minimal increment?
- **C. Audience** — which communities, and do they overlap in one venue?
- **D. Specialist alternative** — is there a better-matched journal, and is there an OA reason to override it?
- **E. Completeness and evidence** — authoritative treatment?
- **F. Tier check** — does it in fact reach PRL/PRX/domain-PRX territory?

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Significant, complete, genuinely multidisciplinary or emerging-topic work with clear physics connection |
| **Strong** | Solid significant contribution; specialist alternative exists but OA or breadth justifies PRResearch |
| **Moderate** | In scope and sound; significance or completeness needs strengthening |
| **Borderline** | A specialist journal is clearly the better home and no OA rationale is offered |
| **Poor** | Physics connection is decorative, or the contribution is not substantive |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRL** | Pivotal, broadly interesting, compressible to a Letter |
| **PRX** | Field-defining discovery or landmark; highly selective tier |
| **PRB / PRA / PRC / PRD / PRE / PRFluids / PRMaterials / PRApplied / PRAB** | The work belongs squarely to that research area and OA is not a constraint — the focused readership is the advantage |
| **PRX Quantum / PRX Energy / PRX Life / PRX Intelligence** | The domain matches *and* the work meets an "exceptional" criterion |
| **APS Open Science** | The output is data, software, a replication study, or a negative/null result |
| **PRPER** | The topic is physics education research |

Prefer **PRResearch** when: the work is significant and in-scope, gold OA is
wanted or needed, or the topic genuinely straddles specialist boundaries.

## 10. Article types and requirements `[OFFICIAL]`

Fetch `/prresearch/authors` for current article types, length guidance, and
required components. PRResearch is gold open access; an APC applies
(`journals.aps.org/authors/apcs`), with waivers for authors from lower-income
countries.

## 11. Positioning advice `[HEURISTIC]`

- Name the communities the work serves, in the abstract.
- Make the physics connection explicit and load-bearing, especially for
  chemistry/biology/CS-adjacent work.
- Do not undersell: the criteria still require significance. Framing work as
  "a modest contribution" invites the corresponding decision.
- If transferring from another *Physical Review* journal, address the prior
  referee criticism substantively in the cover letter.

## 12. Submission checklist

- [ ] Physics connection explicit and central
- [ ] Significance argued against the three criteria
- [ ] Specialist alternative considered; reason for PRResearch stated
- [ ] APC/funding or waiver eligibility settled
- [ ] Data/code availability per APS open-science policy
- [ ] Prior work compared; any transfer history addressed
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Physics connection. 3. Audience map.
4. Significance vs. the three criteria. 5. Specialist alternative + OA
rationale. 6. Upper-tier check (PRL/PRX/domain PRX). 7. Evidence and
completeness. 8. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Reason for PRResearch:** fit / access / both — stated explicitly.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRResearch-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Varies widely — PRResearch spans the
full physics spectrum, so calibrate against the manuscript's *subfield*, using
the corresponding specialist journal's profile as the reference point.

**Expected equation density:** Follow the subfield norm, not a journal norm.

**Role of equations:** Standard — define the model, state the result, support
the claim. No format-driven pressure toward compression.

**Main-text mathematical content:** Defining equations, principal results, key
approximations, anything needed to read the figures.

**Supplementary mathematical content:** Derivations, intermediate steps,
robustness analysis.

**Recommended derivation depth:** As the subfield expects.

**Figure–equation integration:** Standard theory → prediction → evidence chain,
made explicit.

**Recommended presentation strategy:** Because PRResearch readers arrive from
adjacent fields, define notation carefully and do not assume a subfield's
conventions. `[HEURISTIC]` Interdisciplinary work in particular should state
what each symbol means in physical terms, since two communities will read it.

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

**Typical mathematical density:** Varies by subfield (see §Mathematical presentation profile).

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
content. PRResearch's own guidance is that the appropriate length depends on the
information the article contains.

**Presentation priority:** Accessibility across communities. `[STRATEGY]` Define notation and terms without assuming one subfield's conventions — readers arrive from adjacent fields.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Research | https://journals.aps.org/prresearch/about | Official | 2026-08-19 | Identity, aims, scope, criteria |
| PRResearch scope | https://journals.aps.org/prresearch/scope | Official | 2026-08-19 | Detailed scope (fetch) |
| PRResearch Information for Authors | https://journals.aps.org/prresearch/authors | Official | 2026-08-19 | Article types, requirements (fetch) |
| APS APCs | https://journals.aps.org/authors/apcs | Official | 2026-08-19 | Gold OA charges |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prresearch/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
