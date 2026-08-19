---
name: aps-manuscript-reviewer
description: Assess a manuscript the way an APS editor and referee would — scientific soundness, novelty, evidence, and the specific objections likely to be raised — separately from journal fit. Use before or alongside aps-journal-selector.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# APS Manuscript Reviewer

Load `aps-common`. This skill judges **the manuscript**; `aps-journal-selector`
judges **the placement**. Keep the two verdicts separate — that separation is
the point of the whole system.

## 1. What this skill does and does not do

Does: identify the contribution, test the evidence, find the objections a
referee will raise, and say what would fix them.

Does **not**: predict the editorial decision, assign a score, or substitute for
peer review.

## 2. Pass 1 — Reconstruct the claim

Fill this before critiquing anything:

| Field | Value |
|---|---|
| Central claim (one sentence) | |
| Claim type | measurement / mechanism / theory / method / tool / synthesis |
| What was previously known | |
| What this adds | |
| Evidence offered | |
| Assumptions the claim rests on | |
| Scope of validity claimed | |
| Scope of validity supported | |

> The gap between the last two rows is where most referee reports live.

## 3. Pass 2 — Soundness

- **Methodology** — appropriate to the question? Standard for the field?
- **Controls and baselines** — present, and are they the *strong* baselines?
- **Uncertainty** — statistical and systematic, separated and propagated?
- **Convergence/robustness** — for computation: resolution, cutoffs,
  finite-size, seeds. For experiment: repeats, drift, calibration.
- **Statistics** — appropriate tests, effect sizes, multiple-comparison handling,
  priors and likelihoods stated for inference.
- **Reproducibility** — could a competent group reproduce this from what is written?
- **Internal consistency** — do the figures, tables, and text agree?

Any failure here is prior to fit: an unsound manuscript has no correct journal.

## 4. Pass 3 — Novelty audit

Separate and name each:

| Kind | Present? | Evidence |
|---|---|---|
| New phenomenon | | |
| New mechanism | | |
| New material/system | | |
| New measurement or precision | | |
| New method or algorithm | | |
| New tool, dataset, or resource | | |
| New interpretation or unification | | |

Then check novelty **relative to the literature, not to the authors' prior
work**. Search for the nearest prior art and state it explicitly. Novelty
claimed against a strawman baseline is a standard referee objection.

## 5. Pass 4 — Significance

- Who changes what they do because of this result?
- Does it settle a question, open one, or add a data point?
- Is the significance argued, or asserted with adjectives?
- Does the significance survive the stated limitations?

Report significance **without** reference to any particular journal. The journal
comparison happens in the selector.

## 6. Pass 5 — AI/ML and computational specifics

For any manuscript using ML, LLMs, agents, or heavy computation, apply the
five-way decomposition:

1. Method novelty
2. Scientific novelty
3. Enablement — what became possible
4. Generality — transfer beyond the studied systems
5. Validation — baselines (including strong non-ML ones), ablations, held-out
   and out-of-distribution tests, uncertainty, SOTA comparison, compute cost

Additional checks: data leakage between train and test; distribution shift;
cherry-picked examples; metrics that do not measure the scientific claim;
missing seeds or single-run results; interpretability claims with no falsifiable
test.

Do not penalize a manuscript for using ML, and do not credit architecture
sophistication as scientific significance.

## 7. Pass 5b — Mathematical presentation

For any theoretical, computational, or equation-driven manuscript, load
`aps-mathematical-presentation` and run its framework. Report at minimum:

- **Central mathematical object** — the equation or relation expressing the
  contribution, or a finding that the manuscript has one and never writes it down.
- **Equation audit** — any displayed equation with no identifiable purpose, and
  any algebraic expansion that does not advance the argument.
- **Hierarchy check** — essential / supporting / derivational, and whether an
  essential equation has been pushed to the supplement to meet a length limit.
- **Interpretation gaps** — important equations presented without saying what
  they mean, what assumption they embed, or why they matter (equation dumping).
- **Undefined symbols** and approximations introduced without a validity regime.
- **Figure–equation chain** — is theory → prediction → evidence made explicit?
- **Mathematical novelty kind** — new mathematics / new physical theory / new
  solution / new application — and whether the abstract claims more than that.

Two errors to avoid symmetrically: treating mathematical complexity as
significance, and manufacturing mathematical criticism of a manuscript that is
not equation-driven. If the paper's contribution is a measurement or a
characterization, say the section does not apply.

## 8. Pass 6 — Presentation

For manuscript construction — length, figure strategy, main-text vs Supplemental
Material — load `aps-format-and-presentation` and report against its framework.

- Does the title state the claim?
- Does the abstract lead with the result?
- Does the introduction frame a community problem, or the authors' project?
- Do figures carry the argument, or only the data?
- Are limitations stated, or hidden?
- Is prior work cited fairly, including competing groups and negative results?
- **Figure audit** — what does each figure prove? Any figure proving nothing the
  text does not already establish, any figure doing two jobs, any pair doing one
  job, any central claim with no figure?
- **Container audit** — is anything essential to understanding or evaluating the
  central claim sitting in Supplemental Material? That is a defect, not a
  formatting choice.

## 9. Pass 7 — Research integrity

Check and flag: authorship and contribution statements; competing interests;
funding disclosure; data and code availability; ethics approval where human or
animal subjects are involved; image-manipulation risk; text reuse and
self-plagiarism; and disclosure of AI-tool use in manuscript preparation.

For the binding requirements, fetch
`journals.aps.org/authors/editorial-policies-ethics` and the authorship page —
these change, and must be quoted rather than paraphrased from memory.

## 10. Output format

**Central claim:** …
**Claim type:** …

**Soundness:** Sound / Sound with reservations / Unsound — with the specific issues.

**Novelty audit:** which kinds are present, and relative to what prior art.

**Significance:** who is affected and how — journal-independent.

**Evidence gaps:**
1. … (what is missing, and what would close it)
2. …

**Anticipated referee objections:**
1. … — *strength: likely / possible* — *response available: yes / no*
2. …

**Overclaims to retract:** exact sentences that outrun the evidence.

**Mathematical presentation:** central object, equation audit, hierarchy,
interpretation gaps, figure–equation chain — or "not equation-driven".

**Presentation fixes:** …

**Integrity checklist:** items outstanding.

**What would most raise this manuscript's standing:** the two or three highest-
leverage additions, ranked by effort-to-benefit.

**Confidence:** High / Medium / Low — and what you could not assess.

## 11. Rules

1. Critique the manuscript, not the authors.
2. Every objection names the fix.
3. Distinguish "wrong" from "not shown" from "not framed well".
4. Do not manufacture objections to appear rigorous; say when something is solid.
5. Never predict the editorial outcome.
6. If you could not read part of the manuscript (missing figures, SI), say so
   rather than inferring.
7. Never invent an equation for the manuscript and then assess it against your
   own formulation. Work with the notation the authors used, or recommend that
   they write down an object they clearly possess.

## 12. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| APS Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Integrity, authorship, peer review |
| APS ethics and research integrity | https://journals.aps.org/authors/editorial-policies-ethics | Official | 2026-08-19 | Integrity requirements (fetch before advising) |
