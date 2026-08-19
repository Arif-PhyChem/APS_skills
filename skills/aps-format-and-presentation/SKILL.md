---
name: aps-format-and-presentation
description: Determine how a manuscript should be built for a specific APS journal — length and article type, figure strategy and compression, main-text vs Supplemental Material, section structure, and narrative style. Load alongside any journal skill when advising on manuscript construction or revision.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
requires: [aps-common]
companion_skills: [aps-mathematical-presentation]
---

# APS Format and Presentation

Load `aps-common` and the target journal's skill. For equation-driven work also
load `aps-mathematical-presentation`; the two skills are designed to be used
together and share the essential/supporting/derivational hierarchy.

> **Physical Review journals do not share one manuscript format.** Length limits,
> article types, appendix conventions, and presentation norms differ materially
> between titles — and in at least one case (End Matter) a feature exists at one
> journal and explicitly does not exist at its siblings. Never generalize a
> format fact from one *Physical Review* journal to another.

## 1. The three labels (mandatory)

Presentation advice fails when convention is passed off as rule. Label every
statement about manuscript construction as exactly one of:

| Label | Meaning | Source |
|---|---|---|
| **[REQUIREMENT]** | An official APS rule. Binding. | Must cite a `journals.aps.org` URL |
| **[CONVENTION]** | A strong, observable practice at this journal, not a rule. | Inferred from published papers or journal guidance |
| **[STRATEGY]** | This system's editorial recommendation. | Judgment |

Mapping to the provenance tags used elsewhere in this system: every
**[REQUIREMENT]** is also `[OFFICIAL]`; **[CONVENTION]** is `[INFERENCE]`;
**[STRATEGY]** is `[HEURISTIC]`.

**Rule:** never convert a convention into a requirement, and never present a
strategy as either. When a manuscript is at risk of being reshaped, the author
is entitled to know which constraints are real.

## 2. Researching the format (what to fetch)

Determine from current official sources, where applicable:

- article types available at **this** journal, and length limits per type;
- what counts against the limit and what does not;
- title and abstract requirements;
- section structure expectations;
- figure and table requirements (resolution, color, captions, print vs online);
- Supplemental Material policy, deposit mechanics, and how to cite it;
- appendix conventions (they differ by journal);
- reference style, including whether titles in references are encouraged;
- data and code availability requirements;
- templates (REVTeX and journal-specific class options);
- special restrictions or additional required components at submission.

Primary pages: `/<code>/authors`, `/<code>/authors/editorial-policies-practices`,
and the portfolio-wide policy pages.

> **Do not invent numerical limits.** If a limit is not stated, write
> `No explicit limit stated in official sources` rather than estimating one.
> Verified numbers age: re-check any figure older than the skill's
> `refresh_interval_days` before relying on it in author advice.

## 3. Figure strategy

**Do not assume more figures make a stronger paper.** Derive the figure count
from the scientific narrative, never from a target number.

Work through:

1. **What must the reader see to be convinced?** List the decisive evidence.
   Each item is a candidate panel, not necessarily a figure.
2. **What does each existing figure prove?** A figure that proves nothing the
   text does not already establish is a candidate for removal or for
   Supplemental Material.
3. **Is any figure doing two jobs?** Split it. Is any pair of figures doing one
   job? Combine them.
4. **Does a figure exist for every central claim?** An unillustrated central
   claim is usually a weakness; a figure with no claim attached is usually
   padding.

For short-format work, evaluate explicitly whether the central result can be
communicated with a **very small number of main-text figures** — potentially a
single carefully designed multi-panel figure, when it can carry:

1. the central physical problem;
2. the key result;
3. the decisive evidence;
4. the main implication.

A larger number of figures is right when the scientific argument genuinely
requires them — several independent experimental probes, a theory-plus-experiment
comparison plus a phase diagram, a method validated across distinct systems.

> **[STRATEGY]** For PRL-like manuscripts:
> *one central scientific message → one compact narrative → minimal essential figures.*

**Never** state that any APS journal formally requires a particular number of
figures, and never impose an arbitrary figure limit. Where a journal states no
figure limit, say so — the operative constraint is usually the length limit,
which figures consume.

## 4. Figure compression

When a journal favors concise presentation, consider combining related figures
into a coherent multi-panel figure. Test before recommending it:

- **Unity** — do the panels tell one story with a single takeaway? If a reader
  cannot state the figure's message in one sentence, it is not one figure.
- **Redundancy** — do two panels make the same point in different coordinates?
  Keep the more decisive one.
- **Relegation** — is a panel supporting rather than decisive? Move it to
  Supplemental Material.
- **Self-sufficiency** — can the combined figure be read from its caption and
  labels without a paragraph of setup?

> **Do not combine unrelated results merely to reduce the figure count.** A
> multi-panel figure whose panels share no argument is harder to read than the
> separate figures were, and referees say so.

Practical compression that preserves content: shared axes and one legend;
insets for limits and zooms; a schematic panel replacing a paragraph of setup;
consistent color mapping across panels so the reader learns the encoding once.

## 5. Main text vs Supplemental Material

**Main text** — the central scientific question; essential methodology; decisive
equations; key results; the strongest evidence; physical interpretation; the
central conclusion.

**Supplemental Material** — extended derivations; additional validation;
secondary datasets; robustness and convergence tests; additional figures;
implementation details; supplementary methodological analysis.

> **[REQUIREMENT]** APS defines Supplemental Material as information that is
> **not essential to understanding an article's main results** (stated on the
> PRL author page; verify the equivalent wording for other journals). This makes
> the governing rule official rather than merely advisable:

