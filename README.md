<div align="center">

```
AI Engineer  ·  Multi-Agent Systems  ·  LLM Evaluation  ·  MLOps
```

# Kalyan Venkatesh

**AI Engineer with 4+ years across research and production ML**, building compound AI systems with
multi-agent orchestration, evaluation frameworks and adversarial reliability testing, shipped from
prototype through production deployment.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-kalyanvenk.com-8957e5?style=flat-square&logo=github)](https://kalyan-venk.github.io)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Inference--Lens-22d3ee?style=flat-square&logo=github)](https://kalyan-venk.github.io/play.html)

</div>

---

## Experience

### [Graduate Research Engineer · DePaul University](https://kalyan-venk.github.io/agentic-llmops.html) &nbsp; `LangGraph` `Ollama` `MLflow`
*Sep 2025 – Jun 2026*

- Designed a compound AI system (Planner → Critic → Fixer) in LangGraph and Ollama combining
  planning, evaluation and automated error recovery across 10 phases and 5 model families,
  yielding a statistically significant **+4.85 pp pass@1** gain (95% CI [+3.36, +6.34], p = 0.010).
- Established the **Inverse Capability Hypothesis** across 3 independent trials: weak models gained
  (Code Llama +30.3 pp) while strong models regressed (Qwen −4.0 pp), both CIs excluding zero,
  pinning ~65% pass@1 as the reliability threshold above which monitoring turns net-negative. The
  law held across HumanEval-100, HumanEval+ and MBPP.
- Built a **Selective Reversion Gate** that reverts 73.4% of fixer outputs to keep only
  high-confidence corrections, plus a reproducible experiment harness (docker-compose,
  deterministic seeding, multi-trial runs, automated metric aggregation) with MLflow tracking.

### Data Scientist · [sensen.ai](https://sensen.ai) &nbsp; `2022 – 2024`

- Developed 8 SenFORCE ticket generation APIs, court-admissible image storage pipelines and
  time-based compression across AWS and Azure.
- Engineered ANPR model evaluation pipelines across 26 global deployments, adopted as the standard
  model validation workflow at sensen.ai.
- Optimized high-volume data workflows with PL/SQL functions and lightweight image retrieval,
  cutting pipeline latency from ~800ms to ~480ms.
- Replaced manual invoicing with end-to-end ETL pipelines processing ~30k weekly ANPR sightings,
  reducing consolidation time from 10+ hrs to 2 hrs/week.
- Led R&D on industrial pollution enforcement with drone-based effluent sampling, designed to cover
  25–30 discharge points daily against weekly manual checks, a 20–25x increase in coverage.

### Data Engineer · AECOM & Siri &nbsp; `2021 – 2022`

- Automated data preprocessing, cleaning and monthly cost consolidation pipelines in Python and
  Pandas, cutting dashboard preparation time by ~60% (3 hrs → <1 hr).
- Wrote analytical SQL across 2 infrastructure project cost databases, cutting report runtime from
  ~20s to ~8s for client-facing deliverables.

---

## Projects

### [Inference-Lens: Adversarial Reliability of NLP Evaluators](https://kalyan-venk.github.io/inference-lens.html) &nbsp; `DeBERTa-v3` `XGBoost` `LLM-Bar` `MLflow`
*Mar 2026 – Jun 2026*

**[Try the live scorer](https://kalyan-venk.github.io/play.html)** and watch an automated judge pick
the worse response in real time.

- Built an LLM-as-judge evaluation system stress-testing whether automated evaluators can be fooled,
  grounding every experiment in 170K+ human preference annotations (Anthropic HH-RLHF) then
  attacking with 419 adversarial LLM-Bar pairs across 4 perturbation types.
- Trained L2 logistic regression, XGBoost (5-fold CV) and a fine-tuned DeBERTa-v3-small, showing
  evaluator reliability degrades by architecture and attack type, shipped as a zero-backend browser
  live demo.
- Clustered 182K response embeddings (K-Means, DBSCAN, Ward) into 4 quality archetypes predicting
  adversarial vulnerability, extending the pipeline to toxic-comment identification and multi-label
  classification.

### [PredictOps: End-to-End ML Serving Pipeline with Automated Eval Gating](https://github.com/kalyan-venk/PredictOps) &nbsp; `FastAPI` `Docker` `GitHub Actions` `MLflow` `Evidently`
*Jul 2026 – Present*

- Benchmarked LogisticRegression against XGBoost on 7,043-row Telco churn data via stratified
  5-fold CV, selecting the tighter cross-validated model (0.846 vs 0.842 ROC-AUC) and confirming it
  held on a 20% held-out split (0.842 ROC-AUC, 80.6% accuracy).
- Served the selected model behind a FastAPI layer (4 endpoints, 19 Pydantic-validated and
  enum-constrained fields) in a multi-stage Docker image, cutting deployed image size from ~1.2GB
  to ~340MB, a 72% reduction.
- Built a CI eval gate in GitHub Actions as a standing quality contract, hard-blocking any push
  below ROC-AUC ≥ 0.80 from reaching the MLflow registry, verified by shipping a deliberately
  degraded model, watching CI fail, then fixing it to pass.
- Automated data-drift detection with Evidently on a reference-vs-current split, logging a
  per-feature PSI score and tripping a threshold alert at PSI > 0.15 on injected shift.

---

## Skills

**Languages** `Python` `SQL` `Java`

**AI/ML** `LangGraph` `LangChain` `Agentic AI` `Multi-Agent Systems` `Tool Use` `Prompt Engineering` `LLM Evaluation` `HuggingFace Transformers` `Fine-tuning` `Embeddings` `Scikit-learn` `XGBoost`

**MLOps & Serving** `MLflow` `Weights & Biases` `FastAPI` `Model Serving` `Ollama` `Docker` `GitHub Actions (CI/CD)` `Pydantic` `Evidently` `Data Drift Monitoring`

**Reliability & Evaluation** `Imbalanced Classification` `Adversarial Evaluation` `Experimental Design`

**Cloud & Data** `AWS` `PostgreSQL` `NumPy` `Pandas` `Git`

---

## Education

| | |
|---|---|
| **MS Computer Science** | DePaul University · Chicago, IL · Sep 2024 – Jun 2026 |
| **BTech Engineering** | National Institute of Technology · Nagpur, India · Jul 2017 – May 2021 |

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)**
- **AWS Certified Machine Learning Engineer – Associate** · In progress

---

<div align="center">

*Open to AI Engineer · ML Engineer · Data Scientist · Software Engineer roles*

</div>
