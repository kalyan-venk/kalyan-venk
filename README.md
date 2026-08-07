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

### [Graduate Research Engineer · DePaul University](https://kalyanvenk.com/agentic-llmops) &nbsp; `LangGraph` `Ollama` `MLflow`
*Sep 2025 - Jun 2026*

- Designed a compound AI system in LangGraph and Ollama: a Planner writes, a Critic evaluates, a
  Fixer recovers from the errors. Ran it across 10 phases and 5 model families, evaluated on
  HumanEval-100, HumanEval+ and MBPP.
- Named the **Inverse Capability Hypothesis**: the critic-fixer monitoring loop helps weak base
  models (Code Llama) and hurts strong ones (Qwen). The benefit shrinks as baseline capability
  rises, and past a threshold it turns net-negative. Held across 3 independent trials.
- Built a **Selective Reversion Gate** that keeps only high-confidence fixer corrections and
  reverts the rest. The harness around it is reproducible: docker-compose, deterministic seeding,
  multi-trial runs, automated metric aggregation, all tracked in MLflow.

### Data Scientist · [sensen.ai](https://sensen.ai) &nbsp; `2022 - 2024`

- Shipped 8 SenFORCE ticket generation APIs, court-admissible image storage pipelines and
  time-based compression, running across AWS and Azure.
- Wrote the ANPR model evaluation pipelines used across 26 global deployments. sensen.ai adopted
  them as the standard model validation workflow.
- Tuned high-volume data workflows with PL/SQL functions and lighter image retrieval. Pipeline
  latency went from ~800ms to ~480ms.
- Replaced manual invoicing with end-to-end ETL pipelines over ~30k weekly ANPR sightings.
  Consolidation dropped from 10+ hrs a week to 2.
- Led R&D on industrial pollution enforcement with drone-based effluent sampling, designed to cover
  25-30 discharge points daily against weekly manual checks. That is 20-25x the coverage.

### Data Engineer · AECOM & Siri &nbsp; `2021 - 2022`

- Automated data preprocessing, cleaning and monthly cost consolidation pipelines in Python and
  Pandas. Dashboard preparation dropped ~60%, from 3 hrs to under 1.
- Wrote analytical SQL across 2 infrastructure project cost databases and got report runtime on
  client-facing deliverables from ~20s down to ~8s.

---

## Projects

### [Inference-Lens: Adversarial Reliability of NLP Evaluators](https://kalyanvenk.com/inference-lens) &nbsp; `DeBERTa-v3` `XGBoost` `LLM-Bar` `MLflow`
*Mar 2026 - Jun 2026*

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

### [PredictOps: End-to-End ML Serving Pipeline with Automated Eval Gating](https://kalyanvenk.com/predictops) &nbsp; `FastAPI` `ONNX Runtime` `Docker` `GitHub Actions` `MLflow` `Evidently`
*Jul 2026 - Present*

- Built a fraud-scoring API for card transactions (Sparkov data) where every feature is something
  a live authorization request can actually compute. XGBoost scored 0.6472 AUPRC on an out-of-time
  test split.
- Serves through FastAPI on ONNX Runtime only, no scikit-learn or XGBoost in the serving image. A
  CI gate in GitHub Actions blocks any model that falls below the AUPRC floor from reaching the
  MLflow registry, and an Evidently job monitors feature drift against the training distribution.

### [StreamLake: Streaming Lakehouse with Enforced Data Contracts](https://kalyanvenk.com/streamlake) &nbsp; `Kafka` `Spark` `Iceberg` `dbt` `Airflow`
*Jul 2026 - Present*

- Built a card-transaction fraud lakehouse: Sparkov data ingested twice, batch and a live Kafka
  stream, into Iceberg, modeled with dbt, orchestrated by Airflow.
- Every hop asserts a data contract in YAML and quarantines the rows that break it, instead of
  failing silently or letting a broken row reach the warehouse.

---

## Skills

**Languages** `Python` `SQL`

**AI/ML** `LangGraph` `LangChain` `Agentic AI` `Multi-Agent Systems` `Tool Use` `Prompt Engineering` `LLM Evaluation` `HuggingFace Transformers` `Fine-tuning` `Embeddings` `Scikit-learn` `XGBoost`

**MLOps & Serving** `MLflow` `Weights & Biases` `FastAPI` `Model Serving` `Ollama` `Docker` `GitHub Actions (CI/CD)` `Pydantic` `Evidently` `Data Drift Monitoring`

**Reliability & Evaluation** `Imbalanced Classification` `Adversarial Evaluation` `Experimental Design`

**Cloud & Data** `AWS` `PostgreSQL` `NumPy` `Pandas` `Git`

---

## Education

| | |
|---|---|
| **MS Computer Science** | DePaul University · Chicago, IL · Sep 2024 - Jun 2026 |
| **BTech Engineering** | National Institute of Technology · Nagpur, India · Jul 2017 - May 2021 |

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)**
- **AWS Certified Machine Learning Engineer - Associate** · In progress

---

<div align="center">

*Open to AI Engineer · ML Engineer · Data Scientist · Software Engineer roles*

</div>
