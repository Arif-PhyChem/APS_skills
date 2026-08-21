# APS Journal Skill Generator

> A reusable meta-prompt. Give it a journal name; it returns one `SKILL.md`.
> Model-agnostic: works with any agent that has a web-fetch/browse tool
> (Claude, Codex, Gemini, DeepSeek, Qwen, local models with a search tool).

---

## Invocation

```
Use generators/journal-skill-generator.md.
TARGET JOURNAL: Physical Review B
```

Optional switches:

- `MODE: refresh` — an existing `SKILL.md` is supplied; update only the facts
  whose sources changed, preserve hand-tuned heuristics, bump `last_verified`.
- `MODE: create` (default) — produce a new skill from scratch.

---

## Role

You are an expert scientific editor, physicist, bibliographic researcher, and
AI-agent skill designer.

You are producing an **executable editorial reasoning framework**, not an
article about a journal. The reader is another AI agent that must decide
whether a specific manuscript belongs in this journal.

---

## PART I — WEB RESEARCH (do this before writing anything)

### 1. Source priority

**Tier 1 — authoritative, mandatory.** `journals.aps.org` and `aps.org`.
Retrieve at minimum:

| Query | Typical URL |
|---|---|
| journal about/scope | `journals.aps.org/<code>/about` |
| information for authors | `journals.aps.org/<code>/authors` |
| section selection guidelines | `journals.aps.org/<code>/authors/guidelines-section-selection-*` |
| article types & length | `journals.aps.org/<code>/authors/editorial-policies-practices` |
| common editorial policies | `journals.aps.org/authors/editorial-policies` |
| portfolio scope | `journals.aps.org/scope` |

**Tier 2 — official supporting.** APS style guide, open-science policy,
supplemental-material policy, web submission guidelines, APC pages.

**Tier 3 — published APS material.** Editorials, `edannounce` pages,
representative papers, editor-authored guidance. Useful for inferring
editorial positioning. **Never** treat these as policy unless APS states them
as policy.

**Tier 4 — external.** Only when Tiers 1–3 are silent. Never allowed to
override current official APS information.

### 2. Fetching note (practical)

`journals.aps.org` sits behind a bot challenge. A plain fetch often returns
HTTP 403 / "Just a moment...". If your fetch tool is blocked, use a
JS-rendering reader and allow it to wait for the challenge, e.g.

```
curl -sS -m 150 -H "x-timeout: 25" "https://r.jina.ai/https://journals.aps.org/prb/about"
```

Verify you received real content — a body under ~2 KB, or containing
"Enable JavaScript and cookies to continue", is a failed fetch, not an empty
page. **Never** synthesize a scope statement from memory after a failed fetch.

### 3. Verification discipline

For each material claim record: source URL, page title, date accessed, and
whether it is policy or inference. Open the actual page — do not quote search
snippets when the page is reachable. Prefer current pages over archived ones.

If two APS pages disagree: prefer the newer authoritative page, determine
whether the difference is a policy change, record the conflict in the Source
Registry, use the current policy, and do not silently merge them.

### 4. Three-way epistemic labeling (mandatory)

Every statement in the output belongs to exactly one class, and the class must
be visible to the reading agent:

| Tag | Meaning |
|---|---|
| `[OFFICIAL]` | Explicitly stated by APS. Must be traceable to a Tier-1/2 URL. |
| `[INFERENCE]` | Reasonable editorial reading of official scope/criteria. |
| `[HEURISTIC]` | A decision rule invented to help the agent judge fit. Never presented as APS policy. |

Sections that are wholly one class may carry a single header tag instead of
per-line tags.

---

## PART II — UNDERSTAND THE JOURNAL

### 5. Identity

Official name, abbreviation, journal code, publisher, scientific domain,
readership, role in the portfolio, access model. Do **not** use impact factor
or ranking to define identity.

### 6. Scope

Extract the official scope and reorganize it into an operational form:
core areas / major subfields / emerging-interdisciplinary areas / boundaries.
A flat keyword dump is a failure mode — an agent cannot reason over it.

### 7. Editorial criteria

Extract the journal's stated acceptance criteria verbatim where possible.
Then, separately, interpret them. Keep the two visibly distinct.

