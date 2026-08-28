# Identification, inference, and model notes

Public Python labs on identification, statistical mistakes, forecasting, optimisation, and valuation identities. All samples are simulated DGPs or closed forms unless a file says otherwise. Recovering a simulated parameter is not an empirical finding.

The 10-option items in five applied domains are a separate set of notes: [ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md](ECONOMICS_FINANCE_ASSESSMENT_PORTFOLIO.md). DiD and TVM are not substitutes for those items.

## [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)

What estimand is identified, under which assumptions, and what breaks when those fail.

[CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md). DiD, IV, RD, matching, and panel methods sit on documented DGPs. A coefficient that prints is not an empirical causal finding. An IV that satisfies an exclusion restriction in a LATE design is not an ATE.

## [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)

Which inferential claims survive a known DGP.

[docs/statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md). Coverage is a Monte Carlo functional. A robust standard error repairs a variance estimate; it does not repair endogeneity. Majority accuracy on a rare-event DGP remains a bad summary.

## [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab)

Out-of-sample forecast skill, not in-sample fit.

[FORECAST_VALIDATION_PLAYBOOK.md](https://github.com/pavanamthomas/time-series-forecasting-lab/blob/main/FORECAST_VALIDATION_PLAYBOOK.md). Rolling origin, naive benchmarks, and a designed case where an undifferenced ARIMA on a trend loses out of sample.

## [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models)

Does the reported point satisfy the programme that was written down?

[MODEL_AUDIT_CHECKLIST.md](https://github.com/pavanamthomas/optimization-decision-models/blob/main/MODEL_AUDIT_CHECKLIST.md). Solver success is not global optimality. Feasibility, KKT residuals, and a poor local start on a double well are kept visible.

## [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

Fluent quantitative answers that fail on the target object, the information set, or the interpretation.

[FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md) (staggered DiD). A correct final number can still be a fail. One author coded the YAML; Cohen's kappa on known tables is arithmetic, not a second-rater study.

## [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models)

Identities under stated assumptions, not a trading book.

[MODEL_RISK_NOTES.md](https://github.com/pavanamthomas/quantitative-finance-models/blob/main/MODEL_RISK_NOTES.md). Duration-convexity error grows with the yield shock. Recovering a simulated parameter is not live performance.

## [financial-annotation-reconciliation-labs](https://github.com/pavanamthomas/financial-annotation-reconciliation-labs)

A number that ties is not a finished check.

Three packages in one tree: a spreadsheet `SUM` that includes a product row, an invoice span labelled `total` that is the pre-tax subtotal, and a cash rec that ties by adding back a check already on the bank statement. Grids and ledgers are written in the repo. There are no client files.
