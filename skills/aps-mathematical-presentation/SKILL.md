---
name: aps-mathematical-presentation
description: Evaluate and improve how equations, derivations, and quantitative arguments function as scientific content in an APS manuscript — what the central contribution's mathematical object is, which equations belong in the main text, and how formulation connects to figures. Load alongside any journal skill for theoretical, computational, or equation-driven work.
publisher: American Physical Society
scope: portfolio-wide
version: 2026-08-19
last_verified: 2026-08-19
refresh_interval_days: 90
requires: [aps-common]
---

# APS Mathematical Presentation

Load `aps-common` and the target journal's skill. Every journal skill carries a
**Mathematical presentation profile**; this skill is the reasoning engine behind
those profiles.

Tags: `[OFFICIAL]` / `[INFERENCE]` / `[HEURISTIC]`. Almost everything here is
`[HEURISTIC]` or `[INFERENCE]` — APS states formatting and style requirements,
not editorial doctrine about how much mathematics a paper should carry. Never
present the guidance below as APS policy.

## 1. Core principle

> **Mathematical precision + physical clarity + editorial economy.**

Equations are not formatting. For most *Physical Review* theory and computation,
mathematical formulation *is* the scientific communication.

Two symmetric failures to prevent:

- **Do not remove equations to shorten a manuscript.** Cutting the defining
  equation to meet a length limit destroys the paper to fit the box.
- **Do not add equations to look rigorous.** Algebra that does not advance the
  argument is overhead, and referees read it as padding.

The correct mathematical representation is the one that communicates the
contribution most clearly and efficiently *to this journal's readership*.

## 2. The central question

Ask first, before any critique of style:

> **What is the mathematical object, equation, relation, or model that expresses
> the central scientific contribution?**

If the manuscript has one and never writes it down, that is the finding — a
prose description of a Hamiltonian, a governing equation, or a scaling relation
is almost always weaker than the object itself.

If the manuscript genuinely has no such object (a measurement paper, a materials
characterization, a review), say so and stop. Not every APS paper is
equation-driven, and demanding mathematics of a paper that does not need it is
its own failure mode.

Common forms the object takes:

| Contribution | Typical object |
|---|---|
| New model | A Hamiltonian, Lagrangian, or free-energy functional |
| New dynamics | An equation of motion, master equation, or governing PDE |
| New relation | A scaling law, sum rule, or closed-form relation between observables |
| New quantity | A definition, with the properties that make it well posed |
| New approximation | The controlled expansion and its validity condition |
| New method | The estimator, update rule, or variational principle |
| Theory–experiment link | The observable expressed in terms of model parameters |

## 3. Every important equation must do work

Each displayed equation should serve an identifiable purpose:

- define the physical model;
- establish the theoretical framework;
- express the central result;
- introduce a new quantity;
- relate observables;
- derive a prediction;
- explain a mechanism;
- define an approximation and its regime;
- connect theory with experiment or simulation.

**Audit rule** `[HEURISTIC]`: for each displayed equation, name its purpose from
that list. An equation with no purpose is either supporting material, appendix
material, or deletable. Routine algebraic expansion that does not advance the
argument is the most common offender.

## 4. Equation hierarchy

Classify every equation into exactly one tier.

| Tier | Definition | Placement |
|---|---|---|
| **Essential** | Required to understand the central scientific argument, or to interpret a figure | Main text, always |
| **Supporting** | Needed for methodological completeness but not for the main message | Main text if short; otherwise combine, shorten, or move |
| **Derivational** | Intermediate steps, routine manipulations, standard proofs | Appendix or Supplemental Material where the format permits |

**Hard rule** `[HEURISTIC]`: **never move an essential equation to the
supplement to satisfy a length limit.** If the essential equations do not fit
the format, the manuscript is aimed at the wrong article type — that is a
placement finding, not a formatting one.

Test for essentiality: remove the equation and read the paper. If a central
claim becomes ambiguous, or a figure becomes uninterpretable, it is essential.