**Never move material to the supplement if it is needed to understand or
evaluate the central claim.** Doing so does not shorten the paper; it makes the
paper incomplete and moves the evidence out of review's line of sight.

Decision test for any block of content: remove it and read the paper. If a
central claim becomes unclear, unsupported, or unverifiable, it is main text —
whatever the length pressure.

If the essential content does not fit the article type, the finding is a
**placement** finding: change article type, use the journal's appendix
mechanism, consider a joint submission (see §7), or target a full-length venue.

`[REQUIREMENT]` Supplemental Material is typically deposited as a single set of
files with its own URL, must be cited in the paper's reference list with a brief
description of its content, and references cited within it are normally listed
in the main text's reference section. Fetch the target journal's exact wording
and mechanics before finalizing.

## 6. Appendices and journal-specific containers

Appendix conventions are **not** uniform across the portfolio, and this is a
common source of error when moving a manuscript between journals.

- `[REQUIREMENT]` *Physical Review Letters* provides **End Matter** — up to two
  pages of appendices or other content that specialists will want or need to
  read, appearing after the references and **not counting against the core
  length limit** (PRL author page, accessed 2026-08-19).
- `[REQUIREMENT]` **Letters in other *Physical Review* journals do not have End
  Matter**; they use Appendixes instead (stated on the PRL author page).

So: a three-tier split (main text / End Matter / Supplemental Material) is
available at PRL and must not be assumed elsewhere. Always confirm which
containers the target journal offers before planning where content goes.

## 7. Joint submissions

`[REQUIREMENT]` APS explicitly permits **Joint Submissions** — related or
complementary papers submitted to the same or different *Physical Review*
journals, for example a Letter to PRL plus a longer Regular Article to a
specialist journal. The longer article must present considerably more, or
different, information and lead to a substantially improved understanding;
some duplication of figures, tables, and text is often appropriate but should be
limited and properly referenced (PRL author page, accessed 2026-08-19).

> **[STRATEGY]** This is the principled resolution for work that is genuinely
> pivotal *and* genuinely needs length — rather than mutilating one manuscript
> to fit a short format, or padding a short result to fill a long one.

## 8. Narrative style by format

Translate the journal's format into writing advice.

### Short-format (PRL; Letters at specialist journals)

- State the problem immediately — no extended survey.
- Reach the central result early; the reader should know it within the first
  column.
- Methodology: minimal but sufficient; detail goes to appendix/End Matter/SM.
- Compact figures; every panel earning its space.
- Strong physical interpretation — compression must not remove meaning.
- Concise conclusion pointing outward to consequences.

### Full-length research article

- Extended theoretical development, with derivations followed through.
- Detailed methodology sufficient for reproduction.
- Systematic validation, including negative and boundary cases.
- Multiple related results assembled into one authoritative treatment.
- Broader discussion, limitations, and relation to the literature.

### Review or tutorial (RMP; Review Articles at specialist journals)

- Unifying notation established early and held throughout.
- Critical judgment, not enumeration.
- Historical development where it explains current questions.
- Forward-looking open problems with real content.

### Interdisciplinary venues (PRResearch, PRX titles, APS Open Science)

- Define terms for every audience that will referee the paper.
- Do not assume one subfield's conventions or notation.
- Make the connection to physics explicit and load-bearing.

## 9. The governing question

Ask this, and not a numerical question:

> **What is the minimum amount of main-text material needed to communicate and
> convincingly support the central scientific contribution for this journal's
> readership?**

Not: *how many figures or equations should the paper have?*

`[STRATEGY]` For highly selective short-format journals, a compact manuscript
with one exceptionally informative figure may be stronger than a longer one
containing many individually correct but nonessential figures. "Minimum" is
bounded by *convincingly support* — compression that removes the evidence, the
validity conditions, or the interpretation is not compression.

## 10. Output — Presentation profile

Report using these fields; each journal skill carries its own calibrated version:

**Article format:** short / full-length / flexible / review
**Available length containers:** main text, appendix, End Matter, Supplemental Material — as applicable to this journal
**Stated length limits:** the official numbers, with accessed date — or `No explicit limit stated`
**Typical mathematical density:** Low / Moderate / High
**Recommended main-text figure strategy:** derived from the argument, with the official figure limit (or its absence) stated
**Supplementary-material role:** what belongs there at this journal
**Preferred narrative style:** how papers here are written
**Recommended manuscript compactness:** Low / Moderate / High
**Presentation priority:** what the author should emphasize
**Label audit:** which of the above are [REQUIREMENT] vs [CONVENTION] vs [STRATEGY]

## 11. Rules

1. Never generalize a format fact across *Physical Review* journals.
2. Never invent a numerical limit; state its absence explicitly when absent.
3. Never state a figure-count requirement; no APS journal is known to impose one.
4. Never move essential content to Supplemental Material to meet a length limit.
5. Never combine unrelated figures to reduce a count.
6. Always label [REQUIREMENT] / [CONVENTION] / [STRATEGY].
7. Always fetch the target journal's author page before giving construction
   advice; verified numbers in this system carry an accessed date and expire.

## 12. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| PRL Information for Authors | https://journals.aps.org/prl/authors | Official | 2026-08-19 | Length limits, End Matter, Supplemental Material definition and mechanics, Joint Submissions, title/abstract guidance |
| APS Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Portfolio-wide policy |
| Journal author pages | https://journals.aps.org/<code>/authors | Official | 2026-08-19 | Per-journal format (fetch at use time) |
| Tips for Authors | https://journals.aps.org/authors/tips-authors-physical-review-physical-review-letters | Official | 2026-08-19 | Presentation guidance (fetch for current wording) |

**Unknown — not stated in official sources:** any figure-count limit; any
required section structure for research articles.
