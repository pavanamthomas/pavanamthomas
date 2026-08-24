# Dr. Pavanam Thomas

### PhD Quantitative Researcher | Economics · Statistics · Machine Learning · Mathematical Modelling · AI Evaluation

I work on quantitative problems where obtaining a coefficient, forecast, prediction, optimum, or AI-generated answer is only the beginning. My public work spans econometrics and causal inference, statistical validation, computational machine learning, scientific Python, optimisation, SQL information-set integrity, RAG evaluation, and independent ground-truth verification.

Across these areas I use the same discipline:

**target → assumptions → method → implementation → failure analysis → independent validation → bounded interpretation**

The repositories are meant to be inspectable technical work, not a list of technologies. Tests, CI, issues, roadmaps, deliberate failures, and correction notes are retained because they show what was checked, what broke, and what remains unresolved.

---

## Choose the relevant portfolio path

### [Economics Expert / PhD Quantitative Research](ECONOMICS_EXPERT_PORTFOLIO.md)
Econometrics · Causal Inference · Statistical Analysis · Forecasting · Mathematical Modelling · Optimisation · AI Evaluation

### [Machine Learning Expert / Computational STEM](MACHINE_LEARNING_EXPERT_PORTFOLIO.md)
Python · Machine Learning · Model Validation · Ground-Truth Engineering · SQL · GenAI/RAG · PyTorch · MLOps

---

## Technical questions I can defend

- Why can an inner cross-validation score be optimistic even when there is no obvious train/test overlap?
- How should stochastic ground truth be verified when exact numerical equality is scientifically inappropriate?
- How can Recall-at-k improve while a RAG answer becomes worse?
- How can SQL leak future information without ever selecting the label column?
- When finite differences and PyTorch autograd disagree, how do I determine whether the failure is analytical, numerical, or implementation-specific?
- Why can an API return HTTP 200 while its served probability differs from the fitted training pipeline?
- Why can a numerically correct final answer still fail a technical-evaluation rubric?
- When does an econometric design justify causal interpretation rather than association?

Each question above maps to code, tests, or a documented case study in the repositories below.

---

## Selected quantitative and computational work

### [computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)
Can a computational ML/STEM answer be checked by independent objects rather than by repeating the same code path?

→ [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/computational-ml-stem-problem-forge/blob/main/FLAGSHIP_CASE_STUDY.md)

### [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)
What estimand is identified, under which assumptions, and what breaks when those assumptions fail?

→ [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md)

### [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)
When is a fluent quantitative answer still invalid because the target object, assumptions, method, or interpretation are wrong?

→ [FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md)

### [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)
Which inferential claims survive a known data-generating process?

→ [docs/statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md)

### [machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab)
What risk does a validation design actually estimate, and where do leakage and selection bias enter?

→ [CASE_STUDY_MODEL_SELECTION_FAILURE.md](https://github.com/pavanamthomas/machine-learning-model-selection-lab/blob/main/CASE_STUDY_MODEL_SELECTION_FAILURE.md)

### [genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab)
Can retrieval, context-packing, and generation failures be separated and diagnosed?

→ [FLAGSHIP_RAG_FAILURE_ANALYSIS.md](https://github.com/pavanamthomas/genai-rag-evaluation-lab/blob/main/FLAGSHIP_RAG_FAILURE_ANALYSIS.md)

---

## Further research software

| Repository | Question |
| --- | --- |
| [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab) | Does a feature use only information available at the prediction cutoff? |
| [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab) | Do hand derivatives, finite differences, and autograd agree away from kinks? |
| [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab) | Does serving reproduce the fitted training pipeline on the same valid input? |
| [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab) | Is forecast performance genuinely out-of-sample and free of future-data leakage? |
| [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models) | Does a reported optimum satisfy the programme actually written down? |
| [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) | Which valuation and risk identities survive closed-form or simulated checks? |

Samples in the Python laboratories are documented simulated DGPs or closed forms unless explicitly stated otherwise. They are used because the true target can be known and a wrong procedure can be shown to fail. Recovering a simulated parameter is not an empirical finding.

The ML-facing repositories are implementation evidence, not claims of commercial deployment. Where a system is local, synthetic, offline, or incomplete, the README and roadmap say so.

---

## How the repositories are developed

I keep the development trail deliberately technical rather than cosmetic:

- meaningful commits tied to an implemented change, test, correction, or documented limitation;
- automated tests that check properties and failure modes rather than only whether a function returns;
- CI where the repository has an executable workflow;
- issues and roadmaps for unresolved bounds rather than pretending the work is complete;
- failure-and-correction notes that preserve mistakes worth learning from;
- reproducibility scripts and generated outputs that can be rebuilt from source;
- explicit non-claims around simulated data, causality, deployment, and production use.

I avoid generic project templates, decorative comments, boilerplate technology lists, and manufactured commit activity. The intent is that a reviewer can follow a real technical question from formulation to implementation, failure, correction, and remaining limitation.

---

## Formal reasoning

How can a mathematical statement be translated, proved, reviewed, and repaired in Lean without losing its intended meaning?

Compilation is not faithfulness. Lean is useful here because domains, quantifiers, existence versus uniqueness, and boundary conditions must be explicit. A compiled theorem does not establish an empirical causal claim.

- [lean4-optimization-economics](https://github.com/pavanamthomas/lean4-optimization-economics)
- [lean4-formalization-review](https://github.com/pavanamthomas/lean4-formalization-review)
- [lean4-formalization-faithfulness](https://github.com/pavanamthomas/lean4-formalization-faithfulness)
- [lean4-proof-engineering](https://github.com/pavanamthomas/lean4-proof-engineering)
- [lean4-analysis-formalization](https://github.com/pavanamthomas/lean4-analysis-formalization)
- [lean4-automation-debugging](https://github.com/pavanamthomas/lean4-automation-debugging)
- [lean4-mean-value-theorems](https://github.com/pavanamthomas/lean4-mean-value-theorems)

---

Python · R · SQL · NumPy · Pandas · SciPy · statsmodels · scikit-learn · PyTorch · Git/GitHub · Lean 4/mathlib