Example of the required separation:

- `[OFFICIAL]` PRL requires manuscripts to meet one or more stated criteria.
- `[INFERENCE]` A new network architecture with no new physics is unlikely to
  satisfy any of them.

### 8. Article types

For each currently supported type: purpose, research vs. commentary, length
limit, invited or unsolicited, presubmission-inquiry expectations. Do not
invent article types, and do not carry over types from a sibling journal.

### 9. Manuscript requirements

Only those verified and relevant: preparation, title, abstract, references,
figures, tables, supplemental material, data availability, code, author
information, funding, competing interests, submission components.

---

## PART III — EDITORIAL REASONING MODEL

### 10. Positioning model

Answer: *what kind of contribution is this journal looking for?* Assess along
scope, novelty, significance, conceptual advance, methodological advance,
breadth, generality, evidence, presentation.

### 11. Quality ≠ fit (mandatory)

A manuscript can be excellent science and a poor fit; sound but insufficiently
significant for a selective venue; technically impressive but thin on physical
interpretation; narrow but perfect for a specialized journal. Never collapse
"good paper" into "good fit".

### 12. Neighboring journals

Identify the 3–6 APS journals most easily confused with the target. For each,
give both directions:

> Prefer `<neighbor>` when …
> Prefer `<target>` when …

Base the distinction on official scope and positioning, not invented contrast.

---

## PART IV — REQUIRED OUTPUT STRUCTURE

Emit a single `SKILL.md` with YAML frontmatter, then these sections:

```yaml
---
name: aps-<code>
description: <one line: when an agent should load this skill>
journal: <full name>
abbreviation: <abbr>
journal_code: <code>
publisher: American Physical Society
access_model: <hybrid | gold open access>
version: <YYYY-MM-DD>
last_verified: <YYYY-MM-DD>
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
---
```

1. Purpose
2. Journal Identity
3. Scope
4. Scope Boundaries
5. Editorial Criteria (official, quoted)
6. Editorial Positioning
7. What Constitutes a Strong Fit
8. Weak-Fit Patterns
9. Manuscript Evaluation Framework
10. Article Types
11. Manuscript Preparation Requirements
12. Supplemental Material / Data / Code
13. Neighboring APS Journals
14. Journal Selection Rules
15. Manuscript Positioning Advice
16. Submission Checklist
17. Decision Workflow
18. Output Format
19. Mathematical Presentation Profile
20. Presentation Profile
21. Source Registry

---

## PART V — OPERATIONAL EVALUATION CONTENT

### Fit classification

The skill must define operational criteria for: **Excellent / Strong /
Moderate / Borderline / Poor**. Classification from keywords alone is
forbidden; the criteria must reference contribution type, significance, and
breadth.

### Evaluation workflow the skill encodes

1. Primary scientific question
2. Central contribution
3. What is genuinely new
4. Scientific domain
5. Scope fit
6. Novelty
7. Significance
8. Conceptual contribution
9. Methodological contribution
10. Breadth of interest
11. Evidence and validation
12. Comparison with neighboring APS journals
13. Editorial vulnerabilities
14. Fit classification
15. Positioning recommendations

### AI/ML manuscripts

The skill must force these apart:

1. novelty of the AI/ML method;
2. novelty of the scientific result;
3. scientific insight the method enabled;
4. generality of the method;
5. domain significance.

Model architecture is not the scientific contribution. Where the method has a
meaningful mathematical statement — a learning objective, a physical constraint,
a guarantee — the skill should direct the agent to assess *that*, and only when
it genuinely represents the manuscript's method.

A sophisticated architecture is not by itself a scientific advance. Nor is the
use of machine learning a reason to discount work. Evaluate what the method
*enabled*. Note that APS now runs a dedicated AI venue (*PRX Intelligence*),
which changes the neighbor analysis for every journal.

### Mathematical presentation (mandatory section)

Equations are scientific content, not formatting. Every generated skill must
carry a **Mathematical Presentation Profile** calibrated to the journal and its
research areas, with these fields:

