# Dr. Pavanam Thomas

### PhD Quantitative Researcher & Mathematical Modeller
Econometrics · Statistics · Causal Inference · Forecasting · Optimization · Python · AI Evaluation · Formal Reasoning

I am a PhD economist and quantitative researcher. The public work is one practice at different points of the same pipeline: **identification, estimation, validation, decision modelling, evaluation of quantitative arguments, and Lean 4 formalization**.

Machine-learning laboratories below are research software with tests and CI. They record validation failures, leakage, and independent checks. Simulated data are labelled as simulated. They are not production systems and not a substitute for the Lean repositories.

A single methodological sequence is used throughout:

**Problem → formalization → assumptions → computation/estimation → validation → interpretation → limitations**

---

## Machine learning laboratories

| Repository | What a reviewer will see |
| --- | --- |
| [computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge) | Flagship: original ML/STEM problems, Python reference solutions, independent ground-truth units, adversarial audits |
| [machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab) | Invalid model-selection workflows versus the matching validation design |
| [genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab) | Retrieval metrics kept separate from generation failures in a RAG pipeline |
| [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab) | Manual NumPy backprop, finite-difference checks, PyTorch autograd |
| [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab) | Point-in-time SQL features, leaky counterparts, planted temporal sentinels |
| [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab) | Pipeline artifacts, FastAPI contract, training-serving parity and skew |

Inspect first for an ML-expert review: the problem-forge flagship case, the model-selection failure note, and the training-serving skew write-up.

---

## Computational laboratories

| Repository | What a reviewer will see |
| --- | --- |
| [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab) | Estimands, diagnostics, DiD / IV / RD / matching on documented simulated designs |
| [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation) | Inference, Monte Carlo coverage, regression pathologies, statistical-error catalogue |
| [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab) | Rolling-origin forecasts versus naive benchmarks; in-sample fit is not treated as forecast skill |
| [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models) | Programmes, solvers, independent feasibility and duality checks |
| [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) | Educational valuation, portfolios, derivatives, and risk identities |
| [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks) | Expert review of economics, econometrics, statistics, and quantitative answers |

Inspect first for applied roles: the econometrics case study, the AI-evaluation flagship review, and the statistical-error catalogue. Inspect first for formal roles: the Lean repositories below.

---

## Formal reasoning

My current formalization work is organized around a central question:

> **How can mathematical statements be translated, proved, reviewed, and repaired in Lean without losing their intended mathematical meaning?**

My background in quantitative economics and mathematical modelling informs how I approach formalization: **make the domain explicit, identify assumptions, stabilize the statement, construct the proof, and then audit both the mathematics and the formal artifact.**

---

## Lean 4 Formalization Portfolio

### 1. [Formalization Faithfulness](https://github.com/pavanamthomas/lean4-formalization-faithfulness)

A Lean 4 + mathlib study of **semantic faithfulness in mathematical formalization**.

**Focus**

- hidden assumptions and omitted hypotheses
- domain restrictions
- quantifier structure and dependency
- statement weakening and strengthening
- logically valid but semantically incorrect formalizations
- counterexample-guided diagnosis
- axiom and trust auditing
- distinction between compilation and mathematical faithfulness

**Core idea**

> A Lean theorem may compile successfully while still expressing the wrong mathematical claim.

---

### 2. [Proof Engineering](https://github.com/pavanamthomas/lean4-proof-engineering)

A structured Lean 4 + mathlib corpus focused on **reliable and maintainable proof engineering**.

**Focus**

- structured proof construction
- rewriting and equality reasoning
- algebraic proofs
- induction
- type-driven reasoning
- theorem decomposition
- proof robustness
- reviewer-oriented cases
- readable and auditable formal developments

The emphasis is not simply on obtaining a proof term, but on producing proofs whose **structure, assumptions, dependencies, and failure modes can be understood and reviewed**.

---

### 3. [Formalization Review](https://github.com/pavanamthomas/lean4-formalization-review)

An executable Lean 4 review library containing **40 formalization-review cases** for semantic errors that can survive compilation.

**Case families include**

- domain errors
- quantifier errors
- missing assumptions
- logical-structure errors
- counterexamples
- statement-faithfulness failures
- reviewer diagnostics
- semantics-preserving repairs

Candidate formalizations are treated as requiring verification, not as correct merely because Lean accepts them.

---

### 4. [Real Analysis & Topology Formalization](https://github.com/pavanamthomas/lean4-analysis-formalization)

A Lean 4 + mathlib project exploring rigorous formalization in **real analysis and topology**.

**Representative issues**

- continuity versus uniform continuity
- pointwise versus uniform convergence
- sequence limits
- uniqueness of limits
- compactness
- interval non-emptiness
- extreme-value assumptions
- square-root domain conditions
- counterexamples to over-generalized statements

The project emphasizes the relationship between a theorem's **mathematical domain, hypotheses, quantifier structure, and formal Lean statement**.

---

### 5. [Proof Automation & Debugging](https://github.com/pavanamthomas/lean4-automation-debugging)

A Lean 4 case library focused on **proof automation, debugging, theorem-search discipline, and semantics-preserving repair**.

**Focus**

- arithmetic automation
- goal-state diagnosis
- rewriting
- coercions
- tactic selection
- theorem search
- automation failure analysis
- robust proof construction
- repairing proofs without weakening the intended theorem

The objective is not merely to make a goal disappear, but to understand **why a tactic succeeds, why it fails, and whether the resulting theorem still expresses the intended mathematics**.

---

### 6. [Optimization & Economic Models](https://github.com/pavanamthomas/lean4-optimization-economics)

A Lean 4 + mathlib project connecting formal verification with **optimization and mathematical economic modelling**.

**Focus**

- optimization arguments
- inequalities
- feasible sets
- budget constraints
- model assumptions
- edge cases
- domain restrictions
- theorem-level verification of economic and quantitative claims

This repository connects my quantitative economics background with formal mathematical reasoning and verification.

---

### 7. [Mean Value Theorems](https://github.com/pavanamthomas/lean4-mean-value-theorems)

A Lean 4 + mathlib reconstruction of three named calculus theorems: **Rolle's theorem**, **Lagrange's mean value theorem**, and **Cauchy's mean value theorem**.

**Focus**

- interior extrema on a compact interval when endpoint values agree
- Fermat's interior-extremum lemma
- Rolle as a vanishing derivative at that interior point
- Lagrange via an affine correction reducing to Rolle
- Cauchy in product form, without a `g' c ≠ 0` side condition

mathlib already contains these results. This repository records the classical argument from the extreme value theorem and Fermat, rather than quoting the library one-liners.

---

## Verification-First Workflow

Across the portfolio, I use a workflow designed to separate **proof acceptance** from **mathematical faithfulness**.

```text
Natural-language mathematical claim
        ↓
Domain and assumption audit
        ↓
Quantifier / dependency analysis
        ↓
Canonical Lean statement
        ↓
Proof construction or repair
        ↓
Lean compilation
        ↓
Placeholder checks
        ↓
Axiom / trust audit
        ↓
Semantic-faithfulness review
        ↓
Pull-request CI
        ↓
Merge to main
        ↓
Independent main-branch CI
```
