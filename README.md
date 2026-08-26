# Pavanam Thomas

PhD, quantitative research. Public repositories below: identification and statistics on simulated designs, forecasting and optimisation notes, valuation identities, structured reviews of quantitative answers, and Lean 4 + mathlib studies.

Samples in the Python labs are simulated DGPs or closed forms unless a file says otherwise. Recovering a simulated parameter is not an empirical finding. Nothing here is a desk, a trading book, or a commercial deployment. Lean files that compile are theorems about the statements as written.

## Econometrics and statistics

**[econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)** — DiD, IV, RD, matching, and panel methods on documented DGPs. A coefficient that prints is not an identified treatment effect. [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md)

**[statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)** — Type I / Type II, coverage, p-value misuse, omitted-variable bias, under known DGPs. [statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md)

A longer list of those identification and inference labs: [ECONOMICS_EXPERT_PORTFOLIO.md](ECONOMICS_EXPERT_PORTFOLIO.md).

## Forecasting, optimisation, valuation

**[time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab)** — walk-forward skill on simulated series, not in-sample fit.

**[optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models)** — write the programme, solve it, substitute the point back into the original functions. Solver success is not KKT.

**[quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models)** — TVM, duration, parity, VaR/ES identities under stated assumptions. Not a trading book.

## Computational checks

These are method laboratories, not an engineering job title.

**[computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)** — problems with a reference solver and two further checks that are not copies of that solver.

**[machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab)** — invalid workflows kept next to the matching design (full-frame scaling, group leakage, inner `best_score_` treated as generalisation).

**[ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)** — fluent answers that fail on the target, the information set, or the interpretation. One author coded the YAML.

**[genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab)** — gold can sit at rank 1 while the extractive answer abstains. Retrieval metrics are not answer quality.

**[sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab)** — a join without `txn_ts <= cutoff` admits a planted future value without selecting the label.

**[pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab)** — hand derivatives, finite differences, and autograd; they disagree on purpose at a ReLU kink.

**[mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab)** — HTTP 200 with the wrong probability after a column swap.

Notes on those labs: [MACHINE_LEARNING_EXPERT_PORTFOLIO.md](MACHINE_LEARNING_EXPERT_PORTFOLIO.md).

## Question items

Self-directed 10-option items (one key, nine distractors, a derivation, references) in microstructure, macroprudential policy, behavioral finance, urban economics, and tokenomics. Not a venue, central-bank, or protocol job.

**[economics-finance-assessment-benchmark-lab](https://github.com/pavanamthomas/economics-finance-assessment-benchmark-lab)** — accepted items and rejected drafts. CI checks schema, not that the economics is true.

Companions: [microstructure](https://github.com/pavanamthomas/market-microstructure-algorithmic-trading-lab) · [macroprudential](https://github.com/pavanamthomas/macroprudential-systemic-risk-lab) · [behavioral finance](https://github.com/pavanamthomas/behavioral-finance-experimental-economics-lab) · [urban](https://github.com/pavanamthomas/urban-economics-spatial-equilibrium-lab) · [tokenomics](https://github.com/pavanamthomas/tokenomics-defi-mechanism-design-lab).

Map: [ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md](ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md).

## Lean 4

Compilation is not faithfulness.

- [lean4-optimization-economics](https://github.com/pavanamthomas/lean4-optimization-economics) — small programmes and budget sets
- [lean4-analysis-formalization](https://github.com/pavanamthomas/lean4-analysis-formalization) — limits, continuity, compactness
- [lean4-mean-value-theorems](https://github.com/pavanamthomas/lean4-mean-value-theorems) — Rolle, Lagrange, Cauchy reconstructed from EVT and Fermat
- [lean4-formalization-faithfulness](https://github.com/pavanamthomas/lean4-formalization-faithfulness) — compiled theorems that still miss the intended claim
- [lean4-formalization-review](https://github.com/pavanamthomas/lean4-formalization-review) — review cases
- [lean4-proof-engineering](https://github.com/pavanamthomas/lean4-proof-engineering) — structured proofs and tactic habits
- [lean4-automation-debugging](https://github.com/pavanamthomas/lean4-automation-debugging) — failed proofs, classified and repaired

Python, R, SQL, NumPy, Pandas, SciPy, statsmodels, scikit-learn, PyTorch, Lean 4/mathlib.