- **Mathematical representation importance:** Low / Moderate / High / Very High
- **Expected equation density:** Low / Moderate / High
- **Role of equations:** what the mathematics does in this journal's papers
- **Main-text mathematical content:** what must stay
- **Supplementary mathematical content:** what can move
- **Recommended derivation depth:** how much to show, and where
- **Figure–equation integration:** how formulation and evidence connect
- **Recommended presentation strategy:** concrete guidance

The section must also state **when to load `aps-mathematical-presentation`** for
this journal — always, usually, or conditionally — and put that instruction near
the top of the skill as well, so the agent sees it before it starts reasoning.

Constraints on this section:

- All of it is `[INFERENCE]` or `[HEURISTIC]`. APS states formatting and style
  requirements, not doctrine about equation density. Never present density,
  hierarchy, or derivation-depth advice as APS policy.
- Calibrate to the journal's actual research character, not to a portfolio
  average: PRD and PRE are equation-dense; PRMaterials and PRApplied are not;
  PRPER's relevant mathematics is statistical, not physical; RMP's is
  pedagogical and unifying.
- Never state or imply that a journal formally requires a particular number of
  equations or figures. Where a pattern is merely common practice, label it as
  such and keep it separate from official requirements.
- Never invent notation. Example equations in a skill must be generic
  illustrations of a *form*, never fabricated results attributed to anyone.

### References (mandatory pointer)

Every generated journal skill must declare `aps-reference-format` in its `companion_skills` frontmatter and, near the top of the skill, state whether this journal adds anything to the portfolio-wide reference mechanics — most will not (PRL's titles-in-references convention is the only one on record). Never restate the numbering/citation/author-count mechanics inside a journal skill; those live once, centrally, in `aps-reference-format`.

### Format and presentation (mandatory section)

Physical Review journals do **not** share one manuscript format. Research and
encode this journal's own conventions, and never generalize a format fact from a
sibling journal.

Fetch `/<code>/authors` and record, with the accessed date:

- every article type available **at this journal**, with its length limit;
- what counts against the limit and what does not;
- appendix mechanism — note that **End Matter exists only at PRL**;
- title and abstract requirements; section-structure expectations;
- figure and table requirements; whether any figure limit is stated
  (**no APS journal examined states one** — record its absence explicitly);
- Supplemental Material definition, mechanics, and citation format;
- reference-style specifics; data/code requirements; templates.

Then produce a **Presentation Profile**:

- **Article format:** short / full-length / flexible / review
- **Available length containers**
- **Stated length limits** (with accessed date) or `No explicit limit stated`
- **Typical mathematical density**
- **Recommended main-text figure strategy** — derived from the scientific
  narrative, never a target number
- **Supplementary-material role**
- **Preferred narrative style**
- **Recommended manuscript compactness:** Low / Moderate / High
- **Presentation priority**

Label every statement **[REQUIREMENT]** (official rule, with URL),
**[CONVENTION]** (strong practice, not a rule), or **[STRATEGY]** (recommended
editorial approach). Never convert a convention into a requirement. Never invent
a numerical limit — state its absence instead. Never assert a figure count.

### Computational manuscripts

Require: physical interpretation, validation, comparison with established
methods, numerical robustness, reproducibility, generality. Computational cost
and complexity are not evidence of significance.

---

## PART VI — SOURCE REGISTRY

End the skill with:

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|

Every journal-specific fact must be traceable to a row. Use real URLs.

---

## PART VII — QUALITY CONTROL

Before returning, verify and silently fix:

**Accuracy** — every `[OFFICIAL]` claim has a Tier-1/2 URL; current pages
used; conflicts recorded.

**Completeness** — scope, criteria, article types, requirements, neighbors,
evaluation framework, positioning advice, registry all present.

**Reasoning** — scope distinguished from selectivity; quality from fit;
policy from inference; an agent can actually execute it.

**Anti-hallucination** — delete invented acceptance rates, editorial
thresholds, word limits, rejection criteria, claims about named editors, or
claims about typical acceptance behavior. Anything unverifiable is written as
`Unknown — not stated in official sources`, never guessed.

**Size** — the skill must stay loadable as an agent context (target under
~500 lines).

---

## FINAL INSTRUCTION

Research first. Then return **only** the completed `SKILL.md`. No preamble, no
commentary, no summary of what you did.
