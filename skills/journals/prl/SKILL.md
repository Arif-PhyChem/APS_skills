---
name: aps-prl
description: Evaluate a manuscript's fit for Physical Review Letters — APS's flagship short-format journal for the most influential developments across all of physics.
journal: Physical Review Letters
abbreviation: PRL
journal_code: prl
publisher: American Physical Society
access_model: hybrid
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation]
---

# Physical Review Letters — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` whenever the manuscript is equation-driven** — the short format makes the equation/prose trade-off decisive, and compression is where PRL submissions most often go wrong. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

## 1. Purpose

Judge whether a manuscript clears PRL's criteria — a genuinely different
question from whether it is good work — and, if not, route it.

## 2. Identity `[OFFICIAL]`

PRL is "the world's premier physics letter journal and the American Physical
Society's flagship publication." Since 1958 it has published seminal research
across all fields of physics. It publishes "short, high-quality reports of the
most influential developments and transformative ideas in the full arc of
fundamental, applied and interdisciplinary physics research," and is
"distinctive in the depth and breadth of its coverage of the broad subfields of
physics." PRL welcomes manuscripts reporting "pivotal advances that will
influence the research of others."

**All published Letters meet at least one of the acceptance criteria.** `[OFFICIAL]`

Readership: the whole physics community, not one subfield.

## 3. Scope `[OFFICIAL]`

As the flagship journal, PRL welcomes all applied, fundamental, and
interdisciplinary physics topics covered by the *Physical Review* portfolio.
Published sections:

- Quantum information, science, and technology
- Cosmology, astrophysics, and gravitation
- Particles and fields
- Nuclear physics
- Atomic, molecular, and optical physics
- Physics of fluids, earth & planetary science, and climate
- Plasma and solar physics, accelerators and beams
- Condensed matter and materials
- Statistical physics; classical, nonlinear, and complex systems
- Polymers, chemical physics, soft matter, and biological physics

> **Scope is not the filter at PRL.** `[INFERENCE]` Almost all physics is in
> scope; the criteria in §4 are where manuscripts are actually separated. Never
> report "in scope" as if it were a positive fit signal here.

## 4. Acceptance criteria `[OFFICIAL]`

Submitted manuscripts should significantly advance fundamental or applied
physical science by meeting **one or more**:

1. **Open a new research area, or a new avenue within an established area.**
2. **Solve, or make essential steps towards solving, a critical problem.**
3. **Introduce techniques or methods with highly significant impact.**
4. **Be of unusual intrinsic interest to PRL's broad audience.**

**Agent rule** `[HEURISTIC]`: name which criterion the manuscript claims, in
one sentence, using the manuscript's own results. If you cannot write that
sentence without hedging, the manuscript does not yet meet the bar. "Meets all
four vaguely" is a fail, not a pass.

## 5. Editorial positioning `[INFERENCE]`

| Dimension | PRL's demand |
|---|---|
| Novelty | High — pivotal, not incremental |
| Significance | Must influence others' research |
| Breadth | Broad physics audience, not one subfield |
| Format | The message must survive compression to a short paper |
| Evidence | Complete enough to be convincing at short length |
| Timeliness | Advances that change what people do next |

The test is **influence**: will researchers act differently because of this?

## 6. Strong-fit profile `[INFERENCE]`

- Opens a research direction others can immediately pursue.
- Delivers first observation/realization of a predicted phenomenon.
- Resolves a recognized outstanding controversy or problem.
- Introduces a technique that unlocks a class of previously impossible measurements or calculations.
- Bridges subfields such that two communities both care.
- Has a single, sharp, compressible central message.

## 7. Weak-fit patterns `[HEURISTIC]`

- Excellent but subfield-bounded — the classic PRB/PRA/PRC/PRD/PRE case.
- Thorough and definitive but not *pivotal* (route to the specialist journal).
- Message needs full-length development to be convincing.
- Novelty framed relative to the authors' own prior papers.
- Method paper whose impact is asserted rather than demonstrated.
- "First application of technique X to system Y" without a consequence.
- Significance claims that rest on adjectives rather than results.

## 8. Evaluation framework

- **A. Criterion match** — which of the four, and on what evidence?
- **B. Novelty** — what specifically was not known before?
- **C. Influence** — who changes what they do, and when?
- **D. Breadth** — would a physicist outside the subfield read past the abstract?
- **E. Compressibility** — does the argument fit the format without gutting the evidence?
- **F. Evidence** — sufficient at short length; supplemental material used properly.
- **G. Alternatives** — is a specialist journal or PRX the better home?

