---
name: aps-common
description: Shared APS/Physical Review policies, house conventions, and vocabulary. Load once alongside any journal-specific APS skill; never duplicate this content into a journal skill.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
---

# APS Common — Portfolio-Wide Layer

## 1. Purpose

This skill holds everything true across the whole *Physical Review* portfolio,
so that individual journal skills contain only what distinguishes their
journal. Load it once per session. If a journal skill contradicts this file,
the journal skill wins for that journal.

## 2. The portfolio (verified 2026-08-19)

Nineteen author-facing titles are listed on the APS publishing-guidelines page.

| Code | Journal | Domain |
|---|---|---|
| `prl` | Physical Review Letters | All physics — short, high-impact |
| `prx` | Physical Review X | All physics — highly selective, gold OA |
| `prresearch` | Physical Review Research | All physics — broad, gold OA |
| `pra` | Physical Review A | Atomic, molecular, optical; quantum science |
| `prb` | Physical Review B | Condensed matter and materials physics |
| `prc` | Physical Review C | Nuclear physics |
| `prd` | Physical Review D | Particles, fields, gravitation, cosmology |
| `pre` | Physical Review E | Statistical, nonlinear, biological, soft matter, fluids, plasma, computational |
| `prmaterials` | Physical Review Materials | Multidisciplinary materials research |
| `prapplied` | Physical Review Applied | Applied physics and device science |
| `prfluids` | Physical Review Fluids | Fluid dynamics |
| `prab` | Physical Review Accelerators and Beams | Accelerator and beam physics |
| `prper` | Physical Review Physics Education Research | Physics education research |
| `prxquantum` | PRX Quantum | Quantum information science and technology |
| `prxenergy` | PRX Energy | Energy science and technology |
| `prxlife` | PRX Life | Physics of living systems |
| `prxintelligence` | PRX Intelligence | AI/ML and the physical sciences |
| `apsos` | APS Open Science | Portfolio open-science venue |
| `rmp` | Reviews of Modern Physics | Invited reviews |

> `[HEURISTIC]` The existence of *PRX Intelligence* changes the neighbor
> analysis for every other journal in the portfolio. Any manuscript whose
> central contribution is the AI/ML method itself must be checked against it
> before defaulting to a domain journal.

## 3. Common editorial policies `[OFFICIAL]`

All APS journals follow one set of Editorial Policies and Practices, published
at `journals.aps.org/authors/editorial-policies`, organized as:

| Area | URL suffix |
|---|---|
| Editorial oversight and decision making | `-editorial-oversight` |
| Authorship | `-authorship` |
| Submissions, resubmissions, and transfers | `-submissions` |
| Peer review | `-peer-review` |
| Ethics and research integrity | `-ethics` |
| Post publication | `-post-publication` |
| Open access and publication rights | `-open-access` |

**Agent rule.** When a task turns on the precise wording of any of these
(authorship disputes, AI-tool disclosure, dual submission, appeals, corrections,
transfer mechanics), fetch the relevant page and quote it. Do not answer from
this summary and do not answer from model memory — these pages change.

## 4. House conventions verified across journals `[OFFICIAL]`

- **Submission portal:** `authors.aps.org/Submissions/`.
- **Article identification:** journals publish electronically one article at a
  time; articles carry a volume number and a six-digit article number, e.g.
  `Journal 1, XXXXXX (2020)` — not page ranges.
- **Editorial teams** are professional Ph.D. scientists; decisions are made
  against the journal's stated acceptance criteria.
- **Editorial Boards** are appointed by the Executive Editor, serve three-year
  terms, may advise at any review stage, and adjudicate formal appeals.
- **Accelerated review** exists at editors' discretion for a small number of
  particularly important or groundbreaking manuscripts (stated on the *about*
  pages of PRB, PRC, PRE, PRMaterials, and siblings).
- **Transfers** between *Physical Review* journals are a supported route; the
  journals explicitly coordinate to serve new subspecialties.

## 4b. Format facts that hold portfolio-wide `[OFFICIAL]` *(verified 2026-08-19)*

Format is **not** uniform across the portfolio, but these patterns recur. Always
confirm against the target journal's author page; never generalize a number.

- **Full-length research articles carry no length limit** at PRA, PRB, PRC, PRD,
  PRE, PRFluids, PRMaterials, PRApplied, PRAB, PRPER, PRResearch, PRX,
  PRX Quantum, PRX Energy, PRX Life, PRX Intelligence, and APS Open Science.
  Journals state that appropriate length depends on the information the article
  contains.
- **Letters are 4500 words** at PRA, PRB, PRC, PRD, PRE, PRFluids, PRMaterials,
  PRApplied, PRAB, PRResearch, and APS Open Science. **PRL's Letters are 3750
  words** — PRL is the exception, not the template.
- **Comments/Replies are 3500 words** at most journals; PRL is 750, PRC and
  PRX Life are 1500.
- **No APS journal examined states a figure-count limit.** The operative
  constraint is length, which figures consume. Never assert a figure requirement.
- **End Matter exists only at PRL** (up to two pages, outside the core limit).
  Letters at other *Physical Review* journals use Appendixes instead.
- **Supplemental Material** is officially defined as information *not essential
  to understanding an article's main results*, deposited as a single set with
  its own URL, cited in the reference list with a brief description.
- **Joint Submissions** are permitted across the portfolio — e.g. a PRL Letter
  plus a longer Regular Article elsewhere — provided the longer paper contains
  considerably more or different information and duplication is limited and
  referenced.

