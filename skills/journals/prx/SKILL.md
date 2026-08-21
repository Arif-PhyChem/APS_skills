---
name: aps-prx
description: Evaluate a manuscript's fit for Physical Review X — APS's highly selective, flexible-length gold open access journal for breakthrough and paradigm-shifting physics.
journal: Physical Review X
abbreviation: PRX
journal_code: prx
publisher: American Physical Society
access_model: gold open access
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation, aps-reference-format]
---

# Physical Review X — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for theoretical, computational, or tool/database submissions** — at this tier the formalism is part of the evidence for a field-defining claim. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

**Load `aps-reference-format` whenever building, reviewing, or auditing the
reference list** — numbering and citation mechanics apply portfolio-wide; check
this journal's own skill only for a journal-specific addition (PRL's
titles-in-references convention is the only one on record).

## 1. Identity `[OFFICIAL]`

PRX is "the world's leading open access journal for cutting-edge research across
physics and adjacent fields," a premier venue among APS journals, highly
selective, with a diverse readership. It showcases research in established core
areas "that achieves breakthroughs in technology, experiment, and theory, or
that represents a paradigm shift in understanding," and also publishes
"creative, impactful research that brings together multiple physics fields, or
bridges physics with other disciplines."

PRX is known for a "highly personalized and responsive editorial process" —
authors, editors, and referees in interactive, reasoned dialog. It offers
**flexible article lengths and formats**, recognizing that "not all research can
be adequately described in only a few pages."

## 2. Scope `[OFFICIAL]`

All of physics and adjacent fields, including interdisciplinary work bridging
physics with other disciplines. Scope is not the discriminator; §3 is.

## 3. Acceptance criteria `[OFFICIAL]`

Submitted manuscripts should meet **one or more**:

- Makes a fundamental experimental or theoretical discovery
- Defines a landmark in a fast moving topic area
- Establishes key new connections between subfields or between other scientific disciplines and physics
- Propels an established field in an important new direction
- Significantly advances the state of the art of a field
- Creates a new paradigm or develops a paradigm shift of a field
- Provides high impact community tools or databases that enable substantial advances in a field

> `[HEURISTIC]` The seventh criterion is unusual and under-used: PRX explicitly
> values **high-impact community tools and databases**. For infrastructure-type
> work — a dataset, benchmark, or code that others will build on — PRX is a
> legitimate target, provided the "enables substantial advances" clause is
> evidenced by adoption potential, not asserted.

## 4. Editorial positioning `[INFERENCE]`

| Dimension | PRX's demand |
|---|---|
| Novelty | Very high — discovery or landmark |
| Significance | Field-defining, not merely field-advancing |
| Breadth | Broad and often cross-disciplinary |
| Length | Flexible — depth is welcome, unlike PRL |
| Evidence | Must withstand a dialogic, demanding review |
| Access | Gold OA; APC applies |

**PRL vs PRX** `[INFERENCE]`: both are top-tier, and the discriminator is not
only importance but **form**. PRL asks for compression to a short, pivotal
report. PRX accommodates work whose case requires length, multiple lines of
evidence, or a package of results. When the argument is inseparable from its
depth, PRX is the more natural venue.

## 5. Strong-fit profile `[INFERENCE]`

- A fundamental discovery with complete, multi-pronged evidence.
- A definitive treatment that reorients a fast-moving area.
- Work that creates a genuine bridge between subfields or into another discipline.
- A tool/dataset/benchmark with demonstrated enabling power.
- A theoretical framework that changes how a field poses its questions.

## 6. Weak-fit patterns `[HEURISTIC]`

- Strong subfield contribution without field-level consequence.
- Length used for thoroughness rather than for a bigger claim.
- Cross-disciplinary framing asserted in the introduction but absent from the results.
- A tool paper with no evidence anyone else can or will use it.
- Overclaimed "paradigm shift" language unsupported by the results.

## 7. Evaluation framework

- **A. Criterion match** — name which of the seven, with evidence.
- **B. Discovery vs. advance** — is this new knowledge or better knowledge?
- **C. Field-level consequence** — what changes for the field, not the subfield?
- **D. Connections** — real bridge, or rhetorical one?
- **E. Depth justification** — does the work need PRX's flexible length?
- **F. Evidence completeness** — will it survive dialogic review?
- **G. Alternatives** — PRL (shorter/pivotal), the domain PRX title, PRResearch, or the specialist journal.

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Clear discovery/landmark/paradigm claim, fully evidenced, broad consequence |
| **Strong** | Meets a criterion with real field-level impact; evidence solid |
| **Moderate** | Important work whose field-level significance depends on framing or on results not yet in the paper |
| **Borderline** | Excellent subfield work; PRResearch or the specialist journal is more natural |
| **Poor** | Incremental or subfield-bounded; criteria not reachable without overclaiming |

## 9. Neighboring APS journals

