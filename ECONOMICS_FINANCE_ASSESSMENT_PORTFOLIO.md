# Economics & Finance Assessment

This track is the public work sample for **question authoring** and **question verification** in the five domains named in that posting: market microstructure, macroprudential policy, behavioral finance / experimental economics, urban economics, and tokenomics / DeFi.

The object is a 10-option item: one key, nine expert-plausible distractors, a Medium / Hard / Expert label, a written derivation, and 1–5 references that support the keyed claim. Self-directed study. Not a desk, a CFA, or a protocol job.

## What this track is not

Do not treat methods labs as the five domains.

| Methods repo | What it actually is | What it is not |
| --- | --- | --- |
| [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab) | DiD, IV, RD, matching on documented DGPs | Urban economics; a 10-option amenity-shock item |
| [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) | TVM, parity, duration, VaR identities | Market microstructure; an executable book |
| [statistical-reasoning-validation](https://github.com/pavanamthomas/statistical-reasoning-validation) | Coverage, Type I/II, p-value misuse | Behavioral finance; a CPT reference table |
| [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks) | Scoring fluent *answers* | Authoring the stems; the rejected-item file |
| ML laboratories on this profile | Model selection, RAG, SQL, PyTorch | This assessment role |

Those repos are listed on [ECONOMICS_EXPERT_PORTFOLIO.md](ECONOMICS_EXPERT_PORTFOLIO.md). They support quantitative methods. They are not substitutes for the table below.

## What to open first

**[economics-finance-assessment-benchmark-lab](https://github.com/pavanamthomas/economics-finance-assessment-benchmark-lab)**

40 accepted items (eight in each domain below) and 11 rejected drafts. CI checks schema, option count, uniqueness write-up, citation count, and numerical blocks. It does **not** certify that the economics is true. That residual is the derivation, `MANUAL_REVIEW_CHECKLIST.md`, and whoever reads them.

Open [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/economics-finance-assessment-benchmark-lab/blob/main/FLAGSHIP_CASE_STUDY.md). Fee-free CPAMM `(x, y) = (100, 100)`, sale `Δx = 10`. Three numbers: pre-trade spot 1, average execution `10/11`, post-trade spot `100/121`. A stem that asks for “the price” has three defensible keys. The repaired item names the object.

Rejected drafts live in `rejected_items/`. Each names a defect class (two keys, hidden assumption, wrong key, no correct option, unsupported reference, difficulty miscalibration, joke distractors, timing ambiguity, missing equilibrium, unnamed price, ambiguous information set).

## Domain map

| Posting domain | In the corpus | Executable lab |
| --- | --- | --- |
| Algorithmic trading & market microstructure | `items/algorithmic_trading/` (prefix `MM`) | [market-microstructure-algorithmic-trading-lab](https://github.com/pavanamthomas/market-microstructure-algorithmic-trading-lab) |
| Macroprudential policy | `items/macroprudential/` (prefix `MP`) | [macroprudential-systemic-risk-lab](https://github.com/pavanamthomas/macroprudential-systemic-risk-lab) |
| Behavioral finance & experimental economics | `items/behavioral_finance/` (prefix `BF`) | [behavioral-finance-experimental-economics-lab](https://github.com/pavanamthomas/behavioral-finance-experimental-economics-lab) |
| Urban economics | `items/urban_economics/` (prefix `UE`) | [urban-economics-spatial-equilibrium-lab](https://github.com/pavanamthomas/urban-economics-spatial-equilibrium-lab) |
| Tokenomics & decentralized finance | `items/tokenomics_defi/` (prefix `TD`) | [tokenomics-defi-mechanism-design-lab](https://github.com/pavanamthomas/tokenomics-defi-mechanism-design-lab) |

Difficulty mix in the accepted corpus: 10 Medium, 15 Hard, 15 Expert. The rubric is inferential branching, not algebra length (`docs/difficulty_calibration.md`). A glossary card labelled Expert is a reject (`RJ-06`).

### Algorithmic trading & market microstructure

Flagship in the corpus: `MM-E-01` (mid-mark versus executable books). The lab walks the same 4,000-event tape at look-ahead mid, causal mid, quoted touch, walked book, fees, impact, and delayed fill. Causal mid **+0.00745**/unit versus walked book **−0.00588**. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/market-microstructure-algorithmic-trading-lab/blob/main/FLAGSHIP_CASE_STUDY.md)

Related, not this object: [quantitative-finance-models](https://github.com/pavanamthomas/quantitative-finance-models) is valuation and risk summaries, not a limit-order book.

### Macroprudential policy

Flagship in the corpus: `MP-E-01` (Nash fire sale versus coordinated freeze). Three identical banks, shock `p = 0.92`. Freeze κ **9.09%**. Restore a 10% target: the whole float is sold, `p = 0.276`, terminal κ **6.86%**. Releasing the CCyB is the freeze in that calibration. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/macroprudential-systemic-risk-lab/blob/main/FLAGSHIP_CASE_STUDY.md)

### Behavioral finance & experimental economics

Flagship in the corpus: `BF-E-01` — a CPT prediction is not unique until the reference point is stated. The lab prints the TK92 table: purchase R=100 takes the 50-50 (gap **+0.44**); spot R=80 locks (gap **−4.74**); linear `v(x)=x` is indifferent at every R. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/behavioral-finance-experimental-economics-lab/blob/main/FLAGSHIP_CASE_STUDY.md)

Overlap with [econometrics-causal-inference-lab](https://github.com/pavanamthomas/econometrics-causal-inference-lab) is experimental design, not a substitute for the YAML or the value-function table.

### Urban economics

Flagship in the corpus: `UE-H-01` — closed-city versus open-city amenity shock. The lab: closed dR ≈ **+0.094** with du > 0; open dR ≈ **+0.361** with du = 0 and N 1 → 1.555. “Rents rise and residents are better off in both models” is false. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/urban-economics-spatial-equilibrium-lab/blob/main/FLAGSHIP_CASE_STUDY.md)

### Tokenomics & decentralized finance

Flagship in the corpus: `TD-E-01` (the three prices). The lab adds the 30 bp fee case that breaks the geometric-mean identity, IL versus hold, arb restoration, health factor, stale oracles, and ordering rent on a constructed pool — not a bot. [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/tokenomics-defi-mechanism-design-lab/blob/main/FLAGSHIP_CASE_STUDY.md)

## Authoring versus verification

`ai-response-evaluation-benchmarks` scores *answers*. This laboratory writes the *questions*, including the ones that were rejected. That repository is not modified by this track.

Verification here is a written object: uniqueness audit, distractor rationales, independent numerical or boundary check, and an edit trail when a draft fails. Passing CI means the YAML is complete. It does not mean the item should be accepted.

## Boundary

No implied employment at a venue, a central bank, or a protocol. No live returns, no AUM, no client tape, no mainnet deployment. Adjacent identification and methods labs (econometrics, statistics, forecasting, optimisation, quantitative-finance identities) remain listed on [ECONOMICS_EXPERT_PORTFOLIO.md](ECONOMICS_EXPERT_PORTFOLIO.md). They are not this five-domain assessment corpus.
