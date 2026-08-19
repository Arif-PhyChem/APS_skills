---
name: aps-journal-selector
description: Choose the best APS/Physical Review journal for a manuscript. Extracts the scientific contribution, shortlists candidates, evaluates each against its journal skill, ranks them, and explains why the winner beats the runner-up. Start here for any "where should I submit?" question.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# APS Journal Selector

Load `aps-common` first. Load individual journal skills on demand — do not load
all nineteen. For theoretical, computational, or otherwise equation-driven
manuscripts, also load `aps-mathematical-presentation`; each journal skill states
when its own material warrants it.

## 1. Purpose

Recommend the most appropriate *Physical Review* journal for a manuscript, with
a defended comparison against the alternatives and concrete positioning advice.

## 2. Core principle

**Never select a journal from topic keywords.** Derive, in order:

1. primary physics/science domain
2. central scientific contribution
3. novelty (and of what kind)
4. significance
5. conceptual advance
6. methodological contribution
7. breadth of interest
8. intended readership

Then match those against journals' **editorial positioning**, not their topic
lists. Scope tells you which journals are *possible*; positioning tells you
which is *right*.

## 3. Two orthogonal axes

Every APS placement decision resolves along two independent axes. Fix both
before naming a journal.

**Axis 1 — Domain.** Which community is the audience?

```
AMO / quantum science ....... PRA        Condensed matter .......... PRB
Nuclear ..................... PRC        Particles/gravity/cosmo ... PRD
Statistical/nonlinear/soft/   PRE        Materials ................. PRMaterials
  bio/fluids/plasma/comp                 Applied / devices ......... PRApplied
Fluid dynamics .............. PRFluids   Accelerators and beams .... PRAB
Quantum info sci & tech ..... PRXQuantum Energy .................... PRXEnergy
Quantitative biology ........ PRXLife    AI/ML for science ......... PRXIntelligence
Physics education research .. PRPER      All physics ............... PRL/PRX/PRResearch
```

**Axis 2 — Tier / contribution character.**

| Tier | Journals | The bar |
|---|---|---|
| Pivotal & broad, short | PRL | Opens an area, solves a critical problem, highly impactful method, or unusual intrinsic interest |
| Field-defining, flexible length | PRX | Discovery, landmark, paradigm shift, key connections, high-impact community tools |
| Exceptional within a domain | PRX Quantum, PRX Energy, PRX Life, PRX Intelligence | "Exceptional" advance / connection / capabilities / insight |
| Significant within a research area | PRA, PRB, PRC, PRD, PRE, PRMaterials, PRApplied, PRFluids, PRAB, PRPER | High-quality, significant, authoritative and substantive |
| Broad, significant, gold OA | PRResearch | Significant contribution with a connection to physics |
| Sound, useful, transparent | APS Open Science | Technically correct and meaningfully additive — **no significance criterion** |
| Synthesis, not primary research | RMP | Critical, authoritative review or colloquium |

> The most common placement error is getting Axis 1 right and Axis 2 wrong —
> a correct-domain submission aimed one or two tiers above the manuscript's
> actual contribution.

## 4. Workflow

### Step 1 — Extract the manuscript profile

Produce, before considering any journal:

| Field | Value |
|---|---|
| Research field | |
| Physical system | |
| Methodology | |
| Central result | |
| Primary novelty (type) | mechanism / phenomenon / material / measurement / method / tool / interpretation / synthesis |
| What became possible | |
| Evidence quality | |
| Central mathematical object | the equation/relation expressing the contribution, or "none" |
| Mathematical density (actual) | Low / Moderate / High / Very high |
| Intended readership | |
| Broader implication | |

If the manuscript's central result cannot be stated in one sentence without
"and", the paper likely has a positioning problem, not a journal problem. Say so.

### Step 2 — Apply the routing gates (in order)

These are blocking tests; each one, if triggered, overrides topic intuition.

1. **Review gate** — is this a review/colloquium rather than primary research?
   → RMP, or a domain journal's Review Article type. Stop.
2. **Output gate** — is the contribution a dataset, software release,
   replication, or null result? → APS Open Science (or PRX for a high-impact
   community tool/database). Stop unless a research claim dominates.
3. **Education gate** — is the object of study teaching and learning?
   → PRPER. Stop.
4. **AI/ML gate** — is the central contribution the AI/ML method, tool, or
   insight rather than a domain result? → PRX Intelligence; PRE's computational/
   ML/AI section for area-tier work. If ML is instrumentation and the claim is a
   domain claim, continue to the domain journal.
5. **Application gate** — is the claim about a device or application?
   → PRApplied (with the physical-insight requirement) or PRX Energy.
6. **Materials gate** — is the claim about the material rather than the
   mechanism? → PRMaterials rather than PRB.
7. **Format gate** — do the manuscript's *essential* equations fit the target
   article type? If a short format would force an essential equation out of the
   main text, that is a placement finding: recommend the full-length article
   type, or a journal with flexible length, rather than cutting the equation.
   See `aps-mathematical-presentation` §4 and `aps-format-and-presentation` §5.
   Note that full-length articles carry **no length limit** at nearly every
   specialist journal — length pressure is a Letters/PRL problem, not a
   portfolio-wide one, and a "too long" manuscript usually needs a different
   article type rather than a different journal.

### Step 3 — Shortlist 2–5 candidates