| Journal | Prefer it when… |
|---|---|
| **PRL** | The pivotal message compresses to a short Letter and breadth of immediate interest is the strength |
| **PRX Quantum** | The advance is specifically in quantum science and technology |
| **PRX Intelligence** | The advance is AI/ML for the physical sciences |
| **PRX Energy / PRX Life** | Energy, or biology-physics interface, is the defining domain |
| **PRResearch** | The work is significant and gold OA is wanted, but the field-defining bar is not met |
| **Specialist journals (PRA–PRE, PRMaterials, PRApplied, PRFluids, PRAB)** | Significance is real but confined to a research area |
| **RMP** | It is a review or colloquium |

Prefer **PRX** when: the claim is field-defining, the audience is broad or
cross-disciplinary, and the case needs room to be made.

## 10. Article types and requirements `[OFFICIAL]`

PRX offers flexible article lengths and formats. Current article types, length
guidance, and required components: fetch `/prx/authors`. PRX is gold open
access — an APC applies; see `journals.aps.org/authors/apcs`. Waivers exist for
authors from lower-income countries.

## 11. Positioning advice `[HEURISTIC]`

- Lead with the discovery, not the campaign of work that produced it.
- Make the criterion claim explicit and falsifiable in the abstract.
- If claiming a bridge between fields, deliver results that both fields need —
  a shared method is not a bridge.
- If claiming a community tool, show enabling evidence: what became possible.
- Use the flexible length for *completeness of argument*, not for volume.
- Retire unsupported "paradigm" language; at this tier it reads as weakness.

## 12. Submission checklist

- [ ] Named criterion from §3, with supporting result
- [ ] Field-level (not subfield-level) consequence argued
- [ ] Evidence complete across independent lines
- [ ] Length justified by the argument
- [ ] APC/funding for gold OA settled, or waiver eligibility checked
- [ ] Data/code availability per APS open-science policy
- [ ] Alternatives (PRL, domain PRX title, PRResearch) explicitly considered
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Criterion claimed. 3. Discovery vs. advance.
4. Field-level consequence. 5. Cross-disciplinary reality check.
6. Depth justification. 7. Evidence completeness. 8. Neighbor comparison
(PRL first, then domain PRX titles, then PRResearch). 9. Vulnerabilities.
10. Fit class, positioning changes, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Criterion claimed:** *(one of the seven, verbatim)* — with justification.
**Why PRX rather than PRL:** *(form and depth argument)*

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRX-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High, and highly topic-dependent
across a portfolio-wide scope.

**Expected equation density:** Moderate to high — PRX's flexible length means
density should follow the science rather than a format constraint.

**Role of equations:** To establish the framework completely enough that a
field-defining claim is checkable. At this tier the mathematics is part of the
evidence that the claim is as general as asserted.

**Main-text mathematical content:** Full defining framework, principal results,
and the key steps of any argument the claim rests on. PRX explicitly
accommodates work that "cannot be adequately described in only a few pages" —
use that room for the argument, not for volume.

**Supplementary mathematical content:** Routine algebra, auxiliary proofs,
numerical implementation detail, secondary limits and special cases.

**Recommended derivation depth:** Moderate to full — enough that a specialist
can follow the logic in the main text without reconstructing it.

**Figure–equation integration:** Multiple independent lines of evidence are
common at this tier; each should connect to the formulation explicitly.

**Recommended presentation strategy:** Use flexible length for completeness of
argument. Where the contribution is a **community tool or database** (an
explicit PRX criterion), the mathematical specification of what the tool
computes — its definitions, guarantees, and limits — is part of the
contribution, not an appendix to it.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Perspectives | **7500 words** |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Flexible length by design — PRX states that not all research
can be adequately described in a few pages.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate to High, topic-dependent.

**Recommended main-text figure strategy:** `[STRATEGY]` At this tier a
field-defining claim usually needs several independent lines of evidence, and
each deserves main-text visibility. Use the absence of a length limit for
*completeness of argument*, not volume — a figure that does not advance the
central claim still costs the reader.

**Supplementary-material role:** Auxiliary proofs, implementation detail,
additional systems, extended benchmarks.

**Preferred narrative style:** Detailed exposition with a clearly foregrounded
central claim; accessible to a broad and often cross-disciplinary readership.

**Recommended manuscript compactness:** Low to Moderate — depth is welcome,
padding is not.

**Presentation priority:** Making the field-level significance visible and
checkable. `[STRATEGY]` For a community-tool or database contribution — an
explicit PRX criterion — document what the tool computes and its limits as
carefully as a result.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review X | https://journals.aps.org/prx/about | Official | 2026-08-19 | Identity, positioning, acceptance criteria |
| PRX Information for Authors | https://journals.aps.org/prx/authors | Official | 2026-08-19 | Article types, requirements (fetch for detail) |
| APS APCs | https://journals.aps.org/authors/apcs | Official | 2026-08-19 | Gold OA charges |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prx/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
