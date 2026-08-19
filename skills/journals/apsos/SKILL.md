---
name: aps-apsos
description: Evaluate a manuscript's fit for APS Open Science — APS's community-driven open access journal for rigorous research across the scientific process, including data, software, replications, and null results.
journal: APS Open Science
abbreviation: APS Open Science
journal_code: apsos
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

# APS Open Science — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` when formalism is needed for verification** — including null results, where the sensitivity calculation is what makes the submission valuable. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Identity `[OFFICIAL]`

APS Open Science is "a trusted, community-driven open access journal that
publishes high-quality, useful research through rigorous peer review that
ensures research from every stage of the scientific process receives the
recognition it deserves." It is "a fully open access, peer-reviewed journal for
physics and related fields, that supports the global open science movement by
providing a welcoming space for researchers worldwide."

The journal "aims to provide flexible article formats and new article types for
diverse research outputs, with rapid peer review and publication processes."
Beyond research papers, it "welcomes **data and software advances**,
**replication studies**, as well as **negative and null results** that
contribute valuable knowledge, recognizing their importance for scientific
progress." It also provides "efficient manuscript transfers from *Physical
Review* journals."

APS describes it as "an experimental sandbox for APS Publications," testing
innovative features that may later be adopted across APS publications
`[OFFICIAL]`.

> `[HEURISTIC]` This is the portfolio's home for work that is **correct and
> useful but not "significant"** by the other journals' criteria. That is a real
> gap it fills — not a consolation prize.

## 2. Scope `[OFFICIAL]`

"The full spectrum of research topics of interest to the physics community, its
subdisciplines, and adjacent fields." Coverage: fundamental and applied;
theoretical and experimental, including technical and methodological advances;
and interdisciplinary and newly emerging areas. Full scope:
`journals.aps.org/apsos/scope`.

## 3. Acceptance criteria `[OFFICIAL]`

Submitted manuscripts should:

- **Present high-quality primary research** using appropriate methods with scientific rigor.
- **Be technically correct** with rigorous execution and proper application of methods yielding valid, reliable, and useful results.
- **Add meaningfully** to existing knowledge in physics or related fields.
- **Provide transparency** with sufficient detail for verification and follow research integrity standards.

> `[INFERENCE]` Note the deliberate absence of a significance/impact criterion.
> The bar is **soundness, usefulness, and transparency** — a *technical* bar
> rather than an *editorial-selectivity* bar. This is the single most important
> distinction between APS Open Science and every other title in the portfolio.

## 4. Editorial positioning `[INFERENCE]`

| Dimension | The demand |
|---|---|
| Novelty | Meaningful addition; need not be striking |
| Significance | **Not** a stated criterion |
| Rigor | High — this is where the bar sits |
| Transparency | High — sufficient detail for verification |
| Output type | Deliberately broad: papers, data, software, replications, null results |
| Access | Gold OA |

## 5. Strong-fit profile `[INFERENCE]`

- Technically sound work whose interest is real but modest.
- Datasets and software with documentation, licensing, and demonstrated utility.
- Replication studies confirming or failing to confirm published results.
- Negative and null results that close off a hypothesis.
- Methodological or technical notes useful to practitioners.
- Manuscripts transferred from another *Physical Review* journal where the
  science is sound but the significance bar was not met.

## 6. Weak-fit patterns `[HEURISTIC]`

- Work failing the technical-correctness bar — soundness is the criterion here,
  so methodological flaws are fatal rather than merely limiting.
- Insufficient detail for verification.
- Datasets without documentation, provenance, or license.
- Null results with underpowered designs — a null needs enough sensitivity to
  mean something.
- Work that clearly meets a selective journal's criteria and would be better
  served there.

## 7. Evaluation framework

**A. Scope fit** · **B. Technical correctness** (the gate) · **C. Meaningful
addition** · **D. Transparency and verifiability** · **E. Output-type match**
(paper / data / software / replication / null) · **F. Research-integrity
compliance** · **G. Whether a selective journal is warranted instead.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Rigorous, transparent, clearly useful — especially data, software, replication, or a well-powered null result |
| **Strong** | Technically sound and useful; documentation complete |
| **Moderate** | Sound but under-documented or thin on demonstrated usefulness |
| **Borderline** | Would be better served by a selective journal, or usefulness is unclear |
| **Poor** | Technically flawed, or not verifiable from what is provided |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRResearch** | The work is significant as well as sound, and a broad physics readership is wanted |
| **Specialist journals (PRA–PRE, PRMaterials, PRApplied, PRFluids, PRAB)** | The work makes a significant contribution in that research area |
| **PRL / PRX / domain PRX titles** | The work is pivotal, field-defining, or exceptional |
| **PRPER** | It is physics education research (which also welcomes replications) |

Prefer **APS Open Science** when: the work is rigorous and useful but its value
is soundness, reusability, or completing the record rather than significance.

## 10. Article types and requirements `[OFFICIAL]`

`[OFFICIAL]` Verified article types (2026-08-19): Regular Articles (no length
limit); **Letters** (4500 words); **Data/Code** (no length limit);
**Replication** (no length limit); **Negative/Null** (no length limit);
**Protocol** (no length limit); Review Articles (30,000 words).