Always include:
- the natural domain journal (Axis 1);
- one tier up and one tier down (Axis 2);
- any journal implicated by a gate in Step 2.

### Step 4 — Evaluate each candidate against its own skill

Load each candidate's journal skill. Judge scope fit, criterion match,
significance fit, readership fit, breadth, methodological fit, and likely
editorial concerns — **using that journal's stated criteria, not a generic
notion of quality**.

### Step 5 — Rank

Assign each: Excellent / Strong / Moderate / Borderline / Poor. Ranking without
per-criterion reasoning is not acceptable output.

### Step 6 — Explain the margin

State explicitly why #1 beats #2. If they are genuinely close, say so and give
the deciding factor the authors control (framing, added evidence, OA
requirements, speed, audience).

## 5. Special rules

1. **Excellent science can be a poor fit.** Do not conflate them; report them as
   separate lines.
2. **Never predict acceptance.** Report fit and editorial risk only.
3. **Every recommendation names a fallback**, and the transfer path if relevant
   — *Physical Review* journals support transfers, and APS Open Science
   explicitly accepts them.
4. **Open access can be a legitimate deciding factor** (funder mandates,
   dissemination goals). Say so plainly rather than dressing it up as a scope
   argument. PRAB is gold OA at zero author cost; PRX, PRResearch, PRX Quantum,
   PRX Energy, PRX Life, PRX Intelligence, and APS Open Science charge APCs;
   waivers exist for authors from lower-income countries.
5. **Check staleness.** If a journal skill's `last_verified` exceeds its
   `refresh_interval_days`, re-fetch its `about`/`authors` pages or flag the
   staleness in the confidence line.
6. **Letters ≠ PRL.** Recommending "a Letter" must always name the journal.
7. **Mathematical density is a fit dimension, not a quality dimension.** A
   manuscript whose density is wrong for a journal is often right for a
   neighbor — a very-high-density treatment squeezed toward PRL usually belongs
   at PRB, PRD, or PRE at full length. Report the mismatch as placement
   information, never as a defect.

## 6. Output format

### Recommended journal

**[Journal]** — fit class, one-sentence reason.

### Alternative

**[Journal]** — fit class, one-sentence reason.

### Ambitious option (only if defensible)

**[Journal]** — what the manuscript would need to add or demonstrate.

### Comparison

| Criterion | Recommended | Alternative | Ambitious |
|---|---|---|---|
| Scope fit | | | |
| Criterion match | | | |
| Novelty fit | | | |
| Significance fit | | | |
| Breadth / readership | | | |
| Methodological fit | | | |
| Evidence sufficiency | | | |
| Mathematical density fit | | | |
| Essential equations fit format | | | |
| Article type + length fit | | | |
| Access model | | | |
| **Overall fit** | | | |

### Reasoning

Why #1 beats #2, in terms of the manuscripts's actual contribution.

### Editorial risks

The two or three objections a referee or editor is most likely to raise.

### Positioning advice

How to frame the manuscript for the recommended journal — title, abstract,
introduction, emphasis, evidence to add.

### Format consequences

Article type, its verified length limit, available containers (appendix / End
Matter / Supplemental Material), and what would have to move. Label each as
[REQUIREMENT] / [CONVENTION] / [STRATEGY]. Where a **Joint Submission** resolves
a pivotal-but-long manuscript, say so.

### Fallback path

Second choice, and the transfer route if the first submission fails.

### Confidence

High / Medium / Low — and what evidence would change it.

## 7. Worked example of the reasoning style

**Manuscript:** an ML framework fusing chemical heuristics, numerical
descriptors, and a language-model-derived representation to identify candidate
topological materials.

**Profile:** domain = computational materials / topological matter; central
contribution = a hybrid ML architecture; novelty type = method + tool; what
became possible = faster candidate identification; readership = ML-for-materials
and topological-materials communities.

**Gates:** the AI/ML gate fires — the central contribution is the method, not a
statement about topological matter.

**Shortlist and reasoning:**

- **PRX Intelligence** — the method is the contribution, which is precisely what
  this venue rewards. Fit depends entirely on the validation gate (baselines,
  ablations, held-out and out-of-distribution tests, SOTA comparison) and on
  demonstrated enablement. Strong if those hold.
- **PRMaterials** — viable *if* the paper closes the loop and validates
  candidate materials, making the materials outcome the contribution.
- **PRB** — appropriate only if the paper delivers new physical understanding of
  the topological states themselves; a screening pipeline alone is a weak fit.
- **PRResearch** — the sound fallback if the work is solid but neither
  exceptional as ML nor conclusive as materials physics.
- **PRL / PRX** — only with a discovery: a validated new topological material or
  a mechanism insight of broad interest. Not reachable on methodology alone.

**Deciding factor the authors control:** whether the manuscript's centre of
gravity is the architecture (→ PRX Intelligence, strengthen validation) or a
validated material outcome (→ PRMaterials, close the loop experimentally or
computationally).

## 8. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| Publishing Guidelines | https://journals.aps.org/authors | Official | 2026-08-19 | Current title list |
| Scope of APS Journal Portfolio | https://journals.aps.org/scope | Official | 2026-08-19 | Subject coverage |
| Journal *about* pages, all 19 titles | https://journals.aps.org/<code>/about | Official | 2026-08-19 | Scope, acceptance criteria, article types |