## 5. Main text versus supplement

**Main text** — defining equations; the central theoretical framework; key
approximations and their validity conditions; the principal analytical result;
anything required to read the figures.

**Supplement** — lengthy derivations; algebraic intermediate steps; additional
proofs; convergence and robustness analysis; secondary analytical results;
extended methodological detail.

Check the journal's current supplemental-material policy before advising on the
split; APS states requirements there, and they are journal-specific.

`[HEURISTIC]` A well-organized theory paper often reads: defining equations →
approximation and its regime → principal result → what the result implies →
figure testing it, with two to four displayed equations in the main text carrying
the argument and the derivation chain in an appendix.

## 6. Compact mathematical communication

For short-format work — PRL, and Letters at the specialist journals — favor
compactness. The goal is not fewer equations:

> Express the maximum scientifically important information with the minimum
> unnecessary mathematical overhead.

A compact equation can replace several paragraphs. Rather than describing a
dynamical relationship verbally across a paragraph, state it —

$$\dot{\mathbf{x}} = \mathbf{F}(\mathbf{x};\boldsymbol{\theta})$$

— and then spend the prose on what the quantities mean and what the relation
implies. Compression techniques that preserve content: define notation once in a
table or a single sentence; use vector/matrix form over component-wise
expansion; state a result and cite the derivation to an appendix; fold repeated
structure into a single general expression.

Compression that destroys content — dropping the validity condition, hiding the
approximation, omitting the definition of a symbol — is not compression.

## 7. Equation plus physical interpretation

Never present an important equation without interpretation. For each, the text
should make clear:

1. what it represents;
2. what the important variables and parameters mean;
3. what physical assumption is embedded;
4. what it implies;
5. why it matters for the central result.

`[HEURISTIC]` **Discourage equation dumping.** A page of displayed expressions
with no connective physical narrative is a recognizable weakness, and referees
name it. Mathematical sophistication and physical clarity are not in tension; a
manuscript that has one and not the other is incomplete.

Symptoms to flag: symbols used before definition; an approximation introduced
without its regime of validity; a limit taken without saying why it is the
relevant one; a result stated with no sentence on what it means physically.

## 8. Mathematical density

Estimate the appropriate density for the journal *and* the research area:

| Level | Character |
|---|---|
| **Low** | Equations occasional; the argument is carried by measurement or observation |
| **Moderate** | A defining framework plus principal results; derivations mostly in appendices |
| **High** | Mathematics carries the argument throughout; substantial derivation in the main text |
| **Very high** | The manuscript is essentially a mathematical development |

`[HEURISTIC]` **High density is not automatically better.** The correct density
follows the contribution. An experimental paper with very high density is
usually misorganized; a theory paper with low density is usually under-specified.
Judge the mismatch, not the level.

## 9. Figure–equation integration

For equation-driven papers, evaluate the chain:

```
Theory / Model  →  Prediction  →  Numerical or experimental evidence
```

The manuscript should make each arrow explicit. A strong figure demonstrates,
tests, visualizes, or quantifies something introduced mathematically — and its
caption or axis labels should refer to the equation that defines the plotted
quantity.

Flag: figures that display data with no stated connection to the theoretical
argument; predictions never tested by any figure; figures plotting quantities
never mathematically defined; a defining equation whose consequences are never
shown.

## 10. Mathematical novelty — four distinct kinds

Distinguish these explicitly; they carry different scientific weight, and
conflating them is a standard overclaim.

| Kind | What it is |
|---|---|
| **New mathematics** | A new method, formalism, theorem, or analytical framework |
| **New physical theory** | A formulation representing genuinely new physical understanding |
| **New solution** | A new analytical or numerical solution of an existing model |
| **New application** | An established framework applied to a new physical system |

`[HEURISTIC]` **Mathematical complexity is not scientific novelty.** A long,
difficult calculation within an established framework is a new solution, not a
new theory — and should be positioned as such. Equally, a simple equation can
express a genuinely new physical idea; brevity is not weakness.

