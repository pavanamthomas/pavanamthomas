# Dr. Pavanam Thomas

### PhD Economist | Quantitative Researcher & Mathematical Modeller

Quantitative Research · Statistical Analysis · Mathematical Modelling ·
Econometrics · Causal Inference · Forecasting · Optimization · AI Evaluation

I work on quantitative problems where obtaining a coefficient, forecast,
probability, optimum, or benchmark answer is only the beginning. My projects
make assumptions explicit, separate identification from estimation, test failure
modes, independently validate critical outputs, and limit conclusions to what
the design actually supports.

---

## Selected quantitative work

### [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)

How do identification assumptions fail in DiD, IV, RD and matching designs?

→ [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md)

### [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

When is a fluent quantitative answer still invalid as economics or econometrics?

→ [FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md)

### [computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)

Can a candidate solution be checked by an independent calculation rather than by repeating the same code path?

→ [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/computational-ml-stem-problem-forge/blob/main/FLAGSHIP_CASE_STUDY.md)

### [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)

Which inferential claims survive a known data-generating process?

→ [docs/statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md)

### [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models)

Does a reported optimum satisfy the programme that was actually written down?

→ [MODEL_AUDIT_CHECKLIST.md](https://github.com/pavanamthomas/optimization-decision-models/blob/main/MODEL_AUDIT_CHECKLIST.md)

### [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab)

When is a forecast validated, rather than merely well fitted in sample?

→ [FORECAST_VALIDATION_PLAYBOOK.md](https://github.com/pavanamthomas/time-series-forecasting-lab/blob/main/FORECAST_VALIDATION_PLAYBOOK.md)

Samples used in these laboratories are simulated unless a closed form is stated. Simulated recovery of a parameter is not an observational finding.

---

## Case studies

Identification, scoring, and validation write-ups sit in the repositories above. Three further notes are useful when the question is leakage, serving parity, or information-set integrity rather than an estimand:

- [CASE_STUDY_MODEL_SELECTION_FAILURE.md](https://github.com/pavanamthomas/machine-learning-model-selection-lab/blob/main/CASE_STUDY_MODEL_SELECTION_FAILURE.md) — invalid selection workflows versus the matching split
- [FLAGSHIP_POINT_IN_TIME_FAILURE.md](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab/blob/main/FLAGSHIP_POINT_IN_TIME_FAILURE.md) — features that use post-cutoff events
- [FLAGSHIP_TRAINING_SERVING_SKEW.md](https://github.com/pavanamthomas/mlops-reproducible-serving-lab/blob/main/FLAGSHIP_TRAINING_SERVING_SKEW.md) — a live endpoint whose number is not the fitted pipeline

---

## Research software

Supporting laboratories, not a second identity:

| Repository | Question |
| --- | --- |
| [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) | Which valuation and risk identities hold on closed forms or simulated series? |
| [machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab) | What risk does a given validation design actually estimate? |
| [genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab) | Can retrieval failure be separated from generation failure? |
| [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab) | Do hand derivatives, finite differences, and autograd agree away from kinks? |
| [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab) | Does a feature use only information available at the cutoff? |
| [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab) | Does serving reproduce the training-pipeline prediction on the same valid input? |

These are research programmes with tests and CI. They are not production systems, trading books, or client deployments.

---

## Formal reasoning

How can a mathematical statement be translated, proved, reviewed, and repaired in Lean without losing its intended meaning?

Compilation is not faithfulness. Lean is used here for explicit domains, quantifiers, existence versus uniqueness, and boundary cases. A compiled theorem does not establish an empirical causal claim.

For this portfolio the Lean repositories are ordered from economic modelling toward classical analysis:

### 1. [Optimization & Economic Models](https://github.com/pavanamthomas/lean4-optimization-economics)

Feasible sets, budget constraints, inequalities, and theorem-level checks of optimisation claims used in mathematical economics.

### 2. [Formalization Review](https://github.com/pavanamthomas/lean4-formalization-review)

An executable review library of semantic errors that can survive compilation: omitted hypotheses, quantifier mistakes, and repairs that keep the intended statement.

### 3. [Formalization Faithfulness](https://github.com/pavanamthomas/lean4-formalization-faithfulness)

Hidden assumptions, domain restrictions, weakening versus strengthening, and the distinction between a valid proof of the wrong claim and a faithful formalization.

### 4. [Proof Engineering](https://github.com/pavanamthomas/lean4-proof-engineering)

Structured construction, rewriting, induction, and decomposition so that assumptions and failure modes remain readable.

### 5. [Real Analysis & Topology Formalization](https://github.com/pavanamthomas/lean4-analysis-formalization)

Continuity versus uniform continuity, pointwise versus uniform convergence, compactness, and domain conditions that over-generalized statements omit.

### 6. [Proof Automation & Debugging](https://github.com/pavanamthomas/lean4-automation-debugging)

Why a tactic succeeds or fails, and whether the resulting theorem still expresses the intended mathematics.

### 7. [Mean Value Theorems](https://github.com/pavanamthomas/lean4-mean-value-theorems)

Rolle, Lagrange, and Cauchy reconstructed from the extreme value theorem and Fermat’s lemma rather than quoted as mathlib one-liners.

---

## Open work

Unfinished technical bounds are recorded in each repository’s `ROADMAP.md` and in GitHub issues. Typical remaining limits include clustered inference in the econometrics laboratory, the absence of a second-rater study in the evaluation corpus, and graded relevance in the RAG laboratory. CI checks that documented tests still run. It does not certify an observational application.

---

Python · R · SQL · statsmodels · scikit-learn · SciPy · PyTorch · Git/GitHub · Lean 4/mathlib