## 9. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Unambiguously satisfies a criterion; broad interest evident; message sharp and well evidenced |
| **Strong** | Clearly satisfies one criterion; breadth good though possibly concentrated in adjacent subfields |
| **Moderate** | Plausible criterion match that depends on framing; would strengthen with a sharper central claim or stronger evidence |
| **Borderline** | Real advance, but significance is subfield-scale; specialist journal likely a better fit |
| **Poor** | Incremental, narrow, or method-first with unproven impact |

## 10. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRX** | Fundamental discovery, landmark, paradigm shift, or a major community tool/database — and the work needs flexible length and depth rather than compression |
| **PRResearch** | Solid significant work across any physics topic; gold OA; no requirement of pivotal breadth |
| **PRB / PRA / PRC / PRD / PRE / PRFluids / PRMaterials / PRApplied / PRAB** | Significance is real but specific to that research area — the specialist journals' criteria ask for a "high-quality, significant contribution in a specific research area," which is a different bar |
| **PRX Quantum** | Exceptional advance/connection/capabilities/insight specifically in quantum science and technology |
| **PRX Intelligence** | The central contribution is AI/ML for the physical sciences |
| **PRX Energy / PRX Life** | Energy or living-systems focus with a highly selective, interdisciplinary audience |
| **RMP** | The work is a review or colloquium, not primary research |

Prefer **PRL** when: the advance is pivotal, broadly interesting, and expressible
short.

## 11. Article type and submission `[OFFICIAL]`

`[OFFICIAL]` PRL publishes **Letters** — length limit **3750 words**, about
four journal pages for the core of the paper (between the abstract and the
Acknowledgments). Authors may add up to **two pages of End Matter** —
appendices or other content specialists will want or need — which appears after
the references and **does not count against the core limit**. Also: **Essays**
(3750 words) and **Comments/Replies** (750 words). Verified 2026-08-19; re-fetch
`/prl/authors` before advising.

> `[OFFICIAL]` **End Matter is specific to PRL.** Letters at other *Physical
> Review* journals do not have it; they use Appendixes instead.

`[OFFICIAL]` At submission PRL requires a short statement (reported as a
~100-word paragraph) explaining why the manuscript meets the journal's
criteria. **Verify the current wording and word count on `/prl/authors` before
drafting it** — this requirement's details change and must not be asserted from
memory.

> `[HEURISTIC]` That justification paragraph is the highest-leverage text in a
> PRL submission. Draft it by naming one criterion, the specific result that
> satisfies it, and who is affected. Not adjectives.

## 12. Positioning advice `[HEURISTIC]`

- **Title** — the claim, not the system studied.
- **Abstract** — result first, then why it matters, then how. The significance
  sentence should be defensible without the word "novel."
- **Opening paragraph** — the community-level problem, in language a physicist
  from another subfield understands.
- **Criterion alignment** — make the target criterion visible in the abstract
  and the closing paragraph.
- **Compression** — move validation to supplemental material, never the
  reasoning.
- **Breadth** — one explicit sentence on implications beyond the immediate system.
- **Honesty** — do not inflate. Overclaiming is a recognizable and costly
  failure mode at this tier.

## 13. Submission checklist

- [ ] Named criterion, with the specific result that satisfies it
- [ ] Justification statement drafted per current `/prl/authors` requirements
- [ ] Message survives short format; supplemental material carries validation
- [ ] Breadth argued explicitly
- [ ] Section selected from PRL's section list
- [ ] Prior work compared fairly, including competing groups
- [ ] Figures: few, decisive, legible at print size
- [ ] Data/code availability per APS open-science policy
- [ ] AI-tool use disclosed per current APS ethics policy
- [ ] Fallback journal identified before submission

## 14. Decision workflow

1. Central contribution in one sentence.
2. Which criterion (§4) — name exactly one primary.
3. Evidence that the criterion is met.
4. Who is influenced, and how soon.
5. Breadth test outside the subfield.
6. Compressibility test.
7. Evidence sufficiency at short length.
8. Compare against PRX and the relevant specialist journal.
9. Editorial vulnerabilities.
10. Fit class; positioning changes; confidence.

## 15. Output format

Use the standard portfolio output block (see `aps-journal-selector` §Output),
adding a mandatory line:

**Criterion claimed:** 1 / 2 / 3 / 4 — with the one-sentence justification.

Never state or imply the manuscript will be accepted.

## 16. Mathematical presentation profile

