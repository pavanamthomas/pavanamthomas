# Economics Expert / PhD Quantitative Research

This page collects the parts of my public work that are most relevant to economics, econometrics, statistics, forecasting, optimisation, and quantitative review.

These laboratories are the identification and validation foundation of the machine-learning repositories, not a discarded earlier track. The same sequence — target, assumptions, method, check, bound — is what the ML, SQL, and RAG work inherits.

The common question across the repositories is not whether a model can produce a coefficient or score. It is whether the target quantity is defined clearly, the assumptions are defensible, the implementation matches those assumptions, and the reported conclusion survives an independent check.

## Econometrics and causal inference

### [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)

**Question.** What estimand is identified, under which assumptions, and what breaks when those assumptions fail?

**Evidence.** Difference-in-differences, event studies, instrumental variables, regression discontinuity, matching and weighting, panel methods, simulated data-generating processes with known truth, diagnostics, robustness checks, and tests.

**Inspect first.** [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md)

**A question I can defend.** When does an instrumental-variable estimate identify a local average treatment effect rather than an average treatment effect?

**Boundary.** A successful simulation or regression output is not treated as an empirical causal finding.

## Statistical reasoning and validation

### [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)

**Question.** Which statistical claims survive a known data-generating process, and which fail because the inferential object or uncertainty calculation is wrong?

**Evidence.** Monte Carlo coverage, probability identities, p-values and confidence intervals, heteroskedasticity, omitted-variable bias, bootstrap checks, classification metrics, imbalance, calibration, and a catalogue of statistical failure patterns.

**Inspect first.** [docs/statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md)

**A question I can defend.** Why does a robust standard error correct a variance estimate without repairing endogeneity?

**Boundary.** Simulated coverage or estimator recovery is a method check, not evidence about a real population.

## Forecasting and time-series validation

### [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab)

**Question.** Does a model genuinely forecast future observations better than a suitable benchmark without using future information?

**Evidence.** Stationarity checks, ARIMA and SARIMA, exponential smoothing, residual diagnostics, rolling-origin evaluation, naive benchmarks, structural-break analysis, interval coverage, and volatility-related checks.

**Inspect first.** [FORECAST_VALIDATION_PLAYBOOK.md](https://github.com/pavanamthomas/time-series-forecasting-lab/blob/main/FORECAST_VALIDATION_PLAYBOOK.md)

**A question I can defend.** Why can the best in-sample time-series model be the wrong forecasting model?

**Boundary.** In-sample fit is not reported as forecast skill.

## Mathematical modelling and optimisation

### [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models)

**Question.** Does the reported optimum actually satisfy the programme that was written down?

**Evidence.** Constrained and unconstrained optimisation, linear and integer programming, networks, dynamic programming, sensitivity analysis, feasibility checks, and independent verification of candidate optima.

**Inspect first.** [MODEL_AUDIT_CHECKLIST.md](https://github.com/pavanamthomas/optimization-decision-models/blob/main/MODEL_AUDIT_CHECKLIST.md)

**A question I can defend.** Why is a solver success flag not evidence of global optimality?

**Boundary.** Numerical convergence is checked against feasibility, objective values, and problem-specific conditions rather than treated as a proof.

## AI evaluation of quantitative reasoning

### [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

**Question.** When is a fluent quantitative answer still invalid because the target object, assumptions, method, or interpretation are wrong?

**Evidence.** Golden responses, ten-dimensional rubric scoring, severity labels, earliest-failure-point analysis, candidate-answer review, defect taxonomies, tests, and CI.

**Inspect first.** [FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md)

**A question I can defend.** Why can a numerically correct final answer still deserve a fail verdict?

**Boundary.** The corpus is single-author coded. Cohen's kappa checks known label tables; it is not presented as an inter-rater reliability study.

## Quantitative finance

### [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models)

**Question.** Which valuation and risk identities hold under closed-form or simulated conditions, and where do numerical or modelling assumptions break them?

**Evidence.** Reproducible quantitative finance calculations, checks against identities and simulated series, and explicit validation of modelling assumptions.

**Inspect first.** [MODEL_RISK_NOTES.md](https://github.com/pavanamthomas/quantitative-finance-models/blob/main/MODEL_RISK_NOTES.md)

**A question I can defend.** When is a numerically plausible valuation still inconsistent with the underlying model assumptions?

**Boundary.** This repository is not a trading book, client system, or record of live investment performance.

## Working style

Across these repositories, the sequence is deliberately consistent:

**target object → assumptions → method → implementation → failure analysis → independent validation → bounded interpretation**

That sequence is more important to me than presenting a long list of methods. It is also why the repositories retain deliberate failures, correction notes, tests, CI, issues, and roadmaps instead of showing only final successful outputs.