Rapid peer review and publication; efficient transfers from *Physical Review*
journals. Re-fetch `/apsos/authors` before advising — this journal is an
explicit experimental sandbox and its types are the most likely in the portfolio
to change. Gold open access; APC applies.

> `[HEURISTIC]` As an explicitly experimental venue, its article types and
> features are more likely than most to have changed. Always re-fetch before
> advising.

## 11. Positioning advice `[HEURISTIC]`

- Do not oversell. Claiming significance invites the significance question this
  journal deliberately does not ask.
- State usefulness concretely: who will reuse this, and for what.
- For data/software: document schema, provenance, licence, version, dependencies,
  and provide a working example.
- For replications: state the original claim, the protocol followed, deviations,
  and the outcome plainly.
- For null results: report statistical power or sensitivity — this is what makes
  a null informative.
- For transfers: state the transfer history and how prior review was addressed.

## 12. Submission checklist

- [ ] Technically correct and rigorously executed
- [ ] Sufficient detail for independent verification
- [ ] Usefulness stated concretely
- [ ] Output type matched to a supported article type (fetched)
- [ ] Data/software documented, licensed, versioned
- [ ] For nulls: sensitivity/power reported
- [ ] For replications: original claim and deviations documented
- [ ] Transfer history addressed if applicable
- [ ] APC/funding or waiver eligibility settled
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central output — paper, data, software, replication, or null?
2. Scope fit. 3. Technical-correctness gate. 4. Meaningful-addition test.
5. Transparency and verifiability. 6. Selective-journal check (is a better
venue warranted?). 7. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, with **Scientific significance** replaced by:
**Technical correctness:** …
**Usefulness:** who reuses this and for what.
**Verifiability:** is there enough detail?

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. APS Open Science-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Varies entirely with the submission
type; calibrate against the subfield's specialist journal.

**Expected equation density:** Follow the subfield norm.

**Role of equations:** To support **verifiability**, which is this journal's
distinctive criterion. The formalism must be complete enough that a reader can
check and reuse the work, since transparency and technical correctness — not
significance — are the stated bar.

**Main-text mathematical content:** Complete model and method specification;
definitions of every reported quantity; the analysis or estimator used. For
replication studies, the original formulation and any deviation from it, stated
precisely.

**Supplementary mathematical content:** Derivations, extended parameter sets,
full analysis specifications, computational detail.

**Recommended derivation depth:** Whatever verification requires — the bar is
sufficient detail for independent checking, so err toward completeness rather
than compression.

**Figure–equation integration:** Every plotted quantity should be defined; data
and code releases should document the mathematical definitions their fields
implement.

**Recommended presentation strategy:** `[HEURISTIC]` For **null results**, state
the sensitivity or power calculation mathematically — a null without a
quantified detection threshold is uninformative, and this is the calculation
that makes such a submission valuable. For **data and software** submissions,
document the equations the code implements, including conventions and units. For
**replications**, write the original model and the reproduced one side by side
so deviations are visible.

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
| **Data/Code** | no length limit |
| **Replication** | no length limit |
| **Negative/Null** | no length limit |
| **Protocol** | no length limit |
| Review Articles | **30,000 words** |

**No figure limit is stated.**


**Article format:** Deliberately diverse — the portfolio's widest type menu,
matching the journal's remit for outputs from every stage of the scientific
process.

> `[REQUIREMENT]` **Replication**, **Negative/Null**, **Protocol**, and
> **Data/Code** are named article types here. `[STRATEGY]` Choose the type that
> matches the output rather than forcing the work into a Regular Article; the
> type is what signals to readers what kind of contribution they are getting.
> A **Protocol** paper is a distinctive option — a method or study plan
> published before results exist.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Varies with submission type and subfield.

**Recommended main-text figure strategy:** `[STRATEGY]` Verifiability governs.
Include the figures a reader needs to check the work; for a null result, the
sensitivity or power analysis is a main-text figure, not an appendix item.

**Supplementary-material role:** Extended analysis, full datasets, complete
computational specifications — but note that this journal's bar is transparency,
so err toward including rather than relegating.

**Preferred narrative style:** Plain and complete. `[STRATEGY]` Do not oversell;
claiming significance invites the significance question this journal
deliberately does not ask.

**Recommended manuscript compactness:** Low — completeness serves verification.

**Presentation priority:** Sufficient detail for independent verification, with
data, code, licenses, and versions documented.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About APS Open Science | https://journals.aps.org/apsos/about | Official | 2026-08-19 | Identity, scope, criteria, article types, transfers |
| APS Open Science scope | https://journals.aps.org/apsos/scope | Official | 2026-08-19 | Detailed scope (fetch) |
| APS Open Science Information for Authors | https://journals.aps.org/apsos/authors | Official | 2026-08-19 | Article types and requirements (fetch) |

**Unknown — not stated in official sources:** APC amount (see APS APC page),
acceptance rate, length limits, timelines.

**Format facts above verified from** `https://journals.aps.org/apsos/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
