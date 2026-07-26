<div align="center">

```
AI Engineer  ·  Multi-Agent Systems  ·  LLM Evaluation  ·  MLOps
```

# Kalyan Venkatesh

**AI Engineer, 4+ years across research and production ML.** I build compound AI systems with
multi-agent orchestration and evaluation frameworks. A lot of the work is adversarial reliability
testing, which mostly means trying to break my own evaluators. I've taken these from prototype
through production deployment.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-kalyanvenk.com-8957e5?style=flat-square&logo=github)](https://kalyan-venk.github.io)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Inference--Lens-22d3ee?style=flat-square&logo=github)](https://kalyan-venk.github.io/play.html)

</div>

---

## Experience

### [Graduate Research Engineer · DePaul University](https://kalyan-venk.github.io/agentic-llmops.html) &nbsp; `LangGraph` `Ollama` `MLflow`
*Sep 2025 – Jun 2026*

- Designed a compound AI system in LangGraph and Ollama: a Planner writes, a Critic evaluates, a
  Fixer recovers from the errors. Ran it across 10 phases and 5 model families for a
  **+4.85 pp pass@1** gain, statistically significant (95% CI [+3.36, +6.34], p = 0.010).
- Got the same result in 3 independent trials and named it the **Inverse Capability Hypothesis**.
  Weak models gained (Code Llama +30.3 pp), strong models regressed (Qwen −4.0 pp), and neither CI
  crossed zero. The threshold sits at ~65% pass@1. Above that, monitoring turns net-negative. It
  held on HumanEval-100, HumanEval+ and MBPP.
- Built a **Selective Reversion Gate** that reverts 73.4% of fixer outputs and keeps only the
  high-confidence corrections. The harness around it is reproducible: docker-compose, deterministic
  seeding, multi-trial runs, automated metric aggregation, all tracked in MLflow.

### Data Scientist · [sensen.ai](https://sensen.ai) &nbsp; `2022 – 2024`

- Shipped 8 SenFORCE ticket generation APIs, court-admissible image storage pipelines and
  time-based compression, running across AWS and Azure.
- Wrote the ANPR model evaluation pipelines used across 26 global deployments. sensen.ai adopted
  them as the standard model validation workflow.
- Tuned high-volume data workflows with PL/SQL functions and lighter image retrieval. Pipeline
  latency went from ~800ms to ~480ms.
- Replaced manual invoicing with end-to-end ETL pipelines over ~30k weekly ANPR sightings.
  Consolidation dropped from 10+ hrs a week to 2.
- Led R&D on industrial pollution enforcement with drone-based effluent sampling, designed to cover
  25–30 discharge points daily against weekly manual checks. That is 20–25x the coverage.

### Data Engineer · AECOM & Siri &nbsp; `2021 – 2022`

- Automated data preprocessing, cleaning and monthly cost consolidation pipelines in Python and
  Pandas. Dashboard preparation dropped ~60%, from 3 hrs to under 1.
- Wrote analytical SQL across 2 infrastructure project cost databases and got report runtime on
  client-facing deliverables from ~20s down to ~8s.

---

## Projects

### [Inference-Lens: Adversarial Reliability of NLP Evaluators](https://kalyan-venk.github.io/inference-lens.html) &nbsp; `DeBERTa-v3` `XGBoost` `LLM-Bar` `MLflow`
*Mar 2026 – Jun 2026*

**[Try the live scorer](https://kalyan-venk.github.io/play.html)**. Watch an automated judge pick
the worse response in real time.

- Built an LLM-as-judge evaluation system to find out whether automated evaluators can be fooled.
  Every experiment is grounded in 170K+ human preference annotations (Anthropic HH-RLHF), then
  attacked with 419 adversarial LLM-Bar pairs across 4 perturbation types.
- Trained L2 logistic regression, XGBoost (5-fold CV) and a fine-tuned DeBERTa-v3-small. Evaluator
  reliability degrades differently by architecture and by attack type. The whole thing ships as a
  live browser demo with no backend.
- Clustered 182K response embeddings (K-Means, DBSCAN, Ward) into 4 quality archetypes that predict
  adversarial vulnerability. The same pipeline extends to toxic-comment identification and
  multi-label classification.

### [PredictOps: End-to-End ML Serving Pipeline with Automated Eval Gating](https://github.com/kalyan-venk/PredictOps) &nbsp; `FastAPI` `Docker` `GitHub Actions` `MLflow` `Evidently`
*Jul 2026 – Present*

- Benchmarked LogisticRegression against XGBoost on 7,043-row Telco churn data with stratified
  5-fold CV. The tighter cross-validated model won (0.846 vs 0.842 ROC-AUC) and held on a 20%
  held-out split (0.842 ROC-AUC, 80.6% accuracy).
- Served that model behind a FastAPI layer: 4 endpoints, 19 fields validated by Pydantic and
  constrained by enum. A multi-stage Docker image took the deployed size from ~1.2GB to ~340MB,
  a 72% reduction.
- Built a CI eval gate in GitHub Actions that acts as a standing quality contract. Nothing below
  ROC-AUC ≥ 0.80 reaches the MLflow registry. I verified it by shipping a deliberately degraded
  model, watching CI fail, then fixing it until it passed.
- Automated data-drift detection with Evidently on a reference-vs-current split. It logs a
  per-feature PSI score and trips a threshold alert past PSI > 0.15, which injected shift confirmed.

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
