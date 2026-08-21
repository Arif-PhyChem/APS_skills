---
name: aps-prper
description: Evaluate a manuscript's fit for Physical Review Physics Education Research — experimental and theoretical research on the teaching and learning of physics and astronomy.
journal: Physical Review Physics Education Research
abbreviation: PRPER
journal_code: prper
publisher: American Physical Society
access_model: open access
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
source_domain: journals.aps.org
source_verified: true
requires: [aps-common]
companion_skills: [aps-mathematical-presentation, aps-format-and-presentation, aps-reference-format]
---

# Physical Review Physics Education Research — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` when a statistical or measurement model carries the claim** — here the relevant mathematics is inferential, not physical. See §Mathematical presentation profile below for this journal's
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

PRPER is "a trusted open access journal for high-quality, significant
experimental and theoretical research related to the teaching and learning of
physics and astronomy." It publishes detailed research articles, **review
articles**, and **replication studies**, and explicitly welcomes "descriptions
of the development and use of new assessment tools, presentation of research
techniques, and methodology comparisons or critiques." Flexible article lengths;
longer papers welcome.

> `[HEURISTIC]` Explicit welcome of **replication studies** and **methodology
> critiques** is unusual and worth using: these are first-class submissions here,
> not fallbacks.

## 2. Scope `[OFFICIAL]`

All educational levels, from elementary through graduate education. All topics
in experimental and theoretical physics education research, including but not
limited to:

- Educational policy
- Instructional strategies, and materials development
- Research methodology
- Epistemology, attitudes, and beliefs
- Learning environment
- Scientific reasoning and problem solving
- Diversity and inclusion
- Learning theory
- Student participation
- Faculty and teacher professional development

## 3. Acceptance criteria `[OFFICIAL]`

- Present results of importance to the field.
- Generate interest for PRPER's readers.
- Represent an authoritative and substantive addition to the body of literature.

## 4. Editorial positioning `[INFERENCE]`

PRPER is a **research** journal, not a teaching-practice magazine. The
distinction that decides most submissions: a curriculum or activity description
is not research; a study of what students learn, how, and why — with a
methodology and evidence — is.

## 5. Strong-fit profile `[INFERENCE]`

- Studies with a clear research question, appropriate design, and adequate sample.
- Validated assessment instruments with reliability and validity evidence.
- Theory-grounded analyses of learning, reasoning, or participation.
- Replications that test the robustness of established results.
- Methodological work that improves how PER is conducted.
- Equity and inclusion research with rigorous, ethical design.

## 6. Weak-fit patterns `[HEURISTIC]`

- "We tried this in our course and students liked it" — satisfaction is not learning.
- Pre/post gains with no control, no comparison, and no accounting for confounds.
- Instruments used without validity evidence.
- Small samples with strong general claims.
- Missing theoretical framing or disconnection from prior PER literature.
- No statement of ethics approval or participant consent where required.

## 7. Evaluation framework

**A. Scope fit** (physics/astronomy education research) · **B. Research
question** clarity · **C. Methodology** appropriateness · **D. Evidence and
analysis** rigor · **E. Theoretical grounding** · **F. Transferability** beyond
one course · **G. Ethics and reporting standards.**

## 8. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Important, well-designed study with rigorous evidence and clear implications for the field |
| **Strong** | Clearly in scope; sound design and analysis; meaningful contribution |
| **Moderate** | In scope; methodology, sample, or theoretical framing needs strengthening |
| **Borderline** | Practice description with some evidence; not yet a research contribution |
| **Poor** | Course anecdote, or claims unsupported by the design |

## 9. Neighboring venues

`[INFERENCE]` PRPER has little overlap inside the *Physical Review* portfolio;
its neighbors are mostly external education-research journals.

| Venue | Prefer it when… |
|---|---|
| **APS Open Science** | The output is a dataset, instrument release, or null result rather than a study |
| **PRResearch** | The work is physics research that happens to involve teaching contexts |
| **External PER/education journals** | The audience is general science education rather than physics/astronomy specifically |

