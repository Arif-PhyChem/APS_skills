---
name: aps-submission-assistant
description: Prepare an APS submission package — cover letter, criteria justification, article-type and section selection, checklist, and response-to-referees — once the target journal is chosen.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# APS Submission Assistant

Load `aps-common` and the target journal's skill. Run this **after** placement
is settled, not instead of settling it.

## 1. Prerequisites

Do not draft submission materials until you have:

- [ ] the target journal, chosen with reasons;
- [ ] the article type;
- [ ] the manuscript's central claim in one sentence;
- [ ] the journal's stated acceptance criteria (from its skill or freshly fetched);
- [ ] the current author-page requirements, **fetched** — length limits, required
      statements, and submission components are the facts most likely to be
      stale, and must never be asserted from memory.

## 2. Article type and section

1. Confirm the type exists at this journal (types differ: PRMaterials has
   Research Updates; PRApplied has Perspectives; PRX Quantum has Perspectives
   and Tutorials; PRAB and PRPER publish Reviews; PRPER publishes replication
   studies; APS Open Science takes data, software, and null results).
2. Choose the subject section from the journal's section-selection guidelines.
3. For a **Letter** at a specialist journal, confirm the manuscript genuinely
   warrants the short, high-importance format — and never let the author confuse
   it with a *Physical Review Letters* paper.

## 3. Cover letter

Structure — one page, no more:

1. **What the paper reports** — the central claim, one or two sentences, plain.
2. **Why it meets this journal's criteria** — name the criterion in the
   journal's own words and give the result that satisfies it.
3. **Why this journal** — audience and positioning, briefly.
4. **Context** — relation to prior work, including the authors' own; any
   companion or overlapping submissions.
5. **Housekeeping** — transfer history if any, suggested and excluded referees
   with reasons, competing interests, prior presentation of the work.

Rules:
- No adjectives doing the work of evidence ("groundbreaking", "first-ever").
- No claims not supported inside the manuscript.
- Never assert or imply an expected decision.

## 4. Criteria justification statement

Some journals require a separate short justification at submission. `[OFFICIAL]`
PRL requires a short paragraph (reported as ~100 words) explaining why the
manuscript meets its criteria — **fetch `/prl/authors` for the current wording
and word count before drafting.**

Template (adapt to the journal's actual requirement):

> This work [names the criterion]. Specifically, [the result], which [what it
> enables or settles]. This matters to [community], because [consequence].
> Previously, [state of the art]; this work [precise delta].

Then delete every word that is not doing work.

## 5. Manuscript components checklist

Portfolio-general; confirm specifics on the journal's author page.

- [ ] Title stating the claim
- [ ] Abstract leading with the result
- [ ] Author names, affiliations, ORCIDs
- [ ] Corresponding-author details
- [ ] Funding and acknowledgments
- [ ] Competing-interests statement
- [ ] Author-contribution statement (per current APS authorship policy)
- [ ] Data availability statement
- [ ] Code/software availability statement where applicable
- [ ] AI-tool use disclosure per current APS ethics policy
- [ ] References complete and formatted per APS style
- [ ] Figures at required resolution, legible in print, colorblind-safe
- [ ] Tables formatted; long tables moved to supplemental material
- [ ] Supplemental material scoped per APS policy and referenced from the text
- [ ] Length within the article type's limit (fetched, not assumed)
- [ ] Suggested and excluded referees with justifications
- [ ] arXiv posting and, for PRC/PRD, SCOAP³ eligibility considered
- [ ] Open-access route and APC funding or waiver eligibility settled

## 6. Mathematical content placement

For equation-driven manuscripts, settle this before final formatting — it is a
scientific decision, not a typesetting one. Load `aps-mathematical-presentation`.

- [ ] Essential equations identified and **kept in the main text**
- [ ] Supporting equations shortened, combined, or moved as appropriate
- [ ] Derivational detail placed in an appendix or Supplemental Material
- [ ] Every displayed equation has an identifiable purpose
- [ ] Every symbol defined at first use; conventions and units fixed once
- [ ] Every approximation stated with its regime of validity
- [ ] Each important equation followed by its physical reading
- [ ] Figures tied to the equations defining what they plot
- [ ] Supplemental-material policy fetched from the journal's author page
- [ ] Equation numbering consistent; all cross-references resolve

> **If the essential equations do not fit the article type's length, do not cut
> them.** Change the article type, or reconsider the journal. Cutting the
> defining equation to fit the box is the failure this checklist exists to
> prevent.

## 6b. Format and figure placement

Load `aps-format-and-presentation`. Settle before final formatting:

- [ ] Article type confirmed to exist **at this journal**, with its current limit fetched
- [ ] Length within that limit — or the article type changed rather than content cut
- [ ] Containers identified: appendix, **End Matter (PRL only)**, Supplemental Material
- [ ] Figure count derived from the argument, not a target; each figure proves something
- [ ] Multi-panel combinations tested for unity — related panels only
- [ ] Nothing essential to understanding or evaluating the central claim in Supplemental Material
- [ ] Supplemental Material cited in the reference list with a brief description
- [ ] Where a Letter is chosen, its justification drafted if the journal asks for one (PRB does)
- [ ] **Joint Submission** considered where the work is both pivotal and long

> `[REQUIREMENT]` Do not carry format assumptions between journals: End Matter
> exists only at PRL, Letters are 3750 words there but 4500 words at the
> specialist journals, and Review limits range from 6000 to 50,000 words across
> the portfolio.

## 7. Response to referees

Structure:

1. A brief opening thanking referees and summarizing the main changes.
2. Point-by-point: quote each comment, then respond, then quote the revised text
   with its new location.
3. Group related comments; do not pad.

Rules:
- Answer every point, including ones you decline — and say why you decline,
  with reasoning rather than reassertion.
- Distinguish changes made, changes made differently, and changes refused.
- Where a referee is mistaken, show why with evidence, courteously.
- Never claim a change you did not make.
- For **PRX Life**, note that referees see each other's reports (collaborative
  review) — plan the response as one coherent document rather than three
  independent rebuttals.

## 8. Appeals `[OFFICIAL]`

APS has a formal appeals process; editorial boards adjudicate formal appeals.
Fetch `journals.aps.org/authors/editorial-policies-editorial-oversight` and the
journal's own policy page before advising on an appeal, and never characterize
the odds.

Before appealing, ask: is there a substantive error in the review, or only
disagreement about significance? Transfer to a better-matched journal is usually
the faster path for the latter — and the portfolio supports transfers.

## 9. Output format

**Target journal / article type / section:** …
**Criteria justification:** *(drafted to the journal's current requirement)*
**Cover letter:** *(full draft)*
**Checklist status:** items complete / outstanding
**Required fetches performed:** URLs and what was confirmed
**Mathematical placement:** essential / supporting / derivational split, and
whether it fits the chosen article type
**Format plan:** article type, verified limit, container assignments, figure
count and rationale — each labeled [REQUIREMENT] / [CONVENTION] / [STRATEGY]
**Risks flagged:** anything the author should decide before submitting

## 10. Rules

1. Fetch author-page requirements every time; never assert limits from memory.
2. Do not draft claims the manuscript does not support.
3. Never state or imply a likely decision.
4. Keep the cover letter to one page.
5. Flag missing statements rather than inventing content for them.

## 11. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| APS Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Authorship, ethics, submissions, appeals |
| Submit a Manuscript | https://authors.aps.org/Submissions/ | Official | 2026-08-19 | Submission portal |
| Journal author pages | https://journals.aps.org/<code>/authors | Official | 2026-08-19 | Article types, limits, required components (fetch each time) |
