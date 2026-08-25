# Economics & Finance Assessment / AI Benchmarking

This track is for work where the object is not merely an economic answer, but a defensible assessment item: one precise question, one uniquely correct answer, plausible distractors, a calibrated difficulty label, a compact solution, and references that support the result.

My professional base is Economics: doctoral research, university teaching and assessment, econometrics, statistics, mathematical modelling, research writing, and quantitative review. The public repositories below are the evidence I would use for question authoring and verification. They do not claim financial-industry employment, trading-book experience, or production DeFi work.

## What I would expect a reviewer to test

For authoring, I would expect scrutiny on five things:

1. Is the stem self-contained and solvable from the information given?
2. Is exactly one option correct under the stated assumptions?
3. Are the nine distractors plausible because they encode real misconceptions rather than random noise?
4. Is the difficulty label driven by the reasoning burden rather than by cosmetic algebra?
5. Can the solution and references independently support the keyed answer?

For verification, I use a separate sequence:

**solvability -> uniqueness -> completeness -> precision -> economic validity -> mathematical validity -> distractor quality -> difficulty calibration -> reference support**

A polished question still fails if a second option is defensible, a hidden assumption changes the answer, or a cited source does not actually support the keyed result.

## [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

This is the closest existing evidence for benchmark review.

Open [FLAGSHIP_REVIEW_CASE.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/FLAGSHIP_REVIEW_CASE.md). The repository separates the target object, assumptions, reasoning path, final result, error severity, correction, and golden response. A correct final number can still fail if the reasoning or interpretation is invalid.

For assessment verification, the same habit becomes: identify the earliest substantive defect in the stem, key, solution, distractors, or reference support before editing downstream wording.

## [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab)

This is the main source for graduate-level economics items where the distractor hinges on identification rather than recall.

Open [CASE_STUDY.md](https://github.com/pavanamthomas/econometrics-causal-inference-lab/blob/main/CASE_STUDY.md). DiD, IV, RD, matching and panel designs sit on documented DGPs. Useful assessment distinctions include association versus identification, ATE versus LATE, robust inference versus endogeneity, and specification versus estimand.

## [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation)

This is the main source for quantitative distractors that look reasonable but fail on probability, inference, calibration, power, coverage, or interpretation.

Open [docs/statistical_error_catalogue.md](https://github.com/pavanamthomas/statistical-reasoning-validation/blob/main/docs/statistical_error_catalogue.md). The repository keeps common inferential errors next to known-DGP checks so that a wrong option can be tied to a specific misconception rather than made artificially absurd.

## [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models)

This is the finance-facing quantitative evidence.

Open [MODEL_RISK_NOTES.md](https://github.com/pavanamthomas/quantitative-finance-models/blob/main/MODEL_RISK_NOTES.md). The repository focuses on stated assumptions, valuation/risk identities, approximation error, and independent checks. It is not presented as live trading performance.

## [time-series-forecasting-lab](https://github.com/pavanamthomas/time-series-forecasting-lab)

This supports questions where the wrong answer comes from confusing in-sample fit with genuine forecast performance, using future information, or evaluating against the wrong benchmark.

Open [FORECAST_VALIDATION_PLAYBOOK.md](https://github.com/pavanamthomas/time-series-forecasting-lab/blob/main/FORECAST_VALIDATION_PLAYBOOK.md).

## [optimization-decision-models](https://github.com/pavanamthomas/optimization-decision-models)

This supports questions in optimization, equilibrium constraints, feasibility and model verification.

Open [MODEL_AUDIT_CHECKLIST.md](https://github.com/pavanamthomas/optimization-decision-models/blob/main/MODEL_AUDIT_CHECKLIST.md). Solver success is not itself a proof of feasibility or optimality.

---

## Domain map for the current assessment role

### Behavioral Finance & Experimental Economics

Strongest current overlap: probability, decision under uncertainty, causal reasoning, experimental design, treatment effects, inference and interpretation. Relevant item types include prospect theory, loss aversion, reference dependence, overconfidence, anchoring, disposition effects, incentives, randomization and internal/external validity.

### Urban Economics

Strong economics-theory overlap: spatial equilibrium, commuting costs, land/housing markets, local public goods, externalities, sorting and policy evaluation. Appropriate questions should test mechanisms and comparative statics, not only named-model recall.

### Macroprudential Policy

Current overlap is strongest through macroeconomics, banking, risk, causal inference and policy evaluation. Specialist items should make the policy instrument, systemic-risk mechanism and maintained assumptions explicit. I do not treat conceptual familiarity as evidence of supervisory or regulatory employment.

### Algorithmic Trading & Market Microstructure

Current public evidence is quantitative-finance and time-series modelling rather than professional trading infrastructure. Assessment work here should therefore be grounded in explicit models and references: bid-ask spreads, adverse selection, inventory risk, order types, price impact, liquidity, execution costs and market design.

### Tokenomics & Decentralized Finance

This is a specialist extension rather than an employment claim. Questions should be model- and mechanism-specific: AMMs, constant-product pricing, slippage, impermanent loss, collateralization, liquidation, governance incentives, oracle risk, stablecoins and MEV. Any public item should be supported by an academic or primary technical reference.

---

## How I would build a ten-option item

A ten-option multiple-choice item should not be one correct answer plus nine arbitrary false statements.

I would first write the keyed reasoning path, then build distractors from specific error classes such as:

- sign reversal;
- necessary versus sufficient condition;
- level versus marginal effect;
- partial-equilibrium result used where equilibrium feedback matters;
- wrong information set;
- correlation treated as identification;
- correct formula under the wrong denominator or timing convention;
- approximation used outside its valid range;
- correct theorem under a violated assumption.

The final uniqueness audit asks a stricter question than “is the key correct?”: **can a technically strong reader defend any other option under a reasonable interpretation of the stem?** If yes, the item is not ready.

## Difficulty calibration

**Medium**: one core undergraduate concept with direct application and limited inferential branching.

**Hard**: advanced undergraduate reasoning that combines concepts, comparative statics, nontrivial quantitative work, or a realistic misconception.

**Expert**: postgraduate reasoning where assumptions, equilibrium effects, identification, advanced finance mathematics, or a boundary condition determines the answer.

Length of algebra alone is not difficulty.

## Reference standard

For each question I would prefer a small number of sources that actually support the keyed claim: peer-reviewed articles, canonical academic books, university repositories, or primary institutional/technical material where appropriate.

References are part of verification, not decoration. A citation to the right topic is insufficient if it does not support the exact mechanism or result used in the solution.

## Boundary

This page organizes existing public evidence for economics/finance assessment authoring and verification. It does not claim CFA/CPA certification, financial-industry employment, algorithmic-trading production experience, DeFi protocol employment, or expertise unsupported by the linked work and references.
