# APS Skills

**Agent-agnostic skills for deciding where a physics manuscript belongs in the
American Physical Society / *Physical Review* journal portfolio — and how to
build it for that journal.**

Not journal summaries. These are executable editorial reasoning frameworks: a
manuscript goes in, a defended journal recommendation with a fit classification,
neighbor comparison, and concrete positioning/format advice comes out.

Works with Claude, Codex, Gemini, DeepSeek, or any agent that can read a
Markdown file and (optionally) fetch a URL. No runtime, no dependencies, no
vendor lock-in.

> **Unofficial.** Not affiliated with, endorsed by, or reviewed by the American
> Physical Society. Journal-specific facts are verified against
> `journals.aps.org` as of the date stated in each skill and expire — see
> [Verification](#verification-and-staleness) below. Always confirm against the
> live APS pages before submitting.

---

## What's in here

| Skill | Answers |
|---|---|
| [`aps-journal-selector`](skills/aps-journal-selector/SKILL.md) | "Where should this manuscript go?" — extracts the contribution, shortlists candidates, ranks them, explains the margin |
| [`aps-manuscript-reviewer`](skills/aps-manuscript-reviewer/SKILL.md) | "Is this sound, and what will a referee object to?" — journal-independent |
| [`aps-mathematical-presentation`](skills/aps-mathematical-presentation/SKILL.md) | How equations should function as scientific content: what to put in the main text, what belongs in an appendix, how figures should test a formulation |
| [`aps-format-and-presentation`](skills/aps-format-and-presentation/SKILL.md) | Length, article type, figure strategy, Supplemental Material — with verified limits per journal |
| [`aps-submission-assistant`](skills/aps-submission-assistant/SKILL.md) | Cover letter, criteria-justification statement, submission checklist, response-to-referees |
| [`aps-common`](skills/aps-common/SKILL.md) | Portfolio-wide policies, vocabulary, and rules every other skill assumes |
| [`skills/journals/*`](skills/journals/) | One skill per journal — scope, official acceptance criteria, neighbor comparisons, fit classification, verified length limits |

**19 journals covered:** PRL, PRX, PRResearch, PRA, PRB, PRC, PRD, PRE,
PRMaterials, PRApplied, PRFluids, PRAB, PRPER, PRX Quantum, PRX Energy, PRX
Life, PRX Intelligence, RMP, and APS Open Science — including the two most
people's mental model of the portfolio is missing (**PRX Intelligence**, the
AI/ML-for-science title, and **APS Open Science**, which has no significance
criterion at all).

## Why this exists

Journal selection is usually done by keyword-matching a manuscript's topic
against a journal's scope page. That gets the easy cases right and the
interesting ones wrong: scope is not selectivity, and a manuscript's scientific
*quality* is not the same question as whether it's the right *fit*. A brilliant
condensed-matter paper can be a poor fit for a broad-audience journal; a modest
paper can be exactly right for a specialist one.

These skills instead encode each journal's actual editorial positioning —
its stated acceptance criteria, what distinguishes it from its nearest
neighbors, and what a manuscript needs to look like to be well-positioned there
— and force every claim to declare its source:

- `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]` — is this what APS states, a
  reasonable editorial reading of it, or this system's own decision rule?
- `[REQUIREMENT]` / `[CONVENTION]` / `[STRATEGY]` — for presentation advice, is
  this a binding rule, an observed norm, or a recommendation?

Nothing here predicts whether a manuscript will be accepted. Fit and quality are
reported as separate, explicit judgments.

## Quick start

Point any capable coding/reasoning agent at this repo and ask it to follow
[`AGENTS.md`](AGENTS.md). For example, with Claude Code, Codex CLI, or similar:

```
Read AGENTS.md in this repo, then load skills/aps-common/SKILL.md and
skills/aps-journal-selector/SKILL.md. Evaluate the attached manuscript
and recommend an APS journal.
```

```
Read skills/aps-common/SKILL.md and skills/journals/prb/SKILL.md.
Is this manuscript a good fit for Physical Review B? [paste abstract]
```

```
Follow generators/journal-skill-generator.md.
TARGET JOURNAL: PRX Quantum
```

There's nothing to install — clone or download the repo, then point your agent
at the files.

## How it fits together