Review limits vary sharply and must never be generalized: 30,000 words at
PRMaterials, PRApplied, PRX Intelligence, and APS Open Science; **7000 at
PRX Energy**; 6000 at PRX Life; 20,000 for RMP Colloquia and **50,000 for RMP
Articles**; no limit at PRAB and PRPER.

## 5. Visibility mechanisms `[OFFICIAL]`

Relevant because they are what "editorial interest" concretely looks like:

- **Editors' Suggestions** — editor-selected papers, promoted on the journal
  site.
- **Featured in *Physics*** (`physics.aps.org`) — Synopsis, Focus, or Viewpoint
  coverage.
- **Tip Sheet** — weekly press promotion of press-worthy papers.
- **Structured abstracts** — supported at PRC (background, purpose, methods,
  results, conclusions).

> `[HEURISTIC]` "Would an editor plausibly send this to *Physics*?" is a
> serviceable proxy for breadth-of-interest when judging PRL/PRX-tier fit. It is
> a reasoning aid, not an APS criterion.

## 6. Open access `[OFFICIAL]`

- Hybrid titles allow an APC for immediate CC-BY 4.0 publication; PRX,
  PRResearch, PRX Quantum, PRX Energy, PRX Life, and PRX Intelligence are gold
  open access. Current APCs: `journals.aps.org/authors/apcs`.
- APS is a founding member of CHORUS.
- Automatic APC waivers for authors from lower-income countries across hybrid
  and gold titles.
- SCOAP³ applies to high-energy-physics articles in PRC and PRD posted to arXiv
  under a `hep` primary designation (PRC: since 1 January 2018).
- Free access at U.S. public libraries and high schools by application.

## 7. Vocabulary the agent must use precisely

| Term | Meaning |
|---|---|
| **Letter** | Short, length-restricted article of particular importance. Exists *inside* PRA/PRB/PRC/PRD/PRE/PRFluids/PRMaterials/PRApplied — distinct from a paper in *Physical Review Letters*. |
| **Article** | Full-length research paper. Most APS journals state a flexible approach to length. |
| **Acceptance criteria** | The journal's own stated bar. Every journal has one; they are not interchangeable. |
| **Section selection** | The subject section chosen at submission; each journal publishes a section-selection guideline page. |
| **Scope** | What the journal covers. Orthogonal to selectivity. |
| **Essential equation** | An equation required to understand the central argument or to read a figure. Belongs in the main text; never moved to the supplement for length. See `aps-mathematical-presentation`. |
| **Mathematical density** | How much of the argument the mathematics carries. Journal- and subfield-dependent; high is not automatically better. |

## 8. Non-negotiable reasoning rules

1. **Never fabricate** APS policy, acceptance rates, editorial thresholds,
   word limits, or rejection criteria. Unverifiable → write
   `Unknown — not stated in official sources`.
2. **Never imply acceptance.** Fit assessment is not a prediction of the
   editorial outcome.
3. **Scope ≠ selectivity.** In scope and not significant enough are compatible.
4. **Quality ≠ fit.** Excellent science can be a poor fit; modest science can
   be a good fit.
5. **Keywords are not evidence.** A manuscript is not PRB because it contains a
   material, nor PRX Quantum because it contains a qubit. Classify on the
   central contribution.
6. **Label every claim** `[OFFICIAL]`, `[INFERENCE]`, or `[HEURISTIC]`.
7. **Be conservative under thin evidence** and say so in the confidence line.
8. **Refresh before relying.** If a journal skill's `last_verified` is older
   than `refresh_interval_days`, re-fetch its sources or state the staleness.
9. **Equations are scientific content, not formatting.** For most *Physical
   Review* theory and computation, the mathematical formulation carries the
   contribution. Never recommend cutting an essential equation to meet a length
   limit, and never recommend adding equations to raise apparent rigor. Load
   `aps-mathematical-presentation` for equation-driven work; each journal skill
   carries its own calibration and says when to load it.
10. **Never invent notation for a manuscript.** Assessing authors against an
   equation they did not write is fabrication.
11. **Never generalize a format fact between journals.** Length limits, appendix
   mechanisms, and article types differ, and at least one feature (End Matter)
   exists at exactly one journal. Load `aps-format-and-presentation` and check
   the target journal's profile.
12. **Label presentation advice** `[REQUIREMENT]` (official rule),
   `[CONVENTION]` (strong practice), or `[STRATEGY]` (recommendation). Authors
   are entitled to know which constraints are real.
13. **Referencing is an editorial standard, not just a format rule.**
   Comprehensiveness, representativeness, and freedom from citation-count
   inflation are APS submission expectations, stated as policy — not merely
   style. Load `aps-reference-format` for the mechanics and the standard.

## 9. Fetching APS pages (practical) `[HEURISTIC]`

`journals.aps.org` is behind a bot challenge; naive fetches return HTTP 403 or
a "Just a moment..." page. Use a JS-rendering reader with an explicit wait:

```
curl -sS -m 150 -H "x-timeout: 25" "https://r.jina.ai/https://journals.aps.org/<code>/about"
```

A response under ~2 KB, or containing "Enable JavaScript and cookies to
continue", is a **failed fetch**. Retry; never fill the gap from memory.

## 10. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| Publishing Guidelines | https://journals.aps.org/authors | Official | 2026-08-19 | Portfolio title list |
| Scope of APS Journal Portfolio | https://journals.aps.org/scope | Official | 2026-08-19 | Subject coverage |
| Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Policy structure |
| Journal *about* pages (PRA/PRB/PRC/PRE/PRL/PRX/PRResearch/PRMaterials/PRApplied/PRFluids/PRX Quantum) | https://journals.aps.org/<code>/about | Official | 2026-08-19 | House conventions, OA, visibility |
