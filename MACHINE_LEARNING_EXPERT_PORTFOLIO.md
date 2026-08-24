# Machine Learning Expert / Computational STEM

This page collects the parts of my public work most relevant to computational ML problem design, Python scientific computing, model validation, SQL feature engineering, GenAI/RAG evaluation, PyTorch, and reproducible serving.

My professional job history is quantitative research rather than a conventional ML-engineer title. I therefore prefer auditable implementation evidence over title-based claims: code, tests, CI, issues, roadmaps, deliberate failure cases, and documented corrections.

## Computational ML/STEM problem design

### [computational-ml-stem-problem-forge](https://github.com/pavanamthomas/computational-ml-stem-problem-forge)

**Question.** Can I design computationally non-trivial ML/statistics/STEM problems whose answers are independently verifiable rather than accepted because one reference implementation runs?

**Evidence.** Twelve complete problem laboratories, structured problem metadata, Python reference solutions, independent verifier paths, three ground-truth units, deterministic regeneration, tests, CI, and an audit path for candidate solutions.

The current corpus includes entity leakage, temporal leakage, nested-CV optimism, class imbalance, calibration, Monte Carlo coverage, KKT verification, bootstrap dependence, numerical instability, and plausible-but-wrong candidate answers.

**Inspect first.** [FLAGSHIP_CASE_STUDY.md](https://github.com/pavanamthomas/computational-ml-stem-problem-forge/blob/main/FLAGSHIP_CASE_STUDY.md)

**Questions I can defend.** Why is GT2 invalid if it simply recomputes GT1? How should stochastic ground truth be validated when exact equality is scientifically wrong? Why can a solver report success while a candidate solution is still invalid?

**Boundary.** The DGPs are stylised method checks, not empirical findings.

## Model selection and validation

### [machine-learning-model-selection-lab](https://github.com/pavanamthomas/machine-learning-model-selection-lab)

**Question.** What risk does a validation design actually estimate, and how can a technically valid pipeline still answer the wrong evaluation question?

**Evidence.** Full-frame preprocessing leakage, group leakage, temporal leakage, nested cross-validation, inner-score optimism, imbalance, calibration, covariate shift, permutation importance, memorisation, and synthetic DGPs with known truth.

The tests check properties such as group isolation, future-data exclusion, train-only preprocessing, inner/outer split separation, calibration behaviour, and reproducibility.

**Inspect first.** [CASE_STUDY_MODEL_SELECTION_FAILURE.md](https://github.com/pavanamthomas/machine-learning-model-selection-lab/blob/main/CASE_STUDY_MODEL_SELECTION_FAILURE.md)

**Questions I can defend.** Why is `GridSearchCV.best_score_` not a generalisation estimate? Why can shuffled cross-validation be wrong even when train/test rows are disjoint? Why can ROC-AUC improve while probability quality worsens?

**Boundary.** The repository does not claim that one learner is universally best; the DGPs are designed to expose validation pathologies.

## AI-response evaluation

### [ai-response-evaluation-benchmarks](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks)

**Question.** Can I identify the earliest substantive failure in a plausible technical answer rather than scoring fluency as correctness?

**Evidence.** Golden responses, rubric dimensions, severity labels, `correct_result_invalid_reasoning`, earliest-failure-point fields, validation scripts, tests, CI, and explicit correction notes. The corpus now also contains first-class `machine_learning`, `genai_rag`, `python_computation`, and `sql_reasoning` domains with adversarial cases on model-selection leakage, calibration versus ranking, RAG-stage attribution, instruction hierarchy, numerical stability, Monte Carlo tolerance, join cardinality, and point-in-time leakage.

**Inspect first.** [GOLDEN_RESPONSE_STANDARD.md](https://github.com/pavanamthomas/ai-response-evaluation-benchmarks/blob/main/GOLDEN_RESPONSE_STANDARD.md)

**Questions I can defend.** Why can the final numerical answer be correct while the response still fails technical review? How should the earliest substantive failure be separated from downstream symptoms?

**Boundary.** The cases are constructed technical review cases rather than production traffic. There is no second independent human rater or commercial LLM-judge benchmark, and the technical-domain extension is not presented as exhaustive.

## GenAI / RAG evaluation

### [genai-rag-evaluation-lab](https://github.com/pavanamthomas/genai-rag-evaluation-lab)

**Question.** Can retrieval, context-packing, and generation failures be separated instead of collapsed into one vague RAG score?

**Evidence.** Deterministic chunking and hashing embeddings, exact cosine retrieval in NumPy, hybrid search, context-budget checks, retrieval metrics, answer-level correctness and faithfulness flags, abstention cases, injection-like document text, tests, CI, and a flagship failure trace. Exact FAISS `IndexFlatIP` retrieval is now exercised as a second implementation, with L2-normalised cosine parity against NumPy, dimension checks, metadata-filter parity, and a deliberate cosine-versus-dot ranking reversal fixture.

**Inspect first.** [FLAGSHIP_RAG_FAILURE_ANALYSIS.md](https://github.com/pavanamthomas/genai-rag-evaluation-lab/blob/main/FLAGSHIP_RAG_FAILURE_ANALYSIS.md)

**Questions I can defend.** How can Recall-at-k improve while final answer quality falls? Can an answer be faithful to context but factually wrong because retrieval selected the wrong evidence? Why can cosine normalisation change ranking? What does exact FAISS/NumPy parity prove, and what does it not prove?

**Boundary.** The default path remains intentionally offline and reproducible. The repository does not claim production RAG deployment, paid-encoder performance, pgvector/PostgreSQL execution, approximate-index recall, or hosted vector-database scaling.

## SQL feature engineering

### [sql-ml-feature-engineering-lab](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab)

**Question.** Does every feature use only information that was available at the prediction cutoff?

**Evidence.** Correct and deliberately leaky SQL, planted post-cutoff sentinels, joins, windows, `ROW_NUMBER`/`RANK`/`DENSE_RANK`, `LAG`/`LEAD`, deduplication, NULL behaviour, query-plan checks, tests, and CI. A deterministic point-in-time subset is now verified across SQLite and DuckDB and independently recomputed in Pandas, including a post-cutoff `99999.0` sentinel, NULL/no-history cases, recency, counts, spend, and ranking-window semantics.

**Inspect first.** [FLAGSHIP_POINT_IN_TIME_FAILURE.md](https://github.com/pavanamthomas/sql-ml-feature-engineering-lab/blob/main/FLAGSHIP_POINT_IN_TIME_FAILURE.md)

**Questions I can defend.** How can SQL leak future information without selecting the label? Why can `LEAD` be invalid for point-in-time prediction? Why is event time not automatically equivalent to ingestion time? What does cross-engine parity establish versus full dialect equivalence?

**Boundary.** SQLite and DuckDB now provide executable parity evidence for the tested subset. Event time is still not ingest time; PostgreSQL-specific semantics and plans are not tested; time zones are not modelled; deterministic subset parity is not a claim of full database equivalence.

## PyTorch and neural-network verification

### [pytorch-deep-learning-lab](https://github.com/pavanamthomas/pytorch-deep-learning-lab)

**Question.** Do the hand-derived gradients, finite differences, and PyTorch autograd agree away from non-differentiable points?

**Evidence.** A NumPy MLP, analytic gradients, central-difference checks, PyTorch autograd comparison, activation pathologies, zero-initialisation symmetry, dead ReLU, vanishing/exploding gradients, BatchNorm train/eval behaviour, Adam versus AdamW, gradient clipping, a small CNN construction, tests, and CI.

**Inspect first.** [AUTOGRAD_VS_FINITE_DIFFERENCES.md](https://github.com/pavanamthomas/pytorch-deep-learning-lab/blob/main/AUTOGRAD_VS_FINITE_DIFFERENCES.md)

**Questions I can defend.** When autograd and finite differences disagree, which result should I trust? Why is gradient-check error often worst when epsilon is too large or too small? Why can `model.eval()` change predictions without changing weights?

**Boundary.** This is first-principles implementation evidence, not a claim of large-scale production deep-learning deployment.

## Reproducible serving and MLOps

### [mlops-reproducible-serving-lab](https://github.com/pavanamthomas/mlops-reproducible-serving-lab)

**Question.** Can an API be operationally healthy while returning a prediction that is mathematically inconsistent with the fitted training pipeline?

**Evidence.** An sklearn Pipeline, FastAPI, Pydantic schema checks, MLflow logging, versioned artifacts, training-serving skew detectors, drift diagnostics, rollback logic, Docker, parity tests, and CI. GitHub Actions now trains an offline artifact, builds the Docker image, launches the container, waits for model readiness, sends a schema-valid request to `/predict-proba`, and compares the served probability and schema/model versions against the offline fitted bundle. The development history retains the initial startup `ConnectionResetError`, its diagnosis, and the regression test that treats transient startup resets as retryable rather than as prediction failures.

**Inspect first.** [FLAGSHIP_TRAINING_SERVING_SKEW.md](https://github.com/pavanamthomas/mlops-reproducible-serving-lab/blob/main/FLAGSHIP_TRAINING_SERVING_SKEW.md)

**Questions I can defend.** Why does HTTP 200 prove endpoint availability but not model-serving correctness? Why should readiness failure, schema failure, and numerical prediction-parity failure be treated as different objects?

**Boundary.** This is a reproducible local/container serving laboratory, not a claim of production uptime, latency SLOs, load testing, canary traffic, cloud traffic management, Kubernetes, or incident history. One deterministic parity fixture is not exhaustive serving verification.

## What I expect a technical reviewer to challenge

The useful evidence is tests that lock known failure modes, issues that record unresolved bounds, roadmaps that name missing validation, and corrections that show where an initial procedure was insufficient. The recurring sequence is:

**target → assumptions → implementation → deliberate failure → independent check → correction → remaining bound**