Load `aps-mathematical-presentation` for the full framework. PRL-specific
calibration `[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High — varies by section, from
near-essential in condensed-matter theory, particles and fields, and statistical
physics, to moderate in experimental AMO and materials Letters.

**Expected equation density:** Moderate — the format rewards few equations doing
heavy work, not few equations for their own sake.

**Role of equations:** To carry the central claim in the least space. In a PRL
the defining equation and the principal result often *are* the compression: one
displayed relation can replace the paragraph of prose the short format cannot
afford.

**Main-text mathematical content:** The defining model or governing equation;
the principal analytical result; any approximation the claim depends on, with
its validity condition; any quantity plotted in a figure.

**Supplementary mathematical content:** Derivation chains, intermediate algebra,
robustness and convergence analysis, secondary results, extended methods.

**Recommended derivation depth:** Minimal in the main text — state the starting
point, the controlled approximation, and the result; put the route in
Supplemental Material.

**Figure–equation integration:** Tight. The figure should test the equation.
Make the theory → prediction → evidence chain explicit in the caption and text,
since the reader has no room to reconstruct it.

**Recommended presentation strategy:** Run the §12 compression check of
`aps-mathematical-presentation`. If the argument cannot compress without moving
an essential equation out of the main text, that is a signal to target a
full-length article at a specialist journal rather than to cut the equation.

> `[HEURISTIC]` A single well-designed multi-panel figure often carries the
> decisive evidence in a PRL. **This is common practice, not a requirement** —
> PRL does not formally require one figure. Fetch `/prl/authors` for the actual
> formatting and length requirements, and label the three categories separately
> when advising: official requirement, common practice, recommended strategy.

## 17. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Letters | **3750 words** — about four journal pages for the core, between abstract and Acknowledgments |
| End Matter | **up to two pages**, after the references; **does not count against the core limit** |
| Essays | 3750 words |
| Comments / Replies | 750 words |

**No figure limit is stated.** The operative constraint is the word limit, which
figures consume. Never assert a figure count as a requirement.


**Article format:** Short. PRL is the portfolio's compression venue.

**Available length containers:** main text → **End Matter** → Supplemental
Material. `[REQUIREMENT]` End Matter is a PRL feature; Letters at other
*Physical Review* journals do **not** have it (they use Appendixes). Do not
carry the three-tier plan to a sibling journal.

**Typical mathematical density:** Moderate — few equations doing heavy work.

**Recommended main-text figure strategy:** `[STRATEGY]` Derive the count from
the argument, then compress hard. Evaluate explicitly whether the result can be
carried by a very small number of figures — potentially a single well-designed
multi-panel figure covering the problem, the key result, the decisive evidence,
and the implication. More figures are right when independent lines of evidence
genuinely require them. `[CONVENTION]` Compact multi-panel figures are the norm
here. **PRL does not formally require one figure** — never say it does.

**Supplementary-material role:** `[REQUIREMENT]` APS defines Supplemental
Material as information *not essential to understanding the main results*, cited
in the reference list with a brief description. Use it for validation,
robustness, extended methods. Use **End Matter** for detail specialists need
that is too central to bury — that is precisely what it exists for.

**Preferred narrative style:** Problem stated immediately; central result early;
minimal sufficient methodology; strong physical interpretation; concise
outward-pointing conclusion. `[REQUIREMENT]` The title must "clearly and
accurately convey the most important and interesting novel results," and the
abstract must concisely summarize them. `[REQUIREMENT]` A Justification
Paragraph is required at submission. `[CONVENTION]` PRL strongly encourages
titles in references — all or none.

**Recommended manuscript compactness:** High.

**Presentation priority:** Impact, innovation, and interest, conveyed "clearly
and directly" — PRL's own framing. Every paragraph should advance the central
message.

> `[REQUIREMENT]` **Joint Submissions** are permitted: a Letter here plus a
> longer Regular Article at a specialist journal. The longer paper must contain
> considerably more or different information; limited, properly referenced
> duplication of figures and text is acceptable. `[STRATEGY]` This is the right
> answer for work that is both pivotal and genuinely needs length — better than
> mutilating one manuscript to fit.

## 18. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Letters | https://journals.aps.org/prl/about | Official | 2026-08-19 | Identity, scope, acceptance criteria |
| PRL Information for Authors | https://journals.aps.org/prl/authors | Official | 2026-08-19 | Article type, length, justification statement (fetch for current detail) |
| PRL section selection | https://journals.aps.org/prl/authors/guidelines-section-selection-physical-review-letters | Official | 2026-08-19 | Sections |
| Scope of APS Journal Portfolio | https://journals.aps.org/scope | Official | 2026-08-19 | Portfolio coverage |

**Unknown — not stated in official sources:** acceptance rate, numeric length
limits (fetch), review timelines.

**Format facts above verified from** `https://journals.aps.org/prl/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