```
Manuscript
    │
    ▼
aps-manuscript-reviewer ──── is it sound? what is the contribution?
    │
    ▼
aps-journal-selector ─────── extract profile → routing gates → shortlist
    │
    ├── loads 2–5 journal skills on demand (not all 19)
    ├── + aps-mathematical-presentation, if equation-driven
    ├── + aps-format-and-presentation, when building or revising
    │
    ▼
Ranked recommendation ─────── fit class, why #1 beats #2, editorial risks
    │
    ▼
aps-submission-assistant ─── cover letter, criteria statement, checklist
```

Every skill is a plain Markdown file with YAML frontmatter (`name`,
`description`, `requires`, `companion_skills`). [`manifest.json`](manifest.json)
is the machine-readable registry if you want to enumerate or script against the
skill set.

## Design rules the skills enforce

1. **Scope ≠ selectivity.** In scope and not significant enough are compatible judgments.
2. **Quality ≠ fit.** Excellent science can be a poor fit; modest science can be a good one.
3. **Keywords are not evidence.** Placement follows the manuscript's central contribution, not its topic words.
4. **No fabrication.** No invented acceptance rates, thresholds, or limits. Unverifiable facts are written as `Unknown — not stated in official sources`.
5. **Never predicts acceptance.** Fit assessment is not an outcome prediction, and the output schema has no field for one.
6. **Facts expire.** Every skill carries `last_verified` and `refresh_interval_days`; stale skills should be refreshed or flagged.
7. **Equations are scientific content**, not formatting — never cut an essential one for length, never add one for the appearance of rigor, never invent notation on an author's behalf.
8. **Format is not uniform across the portfolio.** Length limits and mechanisms genuinely differ between journals (PRL's "End Matter" appendix exists nowhere else in the portfolio, for example) — never generalize one journal's convention to another.
9. **No APS journal examined states a figure-count limit.** The skills say so explicitly rather than inventing one.

## Verification and staleness

Journal-specific facts (scope, acceptance criteria, article types, length
limits) were verified directly against `journals.aps.org` — each journal's
`about` and `authors` pages, plus the portfolio-wide scope and policy pages —
on the date recorded in that skill's frontmatter (`last_verified`) and its
source registry. Every skill also carries a `refresh_interval_days` (default
90) after which it should be re-verified before being relied on.

`journals.aps.org` sits behind a bot-challenge that blocks naive fetches; see
[`generators/refresh-protocol.md`](generators/refresh-protocol.md) for the
method that works, and for the full re-verification procedure.

**This repo is a snapshot.** APS policy, scope, and formatting requirements can
change at any time. Treat every `[OFFICIAL]` claim as "true as of the stated
verification date," confirm anything submission-critical against the live APS
page, and never treat this repo as a substitute for a journal's actual author
guidelines.

## Repository layout

```
aps-editorial-intelligence/
├── README.md                    you are here
├── LICENSE                      MIT
├── AGENTS.md                    entry point for any agent
├── CLAUDE.md                    entry point for Claude Code (defers to AGENTS.md)
├── CHANGELOG.md
├── manifest.json                machine-readable skill registry
├── generators/
│   ├── journal-skill-generator.md   meta-prompt: journal name → SKILL.md
│   └── refresh-protocol.md          how and when to re-verify against APS
├── schemas/
│   └── fit-assessment.schema.json   structured output contract
└── skills/
    ├── aps-common/                     portfolio-wide policies (load once)
    ├── aps-mathematical-presentation/  equations as scientific content
    ├── aps-format-and-presentation/    length, figures, style, containers
    ├── aps-journal-selector/           cross-journal recommendation
    ├── aps-manuscript-reviewer/        scientific + editorial assessment
    ├── aps-submission-assistant/       cover letter, checklist, response letters
    └── journals/                       one skill per journal (19 total)
        ├── prl/  prx/  prresearch/
        ├── pra/  prb/  prc/  prd/  pre/
        ├── prmaterials/  prapplied/  prfluids/  prab/  prper/
        ├── prxquantum/  prxenergy/  prxlife/  prxintelligence/
        └── rmp/  apsos/
```

## Contributing

Corrections to journal facts, additions of missing article types, or better
neighbor-journal reasoning are welcome. When contributing a fact about a
journal, cite the `journals.aps.org` URL you verified it against and the date —
see any existing skill's source registry for the expected format. To add a new
journal or regenerate one, start from
[`generators/journal-skill-generator.md`](generators/journal-skill-generator.md).

## License

[MIT](LICENSE).
