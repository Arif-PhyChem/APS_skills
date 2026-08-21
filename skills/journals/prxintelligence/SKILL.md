---
name: aps-prxintelligence
description: Evaluate a manuscript's fit for PRX Intelligence — APS's highly selective gold open access journal for AI/ML that advances the physical sciences. Load this whenever a manuscript's central contribution is a machine-learning method, tool, dataset, or insight.
journal: PRX Intelligence
abbreviation: PRX Intelligence
journal_code: prxintelligence
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

# PRX Intelligence — Journal Skill

Load `aps-common` alongside this skill. Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`.

**Load `aps-mathematical-presentation` for every submission** — the architecture-vs-contribution distinction is mathematical, and physics-constrained formulations must be stated to be assessed. See §Mathematical presentation profile below for this journal's
calibration.

**Load `aps-format-and-presentation` whenever advising on manuscript
construction or revision** — length, figures, main-text vs Supplemental
Material, narrative style. See §Presentation profile below for this journal's
verified limits and calibration.

**Load `aps-reference-format` whenever building, reviewing, or auditing the
reference list** — numbering and citation mechanics apply portfolio-wide; check
this journal's own skill only for a journal-specific addition (PRL's
titles-in-references convention is the only one on record).

> **Portfolio-wide note.** PRX Intelligence's existence changes the neighbor
> analysis for every APS journal. Any manuscript whose central contribution is
> the AI/ML method rather than a domain result must be checked here before being
> routed to a domain journal.

## 1. Identity `[OFFICIAL]`

PRX Intelligence is "a highly selective, fully open access journal for impactful
research in artificial intelligence and machine learning (AI/ML) that advances
the physical sciences and related fields." It is "intentionally multidisciplinary
and highly visible, publishing both foundational AI/ML work and domain-driven
applications spanning physics as well as computer science and mathematics,
materials science and engineering, chemistry and biology, earth and
environmental sciences."

APS launched it "at the forefront of the Society's commitment to accelerating
scientific discovery with trustworthy, rigorous, and open research." It builds
on the legacy of PRX, combining "rigorous yet fair editorial standards with a
scope tailored to the AI/ML-for-science community," with timely, transparent
decisions on which papers proceed to review and a personalized, responsive
process.

Stated purposes `[OFFICIAL]`: a high-impact forum for the interdisciplinary
AI/ML-for-science community; connecting AI/ML researchers, physical scientists,
and engineers to the broader physics ecosystem; maximizing dissemination of
significant, timely results.

## 2. Scope `[OFFICIAL]`

Manuscripts on **AI/ML methods** as well as **their use across the physical
sciences and related fields**. Coverage spans theory, computation, and
experiment in conventional physics disciplines and related domains — computer
science and mathematics, materials science and engineering, chemistry and
biology, earth and environmental sciences — **whenever AI/ML advances a
physics-based scientific understanding or capability**.

Full scope statement including subject areas: `journals.aps.org/prxintelligence/scope`.

> `[INFERENCE]` The qualifying clause is the boundary. Pure ML research with no
> physical-science bearing belongs in the ML literature; ML applied to a physical
> science with no advance in understanding or capability meets neither the scope
> clause nor the criteria.

## 3. Acceptance criteria `[OFFICIAL]`

Submitted manuscripts should **address relevant questions, report sufficient or
state-of-the-art validation**, and demonstrate exceptional achievement in **at
least one**:

- **Exceptional advance** — introducing AI/ML concepts, results, or systems that open new and consequential directions for scientific discovery or understanding.
- **Exceptional connection** — bridging AI/ML with disparate areas of science or engineering, or unifying previously separate approaches to enable new capabilities.
- **Exceptional capabilities** — delivering tools, techniques, datasets, software, or platforms that unlock progress on major challenges (e.g., scale, interpretability, reliability, efficiency).
- **Exceptional insight** — providing clear, generalizable understanding of AI/ML behavior or scientific phenomena with high relevance across multiple communities.

> `[HEURISTIC]` Note the two **gating** requirements that precede the four
> criteria: relevant questions, and **sufficient or state-of-the-art
> validation**. A manuscript failing the validation gate cannot be rescued by a
> strong criterion claim. Check baselines, ablations, held-out evaluation,
> uncertainty, and comparison against the current state of the art *first*.

## 4. Editorial positioning `[INFERENCE]`

| Dimension | PRX Intelligence's demand |
|---|---|
| Novelty | Exceptional in at least one named dimension |
| Validation | Explicit gate — sufficient or state-of-the-art |
| Breadth | Multi-community relevance is the norm |
| Contribution type | Method, system, tool, dataset, or insight all count |
| Selectivity | High — PRX-tier standards |
| Access | Gold OA |

This is the venue where **the method is allowed to be the contribution** —
provided it is exceptional and validated. That is precisely what domain
journals such as PRB, PRMaterials, and PRE will not reward.

## 5. Strong-fit profile `[INFERENCE]`

- An AI/ML method that makes a previously intractable scientific computation or
  measurement feasible, demonstrated on a real scientific problem.
- A tool, dataset, benchmark, or platform others will build on, with evidence of
  enabling power.
- Work that unifies previously separate modeling approaches across domains.
- Generalizable insight into *why* ML models behave as they do in scientific
  settings — interpretability, reliability, scaling, failure modes.
- Foundational AI/ML work whose consequences for the physical sciences are shown,
  not asserted.

## 6. Weak-fit patterns `[HEURISTIC]`

- Standard architecture applied to a new dataset with better metrics and no
  scientific or methodological consequence.
- Benchmark-only papers with no baseline comparison or ablation.
- "First use of an LLM/GNN/transformer for X" without a demonstrated capability
  that did not exist before.
- Validation on a single dataset with no held-out or out-of-distribution test.
- A domain result where ML was merely a convenient fitting tool — route to the
  domain journal instead; the physics is the contribution there.
- Claims of interpretability without a falsifiable test of the interpretation.

## 7. The five-way AI/ML decomposition (mandatory) `[HEURISTIC]`

For every manuscript, answer separately and in writing:

1. **Method novelty** — what about the AI/ML is new?
2. **Scientific novelty** — what about the science is new?
3. **Enablement** — what became possible that was not before?
4. **Generality** — does the method transfer beyond the studied systems?
5. **Validation quality** — baselines, ablations, held-out data, uncertainty, SOTA comparison.

Routing rule:

| Pattern | Venue |
|---|---|
| (1) strong, (3) demonstrated, (5) strong | **PRX Intelligence** |
| (2) strong, (1) weak — ML is instrumentation | **Domain journal** (PRB, PRE, PRMaterials, PRA, …) |
| (1) strong, (5) weak | Not ready for either — fix validation |
| Both strong, broad and pivotal | Also consider **PRX** or **PRL** |
| Both moderate | **PRResearch** |

## 8. Evaluation framework

- **A. Scope clause** — does AI/ML advance a physics-based understanding or capability?
- **B. Validation gate** — sufficient or state-of-the-art? (blocking)
- **C. Criterion match** — which of the four, with evidence?
- **D. Decomposition** — §7, all five answered.
- **E. Multi-community relevance** — who beyond the authors' subfield benefits?
- **F. Reproducibility** — code, data, seeds, compute, licensing.
- **G. Alternatives** — domain journal, PRX, PRResearch, or the ML literature.

## 9. Fit classification `[HEURISTIC]`

| Class | Criteria |
|---|---|
| **Excellent** | Clear criterion match, strong validation, demonstrated enablement, multi-community relevance |
| **Strong** | Criterion met and validated; relevance somewhat concentrated |
| **Moderate** | Interesting method or tool; validation or enablement evidence incomplete |
| **Borderline** | Contribution is really a domain result with ML as tooling, or an ML result with thin scientific bearing |
| **Poor** | Application-of-existing-method with metric improvements only, or validation gate failed |

## 10. Neighboring journals

| Journal | Prefer it when… |
|---|---|
| **PRB / PRA / PRC / PRD / PRE / PRMaterials / PRFluids / PRApplied** | The claim is a domain result; ML is instrumentation |
| **PRX** | The advance is a physics discovery or landmark in which ML happens to feature |
| **PRX Quantum** | The work centers on quantum information science and technology (including ML *for* quantum) |
| **PRX Life** | The domain is biological/living systems, including neuroscience-AI overlap |
| **PRX Energy** | The domain is energy research |
| **PRResearch** | Solid AI/ML-for-science work that does not reach "exceptional" |
| **APS Open Science** | The output is primarily a dataset, software release, replication, or null result |
| **PRE** | The core is statistical physics of learning, or computational physics/ML within PRE's stated section |

Prefer **PRX Intelligence** when: the AI/ML contribution is the point, it is
exceptional in a named dimension, and it is validated to current standards.

## 11. Article types and requirements `[OFFICIAL]`

`[OFFICIAL]` Research Articles (no length limit); **Data/Code** (no length
limit); Perspectives (7500 words); Reviews (30,000 words); Tutorials (no length
limit); Roadmaps (no length limit); Comments/Replies (3500 words) — verified
2026-08-19.

**Data/Code is a first-class type here**, with an APS-specified structure for
Data papers (motivation, description, analysis, conclusion) and a requirement to
link or cite appropriate data repositories; Code papers must report a
substantial technical advance in scope. See §Presentation profile. Fetch
`/prxintelligence/authors` for current wording and `/prxintelligence/scope` for
subject areas. Gold open access — APC applies; waivers for authors from
lower-income countries.

## 12. Positioning advice `[HEURISTIC]`

- **Abstract** — lead with the capability unlocked, not the architecture.
- **Criterion** — name the target criterion explicitly and support it.
- **Validation section** — make it prominent: baselines (including strong
  non-ML baselines), ablations, out-of-distribution tests, uncertainty,
  compute cost, and honest failure cases.
- **Artifacts** — release code, data, weights, and configs; state licenses. For
  an "exceptional capabilities" claim, artifacts are the evidence.
- **Generality** — state which conclusions transfer and which are dataset-specific.
- **Scientific consequence** — at least one result that is a statement about the
  world, not about the model.
- Avoid the two symmetric failures: overselling architecture as discovery, and
  burying a real scientific finding under ML framing.

## 13. Submission checklist

- [ ] AI/ML advances a physics-based understanding or capability (scope clause)
- [ ] Validation gate met: baselines, ablations, held-out/OOD, uncertainty, SOTA comparison
- [ ] Named criterion with supporting evidence
- [ ] Five-way decomposition (§7) answered
- [ ] Code/data/model availability with licenses, per APS open-science policy
- [ ] Compute and reproducibility details stated
- [ ] Domain-journal alternative explicitly considered
- [ ] APC/funding or waiver eligibility settled
- [ ] AI-tool use in manuscript preparation disclosed per current APS ethics policy

## 14. Decision workflow

1. Central contribution — method, science, or tool?
2. Scope clause test. 3. Validation gate (blocking). 4. Five-way
decomposition. 5. Criterion match. 6. Multi-community relevance.
7. Reproducibility. 8. Routing rule (§7). 9. Vulnerabilities.
10. Fit class, positioning changes, confidence.

## 15. Output format

Standard portfolio output block, plus mandatory lines:

**Criterion claimed:** advance / connection / capabilities / insight — justification.
**Validation gate:** met / not met — evidence.
**Method novelty vs. scientific novelty:** …
**Enablement:** what became possible.

## 16. Mathematical presentation profile

Load `aps-mathematical-presentation`. PRX Intelligence-specific calibration
`[INFERENCE]` / `[HEURISTIC]`:

**Mathematical representation importance:** High — but pointed at the *method's
guarantees and scientific content*, not at architecture description.

**Expected equation density:** Moderate — high for theory of learning,
interpretability, and physics-constrained formulations; lower for applied
domain-driven papers.

**Role of equations:** To specify what is being learned, under what constraints,
and with what guarantees. The formal statement is what separates a method
contribution from an engineering report.

> **Model architecture ≠ scientific contribution.** Writing
> $\hat{y} = f_{\theta}(x)$ specifies almost nothing; the content is in the
> objective, the constraints, the inductive bias, and the guarantees.

**Main-text mathematical content:** The learning objective and any constraint;
the physical law imposed and its form; the loss decomposition where a
physics-constrained model is used, e.g.
$\mathcal{L}_{\mathrm{total}} = \mathcal{L}_{\mathrm{data}} + \lambda_{\mathrm{phys}}\mathcal{L}_{\mathrm{physics}}$
— **only if this genuinely represents the method**; the evaluation metrics as
defined; any bound, guarantee, or scaling claim.

**Supplementary mathematical content:** Proofs, full architecture and
hyperparameter specification, ablation detail, additional benchmarks.

**Recommended derivation depth:** State objectives, constraints, and guarantees
formally in the main text; proofs and implementation detail to appendices.

**Figure–equation integration:** Performance plots should report the metric as
mathematically defined, with uncertainty across seeds; scaling claims should
show the predicted scaling form, not only a trend.

**Recommended presentation strategy:** `[HEURISTIC]` For physics-informed or
physics-constrained models, state which physical law is imposed, whether it is
enforced exactly or penalized, how the penalty weight is chosen, and what happens
to the constraint at convergence — a physics-informed claim without a
constraint-violation measurement is unsupported. Never introduce notation the
manuscript does not use in order to assess it against a formulation its authors
never made.

## 17. Presentation profile

Load `aps-format-and-presentation` for the framework. Labels below:
**[REQUIREMENT]** = official APS rule · **[CONVENTION]** = strong practice, not a
rule · **[STRATEGY]** = this system's recommendation.

**Article types and length limits [REQUIREMENT]** *(verified 2026-08-19 — re-verify
before advising; these change)*:

| Type | Limit |
|---|---|
| Research Articles | **no length limit** |
| **Data/Code** | **no length limit** |
| Perspectives | **7500 words** |
| Reviews | **30,000 words** |
| Tutorials | no length limit |
| Roadmaps | no length limit |
| Comments / Replies | 3500 words |

**No figure limit is stated.**


**Article format:** Flexible, with a dedicated venue for artifacts.

> `[REQUIREMENT]` **Data/Code is a first-class article type here.** *Data*
> papers document novel datasets that enable new research or improve the
> community's ability to test, compare, or reproduce results; APS specifies a
> structure — **(i) Motivation**, **(ii) Description** (genesis and structure,
> an overview table of entries, format specifications, key distributions),
> **(iii) Analysis** (quality testing, curation, validation, convergence and
> consistency checks), **(iv) Conclusion** (contribution, shortcomings, future
> work) — and requires links or citations to appropriate data repositories.
> *Code* papers report code and algorithms representing a substantial technical
> advance in scope. Fetch `/prxintelligence/authors` for the current wording.
>
> `[STRATEGY]` Route a dataset or software contribution here rather than forcing
> it into a Research Article narrative. It is also the natural alternative to
> APS Open Science when the artifact is genuinely high-impact.

**Available length containers:** main text → Appendixes → Supplemental Material.

**Typical mathematical density:** Moderate; high for theory of learning and
physics-constrained formulations.

**Recommended main-text figure strategy:** `[STRATEGY]` Keep in the main text
the figures establishing the validation gate — baselines, ablations,
out-of-distribution behavior, uncertainty across seeds — and the one figure
showing the scientific consequence. Architecture diagrams are usually less
informative than authors expect; a diagram that does not explain an inductive
bias is decoration.

**Supplementary-material role:** Full hyperparameters, extended ablations,
additional benchmarks, compute accounting, proofs.

**Preferred narrative style:** Detailed exposition legible to both AI/ML and
domain readers; define notation for both.

**Recommended manuscript compactness:** Moderate.

**Presentation priority:** Validation and reproducibility made visible — with
code, data, and configurations released and licensed.

## 18. Source registry
| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| About PRX Intelligence | https://journals.aps.org/prxintelligence/about | Official | 2026-08-19 | Identity, scope, acceptance criteria |
| PRX Intelligence scope | https://journals.aps.org/prxintelligence/scope | Official | 2026-08-19 | Subject areas (fetch) |
| PRX Intelligence Information for Authors | https://journals.aps.org/prxintelligence/authors | Official | 2026-08-19 | Article types, requirements (fetch) |
| Publishing Guidelines | https://journals.aps.org/authors | Official | 2026-08-19 | Confirms title is current in the portfolio |

**Unknown — not stated in official sources:** acceptance rate, length limits (fetch), timelines, launch date specifics.

**Format facts above verified from** `https://journals.aps.org/prxintelligence/authors` **on 2026-08-19.** Length limits and article types change; re-fetch before advising an author.