Prefer **PRPER** when: the work is research on physics or astronomy teaching
and learning, at any educational level.

## 10. Article types `[OFFICIAL]`

Detailed **research articles**, **review articles**, and **replication
studies**. Also welcomed: assessment-tool development and use, research
techniques, and methodology comparisons or critiques. Flexible lengths.

## 11. Positioning advice `[HEURISTIC]`

- State the research question and theoretical framework early and explicitly.
- Describe context, population, and sampling fully enough to judge transferability.
- Report effect sizes and uncertainty, not only p-values.
- Provide validity and reliability evidence for every instrument.
- Address ethics approval and consent.
- Say what the field should do differently as a result.

## 12. Submission checklist

- [ ] Research question and framework stated
- [ ] Design appropriate to the question; comparison/control considered
- [ ] Instruments validated; validity evidence reported
- [ ] Effect sizes and uncertainty reported
- [ ] Context and population described for transferability
- [ ] Ethics approval and consent addressed
- [ ] Article type chosen (research / review / replication)
- [ ] Data availability per APS open-science policy, with participant privacy protected
- [ ] AI-tool use disclosed per current APS ethics policy

## 13. Decision workflow

1. Central contribution. 2. Research-vs-practice test. 3. Scope fit.
4. Methodology appropriateness. 5. Evidence rigor. 6. Theoretical grounding.
7. Transferability. 8. Ethics. 9. Fit class, positioning, confidence.

## 14. Output format

Standard portfolio output block, plus:
**Research vs. practice:** why this is a research contribution.
**Methodological rigor:** design, sample, analysis.

## 15. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRPER-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** Low for physics formalism; **high
for statistical and measurement models**. The mathematics that matters here is
inferential, not physical.

**Expected equation density:** Low. Statistical models are usually specified in
text and tables rather than as displayed equations.

**Role of equations:** To specify the measurement and inference model — item
response models, factor structures, regression or multilevel specifications,
and effect-size definitions — precisely enough to be evaluated and replicated.

**Main-text mathematical content:** The statistical model specification
including random effects and covariates; effect-size definitions; reliability
and validity statistics; any scoring model for an assessment instrument.

**Supplementary mathematical content:** Full model output, sensitivity analyses,
alternative specifications, instrument scoring detail.

**Recommended derivation depth:** Minimal — cite established statistical
methods rather than deriving them.

**Figure–equation integration:** Plots should report uncertainty and identify
the model that generated fitted lines or predicted values.

**Recommended presentation strategy:** `[HEURISTIC]` Specify the statistical
model completely rather than naming a test — under-specified models are a
standard PRPER referee objection. Report effect sizes with uncertainty, not only
p-values. Physics content appearing in the manuscript (the material students are
learning) should be presented at the level the study requires, not elaborated
for its own sake.

## 16. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| Review Articles | **no length limit** |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Full-length; no length limit on research articles.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Low for physics formalism; the relevant
formal content is statistical (see §Mathematical presentation profile).

**Recommended main-text figure strategy:** `[STRATEGY]` Education-research
figures should report uncertainty and identify the model behind fitted values.
Instruments, coding schemes, and full item statistics belong in Supplemental
Material; the analysis that supports the central claim belongs in the main text.

**Supplementary-material role:** Instruments, interview protocols, coding
schemes, full model output, sensitivity analyses — subject to participant
privacy.

**Preferred narrative style:** Detailed exposition in the conventions of
education research: explicit research questions, theoretical framework, methods,
results, limitations. `[CONVENTION]` Context and population must be described
fully enough for readers to judge transferability.

**Recommended manuscript compactness:** Low — completeness of method reporting
matters more than brevity.

**Presentation priority:** Methodological transparency and ethics reporting.

## 17. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About Physical Review Physics Education Research | https://journals.aps.org/prper/about | Official | 2026-08-19 | Identity, scope, criteria, article types |
| PRPER Information for Authors | https://journals.aps.org/prper/authors | Official | 2026-08-19 | Requirements (fetch) |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines.

**Format facts above verified from** `https://journals.aps.org/prper/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
