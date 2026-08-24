# Machine Learning Expert / Computational STEM

Job history is quantitative research, not an ML-engineer title. What follows is implementation that can be opened, run, and challenged.

## [computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)

Twelve problems, each with a reference solver, a second ground-truth object, and a third code path. Copying the reference module is not verification.

Open [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/computational-ml-stem-problem-forge/blob/main/FLAGSHIP_CASE_STUDY.md). Entity intercepts leak under naive KFold; GT2 is overlap counts, not the accuracy gap. Nested CV keeps two positive optimism numbers whose magnitudes need not match because the fold constructions differ. Monte Carlo coverage is judged by SE, not `phat == 0.95`.

The DGPs are method checks. They are not empirical findings.

## [machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab)

Invalid workflows are kept next to the matching design: full-frame preprocessing, group leakage, a post-outcome sentinel, and `GridSearchCV.best_score_` treated as generalisation.

Open [CASE_STUDY_MODEL_SELECTION_FAILURE.md](https://github.com/pavanamthomas/machine-learning-model-selection-lab/blob/main/CASE_STUDY_MODEL_SELECTION_FAILURE.md). Tests lock group isolation, future-data exclusion, train-only scalers, inner/outer index separation, and the fact that perfect ROC-AUC can coexist with worse Brier and log loss.

## [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

A prompt, a candidate answer, earliest failure, corrected reasoning, golden response. Fluency is cheap. The corpus keeps economics and econometrics cases, and adds ML, RAG, Python, and SQL items including `correct_result_invalid_reasoning`.

Open [GOLDEN_RESPONSE_STANDARD.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/GOLDEN_RESPONSE_STANDARD.md). One author coded the YAML. There is no second-rater study.

## [genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab)

Retrieval metrics are not answer quality. Gold can sit in top-k while the extractive answer abstains on conflicting context.

Open [FLAGSHIP_RAG_FAILURE_ANALYSIS.md](https://github.com/pavanamthomas/genai-rag-evaluation-lab/blob/main/FLAGSHIP_RAG_FAILURE_ANALYSIS.md). CI compares FAISS `IndexFlatIP` with exact NumPy cosine after L2 normalisation, including a genuine cosine-versus-dot ranking reversal. FAISS is an in-memory index, not a vector database. The flagship trace itself uses NumPy.

No hosted RAG, no pgvector path, no approximate-index recall claim.

## [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab)

A feature at cutoff `t` may use only information available by `t`. Joining transactions on `customer_id` without `txn_ts <= cutoff` admits a planted `99999.0` without ever selecting the label.

Open [FLAGSHIP_POINT_IN_TIME_FAILURE.md](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab/blob/main/FLAGSHIP_POINT_IN_TIME_FAILURE.md). A compact fixture is checked in SQLite, DuckDB, and Pandas. That is not PostgreSQL equivalence. Event time is not ingest time.

## [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab)

Hand derivatives, central differences, and autograd are compared on synthetic maps. Finite-difference error is U-shaped in ε. At a ReLU kink the two conventions disagree on purpose.

Open [AUTOGRAD_VS_FINITE_DIFFERENCES.md](https://github.com/pavanamthomas/pytorch-deep-learning-lab/blob/main/AUTOGRAD_VS_FINITE_DIFFERENCES.md). `model.eval()` changes BatchNorm predictions without changing weights. This is not a production training stack.

## [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab)

HTTP 200 is not training-serving equality. A schema-valid request with swapped columns still returns 200 and the wrong probability.

Open [FLAGSHIP_TRAINING_SERVING_SKEW.md](https://github.com/pavanamthomas/mlops-reproducible-serving-lab/blob/main/FLAGSHIP_TRAINING_SERVING_SKEW.md). CI trains an artifact, builds the Docker image, waits for model readiness, and compares `/predict-proba` with the offline Pipeline. The first container attempt failed with `ConnectionResetError` during readiness polling; that is retained as a retry, not as a parity failure.

No Kubernetes, no SLO, no production traffic.
