# Agent Instructions — APS Editorial Intelligence

This repository is a set of Markdown skills for evaluating manuscripts against
the APS / *Physical Review* journal portfolio. It is model- and vendor-neutral:
Claude, Codex, Gemini, DeepSeek, Qwen, or any agent that can read files and
fetch URLs can execute it.

## How to use it

1. **Always load `skills/aps-common/SKILL.md` first.** It carries the
   portfolio-wide policies, the vocabulary, and the reasoning rules that the
   journal skills assume and do not repeat.

2. **Then load what the task needs — and nothing more.** Do not load all
   nineteen journal skills; the selector tells you which to open.

   | Task | Load |
   |---|---|
   | "Where should I submit?" | `skills/aps-journal-selector/SKILL.md`, then 2–5 journal skills |
   | "Is this right for *X*?" | `skills/journals/<code>/SKILL.md` |
   | "Review this manuscript" | `skills/aps-manuscript-reviewer/SKILL.md` |
   | Theory, computation, or equation-driven work | add `skills/aps-mathematical-presentation/SKILL.md` |
   | Building or revising a manuscript (length, figures, containers, style) | add `skills/aps-format-and-presentation/SKILL.md` |
   | "Prepare the submission" | `skills/aps-submission-assistant/SKILL.md` + the target journal skill |
   | "Add/refresh a journal skill" | `generators/journal-skill-generator.md` and `generators/refresh-protocol.md` |

3. **Follow the skill's decision workflow and output format literally.** The
   formats exist so that outputs are comparable across journals and sessions.

## Non-negotiable rules

- **Label every claim** `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`, matching
  the convention already used in the skills.
- **Never fabricate** APS policy, acceptance rates, editorial thresholds, word
  limits, or rejection criteria. Write `Unknown — not stated in official
  sources` instead of guessing.
- **Never predict acceptance.** Report fit and editorial risk.
- **Never confuse scope with selectivity**, or scientific quality with journal fit.
- **Never place a manuscript on keywords.** Place it on its central contribution.
- **Treat equations as scientific content, not formatting.** Never recommend
  cutting an essential equation to meet a length limit; never add equations to
  raise apparent rigor; never invent notation a manuscript does not use. Each
  journal skill states when to load `aps-mathematical-presentation`, and carries
  a profile calibrated to its field.
- **Never generalize a format fact between *Physical Review* journals.** Length
  limits, article types, and appendix mechanisms differ; End Matter exists only
  at PRL. Load `aps-format-and-presentation` and use the target journal's
  Presentation profile.
- **Label presentation advice** `[REQUIREMENT]` / `[CONVENTION]` / `[STRATEGY]`,
  and never assert a figure-count requirement — no APS journal examined states one.
- **Fetch volatile facts** — length limits, required submission components,
  current article types — from the journal's author page at use time.
- **Check staleness.** If a skill's `last_verified` is older than its
  `refresh_interval_days`, either refresh it or state the staleness in your
  confidence line.

## Fetching APS pages

`journals.aps.org` is behind a bot challenge; plain fetches return HTTP 403 or a
"Just a moment..." interstitial. Use a JS-rendering reader with an explicit wait:

```bash
curl -sS -m 150 -H "x-timeout: 25" \
  "https://r.jina.ai/https://journals.aps.org/prb/about"
```

A response under ~2 KB, or containing "Enable JavaScript and cookies to
continue", is a **failed fetch**, not an empty page. Retry it. Never fill the
gap from model memory.

## File conventions

- Skills live at `skills/**/SKILL.md` with YAML frontmatter (`name`,
  `description`, `requires`, `companion_skills`, and, for journals,
  `journal_code`, `last_verified`, `refresh_interval_days`). `requires` must be
  loaded; `companion_skills` are loaded conditionally, on the trigger stated near
  the top of the skill.
- `manifest.json` is the machine-readable registry — parse it to enumerate
  skills rather than globbing.
- `schemas/fit-assessment.schema.json` defines the structured output contract
  when a caller wants JSON instead of prose.
