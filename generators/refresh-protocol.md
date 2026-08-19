# Refresh Protocol

How to keep the skills true. Facts in this system expire; the protocol makes
expiry visible and cheap to fix.

## 1. When to refresh

| Trigger | Action |
|---|---|
| `last_verified` + `refresh_interval_days` < today | Refresh before relying on the skill, or state the staleness in the confidence line |
| The user reports a policy or requirement that contradicts a skill | Refresh that journal immediately; the live page wins |
| APS announces a new journal or retires one | Add/remove a journal skill; update `aps-common` §2, the selector's Axis-1 map, and `manifest.json` |
| Before drafting any submission material | Fetch the target journal's author page regardless of `last_verified` |

Default cadence: **90 days**.

## 2. What is deliberately not cached

These change often enough that hardcoding them is a liability. The skills point
at them instead of stating them:

- required submission components and statement wording;
- APC amounts;
- article-type definitions in fine detail;
- the exact wording of the PRL criteria-justification requirement;
- review timelines.

Fetch these at use time.

**Length limits and article types are the exception**: they are recorded in each
journal's Presentation profile **with an accessed date**, because a verified
number with an expiry is more useful than no number at all. They must always
carry the date and the re-verify instruction, and they are the first thing to
re-check on every refresh cycle.

## 3. Fetch method

`journals.aps.org` sits behind a Cloudflare bot challenge. Direct fetches
(including most agent web-fetch tools and plain `curl`) return **HTTP 403** or a
`Just a moment...` interstitial.

Working method — a JS-rendering reader with an explicit wait:

```bash
curl -sS -m 150 -H "x-timeout: 25" \
  "https://r.jina.ai/https://journals.aps.org/<code>/about" -o <code>-about.md
```

**Validate every fetch.** A result is a failure, not an empty page, if it is
under ~2 KB or contains `Enable JavaScript and cookies to continue`:

```bash
[ "$(wc -c < f.md)" -gt 2500 ] && ! grep -q "Enable JavaScript" f.md && echo OK
```

Retry failures with a delay; the challenge is intermittent. **Never** substitute
model memory for a failed fetch — that is exactly how fabricated policy enters
a skill.

## 4. Pages per journal

| Page | URL | Carries |
|---|---|---|
| About | `/<code>/about` | Identity, scope, acceptance criteria, article types, OA model |
| Authors | `/<code>/authors` | Requirements, limits, submission components |
| Section selection | `/<code>/authors/guidelines-section-selection-*` | Subject sections |
| Editorial policies and practices | `/<code>/authors/editorial-policies-practices` | Article-type definitions |
| Scope (PRX-family) | `/<code>/scope` | Detailed subject areas |

Portfolio-level: `/scope`, `/authors`, `/authors/editorial-policies`,
`/authors/apcs`.

## 5. Refresh procedure

1. Fetch the journal's `about` page and validate the response.
2. Diff scope bullets and acceptance criteria against the skill's §Scope and
   §Editorial criteria. Any change to criteria is a **material** change.
3. Fetch the author page; confirm article types still exist as described, and
   re-verify every length limit in the Presentation profile. Update the accessed
   date. Check specifically for: new or retired article types, changes to what
   counts against a limit, and any newly stated figure limit (none existed at
   the 2026-08-19 baseline).
4. Update only `[OFFICIAL]` content. Leave `[INFERENCE]` and `[HEURISTIC]`
   sections alone unless the official change invalidates them — hand-tuned
   heuristics are the accumulated value of the system. The Mathematical
   presentation profile is entirely `[INFERENCE]`/`[HEURISTIC]` and should
   normally survive a refresh untouched; revisit it only if the journal changes
   article types, length policy, or supplemental-material policy.
5. Update `version`, `last_verified`, and the source-registry `Accessed` dates.
6. If criteria changed materially, re-check the neighbor tables in *other*
   journal skills that reference this one, and the selector's tier table.
7. Record what changed in `CHANGELOG.md`.

## 6. Portfolio-level checks

Run at every refresh cycle:

1. Fetch `https://journals.aps.org/authors` and compare its journal list against
   `aps-common` §2 and `manifest.json`. New titles appear here first.
2. Fetch `https://journals.aps.org/scope` and check for new subject areas — they
   signal scope expansion across the portfolio.
3. Fetch `https://journals.aps.org/authors/editorial-policies` and check the
   policy section list is unchanged.

## 7. Adding a new journal

1. Run `generators/journal-skill-generator.md` with `TARGET JOURNAL: <name>`.
2. Write the result to `skills/journals/<code>/SKILL.md`.
3. Add it to `aps-common` §2, `manifest.json`, and the selector's Axis-1 domain
   map and Axis-2 tier table.
4. Add it to the neighbor tables of every journal it plausibly competes with —
   this step is the one most often skipped, and neighbor tables are where the
   system's discrimination lives.

## 8. Verification log

Keep one row per refresh in `CHANGELOG.md`:

```
| Date | Scope | Journals touched | Material changes |
|---|---|---|---|
| 2026-08-19 | Initial build | all 19 | Baseline; PRX Intelligence and APS Open Science included |
```
