# Dr. Pavanam Thomas

PhD quantitative researcher. Economics, statistics, mathematical modelling, and — in public code — machine learning, SQL, RAG evaluation, and PyTorch.

The economics work is not a previous identity. Identification, information sets, and independent checks are the same habit whether the object is an IV, a nested-CV score, a SQL feature, or a RAG trace. Job history is quantitative research, not an ML-engineer title.

**Economics & Finance assessment authoring / verification** (the five posting domains: market microstructure, macroprudential policy, behavioral finance, urban economics, tokenomics/DeFi) is the first track below. DiD, TVM, and the ML laboratories are quantitative methods. They are **not** those five domains.

[Economics & Finance Assessment](ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md) · 10-option authoring and verification in the five posting domains. This is the work sample for that role.

[Economics Expert / PhD Quantitative Research](ECONOMICS_EXPERT_PORTFOLIO.md) · Econometrics, causal inference, forecasting, optimisation, AI evaluation of quantitative answers. Methods track. Not a substitute for the five domains.

[Machine Learning Expert / Computational STEM](MACHINE_LEARNING_EXPERT_PORTFOLIO.md) · Python, model validation, ground-truth engineering, SQL, GenAI/RAG, PyTorch, reproducible serving.

Samples in the Python repos are documented simulated DGPs or closed forms unless a file says otherwise. Recovering a simulated parameter is not an empirical finding. Nothing here is a commercial deployment.

---

## Economics & finance assessment (the five posting domains)

This is the sample for **question authoring** and **question verification**. Eight 10-option items in each domain, plus an executable companion lab for each domain.

**[economics-finance-assessment-benchmark-lab](https://github.com/pavanamthomas/economics-finance-assessment-benchmark-lab)** — 40 accepted items and 11 rejected drafts. The validator checks completeness, not economic truth. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/economics-finance-assessment-benchmark-lab/blob/main/FLAGSHIP_CASE_STUDY.md): fee-free pool `(100, 100)`, sale of 10 X; spots 1 and `100/121` versus fill `10/11`.

| Posting domain | Companion lab |
| --- | --- |
| Algorithmic trading & market microstructure | [market-microstructure-algorithmic-trading-lab](https://github.com/pavanamthomas/market-microstructure-algorithmic-trading-lab) |
| Macroprudential policy | [macroprudential-systemic-risk-lab](https://github.com/pavanamthomas/macroprudential-systemic-risk-lab) |
| Behavioral finance & experimental economics | [behavioral-finance-experimental-economics-lab](https://github.com/pavanamthomas/behavioral-finance-experimental-economics-lab) |
| Urban economics | [urban-economics-spatial-equilibrium-lab](https://github.com/pavanamthomas/urban-economics-spatial-equilibrium-lab) |
| Tokenomics & decentralized finance | [tokenomics-defi-mechanism-design-lab](https://github.com/pavanamthomas/tokenomics-defi-mechanism-design-lab) |

Full map: [ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md](ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md).

**Not a substitute for the five domains.** [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab) is DiD / IV / RD on documented DGPs — it is not urban economics. [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) is TVM, parity, and VaR identities — it is not a limit-order book. [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks) scores *answers* — it does not author the 10-option stems. Those repos stay on the methods page.

---

## Work a reviewer can open (identification and ML)

**[econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)** — DiD, IV, RD, matching, and panel methods on documented DGPs. A coefficient that prints is not an identified treatment effect. [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md)

**[computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)** — twelve problems, each with a reference solver and two further checks that are not copies of that solver. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/computational-ml-stem-problem-forge/blob/main/FLAGSHIP_CASE_STUDY.md)

**[statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)** — Type I / Type II, coverage, and p-value misuse under known DGPs. [statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md)

**[machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab)** — invalid workflows kept next to the matching design: full-frame scaling, group leakage, inner `best_score_` treated as generalisation. [CASE_STUDY_MODEL_SELECTION_FAILURE.md](https://github.com/pavanamthomas/machine-learning-model-selection-lab/blob/main/CASE_STUDY_MODEL_SELECTION_FAILURE.md)

**[ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)** — fluent answers that fail on the target, the information set, or the interpretation. One author coded the YAML. [FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md)

**[genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab)** — gold can sit at rank 1 while the extractive answer abstains. Retrieval metrics are not answer quality. [FLAGSHIP_RAG_FAILURE_ANALYSIS.md](https://github.com/pavanamthomas/genai-rag-evaluation-lab/blob/main/FLAGSHIP_RAG_FAILURE_ANALYSIS.md)

---

## Also in the tree

- [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab) — a join without `txn_ts <= cutoff` admits a planted `99999.0` without selecting the label.
- [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab) — hand derivatives, finite differences, and autograd; they disagree on purpose at a ReLU kink.
- [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab) — HTTP 200 with the wrong probability after a column swap.
- [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab) — walk-forward skill, not in-sample fit.
- [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models) — solver success is not KKT.
- [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) — identities under stated assumptions, not a trading book.

Lean 4 work (compilation is not faithfulness): [lean4-optimization-economics](https://github.com/pavanamthomas/lean4-optimization-economics), [lean4-formalization-review](https://github.com/pavanamthomas/lean4-formalization-review), [lean4-formalization-faithfulness](https://github.com/pavanamthomas/lean4-formalization-faithfulness), [lean4-proof-engineering](https://github.com/pavanamthomas/lean4-proof-engineering), [lean4-analysis-formalization](https://github.com/pavanamthomas/lean4-analysis-formalization), [lean4-automation-debugging](https://github.com/pavanamthomas/lean4-automation-debugging), [lean4-mean-value-theorems](https://github.com/pavanamthomas/lean4-mean-value-theorems).

Python, R, SQL, NumPy, Pandas, SciPy, statsmodels, scikit-learn, PyTorch, Lean 4/mathlib.