Name which kind the manuscript offers, in one sentence, and check that the
abstract claims that kind and no more.

## 11. AI/ML manuscripts

> **Model architecture ≠ scientific contribution.**

Where useful, identify the method's mathematical representation — for a learned
map, $\hat{y} = f_{\theta}(x)$; for a physics-constrained objective,

$$\mathcal{L}_{\mathrm{total}} = \mathcal{L}_{\mathrm{data}} + \lambda_{\mathrm{phys}}\,\mathcal{L}_{\mathrm{physics}}$$

— **but only when such a formulation genuinely represents the method described.**
Direct the editorial assessment at what the formulation *enables scientifically*,
not at its sophistication.

For physics-informed or physics-constrained models, require the manuscript to
state: which physical law is imposed and in what form; whether it is enforced
exactly or penalized; how $\lambda_{\mathrm{phys}}$ or its analogue is chosen;
and what happens to the physical constraint at convergence.

**Never introduce notation that is not present in, or justified by, the
manuscript.** Writing an equation the authors did not write, and then assessing
them against it, is fabrication.

## 12. Short-format compression check

For PRL-type manuscripts and specialist-journal Letters, test whether the
argument compresses to:

1. a clearly defined physical problem;
2. a compact mathematical formulation;
3. one or a few decisive results;
4. a concise physical interpretation;
5. a clear statement of broader significance.

A single well-designed multi-panel figure may carry the decisive evidence.

> `[HEURISTIC]` **Do not state that PRL formally requires one figure.** It does
> not. Keep three things separate and label them when advising:
> **official formatting requirements** (fetch from the journal's author page),
> **common presentation practice** (observable in published papers),
> and **recommended editorial strategy** (this skill's advice).

If the argument cannot compress without moving an essential equation out of the
main text, recommend the full-length article type instead.

## 13. Output format

Report as the **Mathematical presentation profile**, using the same fields the
journal skills carry:

**Central mathematical object:** the equation/relation expressing the contribution — or "none; the contribution is not equation-driven."
**Mathematical representation importance:** Low / Moderate / High / Very High
**Expected equation density:** Low / Moderate / High *(and the manuscript's actual density, if assessing one)*
**Role of equations:** what the mathematics is doing in this manuscript
**Main-text mathematical content:** what must stay
**Supplementary mathematical content:** what can move
**Recommended derivation depth:** how much to show, and where
**Figure–equation integration:** how the chain is or is not made explicit
**Mathematical novelty kind:** new mathematics / new physical theory / new solution / new application
**Equation audit:** any displayed equation with no identifiable purpose
**Interpretation gaps:** important equations presented without physical reading
**Recommended presentation strategy:** concrete changes

## 14. Rules

1. Never invent an equation for a manuscript. Work only with what is there, or
   recommend that the authors write down an object they clearly possess.
2. Never present density or hierarchy advice as APS policy.
3. Never recommend moving an essential equation to the supplement for length.
4. Never equate mathematical complexity with novelty or significance.
5. Fetch the journal's supplemental-material and formatting requirements before
   advising on placement; do not assert limits from memory.
6. When a manuscript is not equation-driven, say so rather than manufacturing
   mathematical criticism.

## 15. Source registry

| Source | URL | Type | Accessed | Used for |
|---|---|---|---|---|
| APS Editorial Policies and Practices | https://journals.aps.org/authors/editorial-policies | Official | 2026-08-19 | Supplemental material, common policy |
| Journal author pages | https://journals.aps.org/<code>/authors | Official | 2026-08-19 | Formatting, length, supplemental policy (fetch at use time) |
| APS Style Guide / Tips for Authors | https://journals.aps.org/authors/tips-authors-physical-review-physical-review-letters | Official | 2026-08-19 | Presentation guidance (fetch for current wording) |

**Unknown — not stated in official sources:** any editorial threshold on
equation count, density, or derivation length. All such guidance here is
`[HEURISTIC]`.
