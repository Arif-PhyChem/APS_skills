---
name: aps-reference-format
description: Build, audit, or fix an APS/Physical Review manuscript's reference list — numbering and citation mechanics, what must be listed, author-count rules, e-print and unpublished-work handling, and the ethical referencing standard APS states explicitly (comprehensiveness, no self-citation inflation). Load alongside any journal skill when reviewing, drafting, or formatting references.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-21
last_verified: 2026-08-21
refresh_interval_days: 90
requires: [aps-common]
---

# APS Reference Format

Load `aps-common` alongside this skill. This skill is **portfolio-wide** — APS
reference mechanics and referencing ethics are stated once, centrally, and
apply the same way at every *Physical Review* journal. Where a journal adds
something on top (PRL's titles-in-references convention, for instance), that
journal's own skill says so and points back here.

Tags: `[OFFICIAL]` (stated by APS) / `[INFERENCE]` (editorial reading) /
`[HEURISTIC]` (this system's recommendation) — the same convention used
throughout this repository.

## 1. Purpose

Get a manuscript's reference list mechanically correct and ethically sound
before it reaches a referee — numbering, completeness, author-count handling,
and the substantive referencing standard APS states as policy, not just style.

## 2. Mechanics `[OFFICIAL]`

Verified against `journals.aps.org/authors/style-basics` (2026-08-20):

- **Combine** references (citations of other work) and endnotes (subsidiary
  remarks) in a **single list** at the end of the paper.
- **Number items consecutively** in the order first cited.
- **Cite inline** with numerals in square brackets, e.g. `[3]`, at every point
  of use — including citations inside figure and table captions.
- **All sources appear in the reference list**, including URLs — a URL should
  **not** appear in the body of the paper.
- Provide **enough information to locate** items not in the published
  literature — internal reports, unpublished work, etc.
- **Do not cite e-prints in place of primary references** (peer-reviewed
  journal papers) — an e-print supplements, it does not substitute.
- **Avoid citing classified or restricted-circulation documents.**
- **Check bibliographic accuracy.** Incorrect or incomplete data (missing
  author, wrong volume or page) breaks the reference-linking system APS builds
  from the list.

### Author-count rule — a genuine conflict between two APS pages `[OFFICIAL]`, flagged not resolved

Three APS-hosted sources give **three different rules**, and this skill will
not silently pick one:

| Source | Accessed | Says |
|---|---|---|
| `authors/style-basics` | 2024-08-15 page, verified 2026-08-20 | List all authors up to **ten**; for more than ten, list up to **20 names** then *et al.* |
| `authors/references-physical-review-physical-review-letters` | 2012-04-11 page, verified 2026-08-21 | *"The use of et al. is discouraged... The names of all authors should be given... If the number of authors exceeds ten, then the first ten author names may be listed and then et al."* An exception applies to alphabetic author lists and collaborations, where only the first name precedes *et al.*, followed by the collaboration name. |
| `revtex/revtex-faq` (2019-01-11) | verified 2026-08-21 | *"APS editors prefer full author lists be used for references with 15 or less authors. For longer lists, use the phrase 'and others' in place of the authors you want to omit."* Also notes current REVTeX BibTeX styles (4.1/4.2) **no longer truncate** author lists past ten the way REVTeX 4's did. |

`[HEURISTIC]` `style-basics` carries the most recent page-publication date and
sits on the main author-facing domain, so treat it as the default: **list all
authors up to ten; beyond ten, up to twenty names then *et al.*** But state the
conflict rather than hiding it whenever author-count handling is
submission-critical, and where the manuscript has 11–20 authors, prefer
whichever rule the *target journal's own recent published papers* actually
follow — that is more reliable than any of these three pages in isolation.
**Never assert a single author-count rule as settled APS policy; this is
exactly the kind of drift the refresh protocol exists to catch.**

### Citations in the abstract `[OFFICIAL]`

*Physical Review* and *Physical Review Letters* explicitly forbid numbered
citations in the abstract: **"References in the abstract must be written out
in full within square brackets and never numbered."** — e.g. `[J. Smith and
K. Lee, Phys. Rev. B 100, 054321 (2019)]` inline, not `[3]`. This is a common,
easy-to-miss defect; check it specifically.

### Byline footnotes — PRB is the exception, again

- **All journals except PRB:** byline footnotes (author names, addresses)
  appear under a single rule at the **bottom of the first page**. Subsidiary
  in-text footnotes are numbered consecutively and placed at the bottom of the
  page where cited.
- **PRB specifically:** byline footnotes appear **at the top of the reference
  section**, not the bottom of the first page, and should be limited to what
  is necessary to locate the author. Subsidiary remarks are handled as
  numbered references or incorporated directly into the text — **not** as
  page-bottom footnotes.

`[HEURISTIC]` This is the same pattern as PRL's End Matter and PRC's
structured abstracts: a real, journal-specific mechanical difference. Never
carry PRB's footnote placement to another journal, or vice versa.

## 2b. Format by source type `[OFFICIAL]`

Verified against `journals.aps.org/authors/references-physical-review-physical-review-letters`
(the canonical APS reference-format page, dated 2012-04-11 on the APS site,
verified live 2026-08-21). APS states these as general forms, not rigid
templates — "authors should be guided by any recent publication in the
relevant *Physical Review* journal and the *Physical Review Style and
Notation Guide*" for edge cases.

| Source type | Elements, in order | Notes |
|---|---|---|
| **Journal article** | Authors, journal name (abbreviated), volume number **(bold)**, page or article number, year **(in parentheses)** | Titles and page *ranges* are generally not printed. Multiple references in one entry are separated by a **semicolon**; *ibid.* may be used for a repeated source within the same entry. |
| **Conference proceedings** | Authors, exact title, editors, publisher, city of publication, year — **last three in parentheses**; edition/volume/page follow the parenthesis if provided | |
| **Books** | Authors, exact title, editors (if any), publisher, city of publication, year — **last three in parentheses**; edition/volume/page follow if provided | A book in press: append **"(in press)."** |
| **Reports** | Authors, institution, report number, year | Include the report's title if provided, especially when no report number exists. |
| **Theses** | Author, degree, institution, year | Do **not** add "(unpublished)" to a thesis. |
| **E-prints** | e.g. `authors, arXiv:1204.1234.` | Do not add "e-print," "unpublished," or a year. If accepted for publication, append `[journal name (to be published)]`. |
| **Accepted but not yet published** | Cite as normal, append **"(to be published)"** | Applies to journal articles and conference proceedings alike. |
| **Not yet accepted** | **"(unpublished)"** | For work in preparation, to be submitted, lectures, or invited talks: `authors (unpublished)`. |
| **Private communication** | `authors (private communication)` | For information not available in published or report form. |

`[HEURISTIC]` When auditing a reference list against these forms, check
specifically for: page *ranges* left in (should generally be a single page or
article number); titles present where the journal doesn't ask for them (except
where an author has opted into PRL's titles-in-references convention, §7);
e-prints carrying a spurious "(unpublished)" or year; and "(to be published)"
used for something not actually accepted yet — that belongs under
"(unpublished)" instead.

## 3. Referencing as an editorial standard, not just formatting `[OFFICIAL]`

Verified against `journals.aps.org/authors/editorial-policies-submissions`
(2026-08-20) — APS states these as submission expectations, not stylistic
preference:

- Include proper references to pertinent earlier work and **credit significant
  contributions by other researchers.**
- Ensure references are **comprehensive and up to date at submission** — and
  add new references for relevant work published **during review**.
- Citable source types are broad: e-print archives, books, published
  conference proceedings, internal reports, or results reported orally at
  meetings.
- The reference list should **represent the field**, avoiding favoritism
  toward specific research groups, regions, or institutions.
- **Avoid citation-count inflation** — excessive self-referencing, or
  excessive references to the journal reviewing the paper.

> `[HEURISTIC]` Treat the last two bullets as an explicit **referee-facing
> check**, not background policy: a reference list skewed toward the authors'
> own prior work, one research group, or one country is a documented APS
> concern, and a referee is entitled to flag it. When auditing a manuscript,
> compute (informally) what fraction of citations are self-citations and
> whether the geographic/institutional spread looks representative of the
> field, and say so if it looks skewed.

## 4. Format and template `[OFFICIAL]`

- APS's LaTeX class is **REVTeX**; the preferred submission format is REVTeX,
  with LaTeX and MS Word also accepted. PDF/PostScript submission may delay
  production.
- Template files (`apstemplate.tex`) are distributed from the REVTeX Home Page
  (`journals.aps.org/revtex`), in `doc/latex/revtex/sample`.
- **For REVTeX/LaTeX submissions, run BibTeX before submitting**, and
  `\input` (or paste) the resulting `.bbl` file into the reference section —
  APS explicitly asks for the compiled bibliography, not a live `\bibliography`
  command left unresolved.
- `[HEURISTIC]` Journal names are conventionally abbreviated in the compiled
  reference list (e.g. *Phys. Rev. B*, *Phys. Rev. Lett.*) — this is what the
  standard APS BibTeX styles (`apsrev4-2.bst` and similar, distributed with
  REVTeX) produce. Confirm the current style file and abbreviation list from
  the REVTeX Home Page rather than hand-abbreviating.
- `[OFFICIAL]` REVTeX selects the correct BibTeX style automatically from the
  journal class option. Per the REVTeX FAQ (2019-01-11, verified live
  2026-08-21): `apsrev4-2.bst` is the **numeric** citation style used by
  **most APS journals**; `apsrmp4-2.bst` is a **separate author/year style
  file for RMP**. `[HEURISTIC]` **Not independently confirmed on a
  `journals.aps.org` page in this session** — third-party BibTeX
  documentation and the CTAN-hosted *APS Author Guide for REVTeX 4.2* both
  describe `apsrmp4-2.bst` as author/year, which would mean **Reviews of
  Modern Physics cites differently from every other journal in the
  portfolio**. Before advising an author preparing an RMP manuscript, confirm
  this against a recent published RMP article or `journals.aps.org/revtex`
  directly — do not assume numeric citation for RMP, and do not assert
  author/year as certain either.
- `[OFFICIAL]` To combine multiple works into one bibliography entry with
  BibTeX, prepend `*` to the key: `\cite{feynman,*bohr}` — REVTeX renders them
  as one entry with a **semicolon** between, matching the "separate multiple
  references by a semicolon" convention in §2b.
- `[OFFICIAL]` Article titles appear in the bibliography only when the
  `longbibliography` class option is used — this is the mechanism behind
  PRL's titles-in-references convention (§7); it is not the REVTeX default.
- `[OFFICIAL]` REVTeX applies the correct **footnote style per journal**
  automatically (§2's PRB exception), overridable with the `footinbib` /
  `nofootinbib` class options.

## 5. Reference list vs. Supplemental Material `[OFFICIAL]`

- All citations appearing **anywhere** in the paper — main text, figure
  captions, table footnotes, and **Supplemental Material** — belong in the
  **one** reference list in the main text. Supplemental Material does not carry
  its own separate bibliography.
- Supplemental Material itself must be **cited** in the paper's reference list
  (see `aps-format-and-presentation` §5 for the citation mechanics and the
  Supplemental Material definition itself).

## 6. Endnotes

APS combines references and endnotes (subsidiary remarks — asides, brief
clarifications) into the **same** numbered list. `[HEURISTIC]` Do not create a
separate footnote-numbering scheme; an endnote gets the next sequential
reference number at its point of first use, exactly like a citation.

## 7. Journal-specific additions (not portfolio-wide — check the journal skill)

- `[OFFICIAL]` **PRL** strongly encourages **titles in references**, as an aid
  to the reader and to improve online-search accuracy — and if an author
  elects to use titles, they should be used **in all** references, not some.
  This convention is **PRL-specific**; other journals do not state it. See
  `skills/journals/prl/SKILL.md`.
- `[OFFICIAL]` **PRL** also permits **Endnotes** as brief asides within the
  reference section (consistent with §6 above, stated explicitly for PRL).
- `[OFFICIAL]` **PRC** supports **structured abstracts**; an editorial example
  and REVTeX instructions are available — not a reference-format matter per se,
  but adjacent enough to check when preparing a PRC submission.

> `[HEURISTIC]` Because this one convention (titles in references) differs
> between journals, never carry a reference-formatting habit from one
> *Physical Review* journal to another without checking that journal's own
> author page — the same discipline `aps-format-and-presentation` applies to
> length limits applies here.

## 8. Common defects to audit for

- Numbering that does not match order of first citation.
- A cited item (including in a caption) missing from the list, or a listed
  item never cited.
- A URL appearing in the body text instead of the reference list.
- An e-print cited as if it were the primary (peer-reviewed) reference when a
  published version exists.
- Incomplete bibliographic data — missing author, wrong volume/page/year —
  that would break reference linking.
- Author lists truncated inconsistently with the target journal's actual
  practice — see the flagged conflict in §2; check recent papers in that
  journal rather than assuming a single rule.
- **Numbered citations in the abstract** — must instead be written out in full
  within square brackets (§2).
- Byline/subsidiary footnotes placed at the wrong location for the journal —
  bottom-of-first-page everywhere except PRB, top-of-reference-section at PRB.
- Page *ranges* left in a journal-article reference where a single page or
  article number is expected; a title present where the journal doesn't
  encourage one; "(to be published)" used for work not actually accepted.
- A skewed reference list — heavy self-citation, one group or region
  dominating, or no engagement with the nearest competing work.
- Reference list not current — a relevant paper published after the original
  submission and not added before the current revision.
- A separate, informal bibliography for Supplemental Material instead of one
  unified list.
- Titles-in-references used inconsistently at a journal (PRL) that requires
  all-or-nothing once elected.

## 9. Output format

**Mechanical compliance:** numbering / inline citation / author-count
handling (with the §2 conflict noted if 11–20 authors) / URL placement /
abstract-citation rule / footnote placement — pass or list defects.

**Source-type formatting:** each reference checked against §2b's form for its
type (journal article / proceedings / book / report / thesis / e-print /
unpublished / private communication).

**Completeness:** any citation (main text, caption, or SM) missing from the
list; any listed item never cited.

**Currency:** is the reference list up to date as of the current submission or
revision?

**Representativeness:** `[HEURISTIC]` self-citation share, and whether the
field's competing work and geographic/institutional spread look represented.

**Format/template:** REVTeX/BibTeX status — `.bbl` resolved and included, or
outstanding.

**Journal-specific conventions checked:** e.g. PRL titles-in-references,
applied consistently or not.

**Fixes recommended:** concrete, ordered by effort-to-benefit.

## 10. Rules

1. Never invent a citation-count threshold, a self-citation percentage limit,
   or a formal rejection criterion — APS states the *principle*
   (representativeness, no inflation), not a numeric bar. Treat any such
   number as `[HEURISTIC]` guidance, never as policy.
2. Never assert a journal-specific reference convention (like PRL's
   titles-in-references) as portfolio-wide, and never assert a portfolio-wide
   mechanic as journal-specific.
3. Never fabricate a BibTeX style name or abbreviation list — point to the
   REVTeX Home Page for the current one.
4. Treat comprehensiveness and non-favoritism as editorial-quality findings a
   referee could raise, not merely formatting nitpicks.
5. **Never silently resolve a conflict between APS-hosted pages.** The
   author-count rule (§2) has three different statements across three APS
   sources of different ages; state the conflict and the reasoning for the
   default chosen, every time it is submission-critical.
6. **Never assert RMP's citation style as settled** without confirming against
   a recent RMP paper or `journals.aps.org/revtex` directly — the author/year
   claim in §4 is not yet confirmed on an APS-hosted page in this skill.

## 11. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| Style Basics — References and subsidiary remarks | https://journals.aps.org/authors/style-basics | Official | 2026-08-20 | Numbering, inline citation, author-count (one of three conflicting statements), e-print, URL placement rules |
| References in Physical Review and Physical Review Letters | https://journals.aps.org/authors/references-physical-review-physical-review-letters | Official (2012-04-11 page, verified live) | 2026-08-21 | Canonical per-source-type formats (§2b), abstract-citation rule, PRB byline-footnote exception, author-count (second conflicting statement) |
| Editorial Policies — Submissions: References to Other Work | https://journals.aps.org/authors/editorial-policies-submissions | Official | 2026-08-20 | Referencing as editorial standard: comprehensiveness, representativeness, no inflation |
| REVTeX Home Page | https://journals.aps.org/revtex | Official | 2026-08-20 | Templates, BibTeX styles (fetch for current file names) |
| REVTeX 4 Frequently Asked Questions | https://journals.aps.org/revtex/revtex-faq | Official (2019-01-11 page, verified live) | 2026-08-21 | `\cite{a,*b}` combining, `longbibliography` option, `footinbib`/`nofootinbib`, author-count (third conflicting statement), numeric-vs-author/year `.bst` files |
| Tips for Authors | https://journals.aps.org/authors/tips-authors-physical-review-physical-review-letters | Official | 2026-08-20 | REVTeX/BibTeX `.bbl` submission mechanics |
| PRL Information for Authors | https://journals.aps.org/prl/authors | Official | 2026-08-20 | PRL-specific titles-in-references convention |

**Unknown — not stated in official sources on this domain:** the settled
current author-count rule (three APS pages disagree — see §2); whether RMP's
citation style is genuinely author/year (stated only in non-`journals.aps.org`
documentation); any numeric limit on reference-list length; any formal
self-citation threshold.
