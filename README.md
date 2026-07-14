<div align="center">

```
ML Engineer  ·  NLP  ·  LLM Evaluation  ·  MLOps
```

# Kalyan Venkatesh

**Most LLM reliability work assumes the problem is the model.**
I think the problem is the system around the model: the evaluation loop, the pipeline architecture,
the assumptions baked into how we measure failure.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-kalyan--venk.github.io-8957e5?style=flat-square&logo=github)](https://kalyan-venk.github.io)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Inference--Lens-22d3ee?style=flat-square&logo=github)](https://kalyan-venk.github.io/play.html)

</div>

---

| | |
|---|---|
| **MS Computer Science** | DePaul University · Jun 2026 · GPA 3.84 |
| **Production ML** | 3+ years · sensen.ai · 26 global deployments |
| **Research** | LLM inference reliability · 2 systems under faculty supervision |
| **Availability** | OPT eligible Jun 2026 · Open to DS / MLE / AI Engineer / SWE roles |

---

## Research

### [Multi-Agent Inference Reliability Framework](https://kalyan-venk.github.io/agentic-llmops.html) &nbsp; `LangGraph` `Ollama` `HumanEval`
*DePaul University · Supervised by Prof. Vahid Alizadeh · Jan 2026 - Jun 2026*

> Can a lightweight 3-agent runtime (Planner → Critic → Fixer) fix LLM failures without touching model weights?
> Yes. But not the way you'd expect.

Built across **10 phases · 5 model families · hundreds of experimental conditions**.

| Finding | Result |
|---|---|
| Upgrading the Critic (3B → 8B) made **18 conditions net-negative** | Stronger critics are confidently wrong in new ways |
| **Inverse Capability Hypothesis**: interventions help weak models, hurt strong ones | Validated across all 4 families. Crossover at ~65% pass@1 |
| **Selective Reversion Gate** reverts 73.4% of degraded fixer outputs | **+4.85 pp pass@1** (95% CI [+3.36, +6.34], p = 0.010) |
| Threshold sweep across 6 values, τ = 0.70 optimal | Latency: 7.89s → 4.79s · Trigger rate down 78% |

Statistically validated across 3 independent trials. Currently under peer review.

---

### [Inference-Lens](https://kalyan-venk.github.io/inference-lens.html) &nbsp; `NLP` `DeBERTa-v3` `XGBoost` `MLflow` `LLM-Bar`
*DePaul University · Supervised by Prof. Bamshad Mobasher · May 2026 - Jun 2026*

> LLM-as-judge is the default eval paradigm. Almost nobody is asking how easily the judge can be deceived.

**[Try the live scorer](https://kalyan-venk.github.io/play.html)** and watch an automated NLP judge pick the worse response in real time.

Built an end-to-end NLP text classification pipeline to stress-test evaluator reliability under systematic adversarial pressure. The core task: can a model learn what humans genuinely prefer in natural language responses?

| What I Built | Scale |
|---|---|
| NLP text classification (LR, XGBoost, DeBERTa-v3) benchmarked against adversarial NLP inputs | 419 LLM-Bar pairs across 4 NLP perturbation categories |
| Response archetype clustering to map structural vulnerability in natural language | 170K+ Anthropic HH-RLHF human preference annotations |
| 5-fold CV supervised NLP pipeline + MLflow artifact versioning | ~0.50 AUC-ROC across all 3 models, the finding rather than a shortfall |
| Real-time Streamlit NLP evaluation interface | Per-feature verdict breakdowns |

The goal isn't just "can we fool the NLP judge." It's finding *which classes of natural language outputs are vulnerable*, so you can build evaluators that aren't.

---

## Engineering

### [PredictOps](https://kalyan-venk.github.io/predictops.html) &nbsp; `FastAPI` `Docker` `MLflow` `GitHub Actions` `Evidently`
*Personal project · build in progress*

> Most ML portfolio projects stop at a trained model. This one is about everything after.

A deliberately boring tabular model (customer churn, never the headline) with all the depth put into the ops loop around it. Logistic Regression beat XGBoost on cross-validated ROC-AUC, 0.846 vs 0.842, so the simpler model is what actually got served. A validated FastAPI serving layer (`/health` `/predict` `/info` `/reload`) and a multi-stage Docker build are done too. **3 of 7 planned phases shipped.** Next: a GitHub Actions CI eval gate that fails a build if a model doesn't clear a quality threshold, then MLflow registry promotion and Evidently drift detection.

Also building: **hawk-eye-geospatial**, a satellite change-detection project with a calibrated-uncertainty reliability layer. On hold while I focus on PredictOps, no results to report yet.

---

## Industry

**Data Scientist · [sensen.ai](https://sensen.ai)** `2022 - 2024`
- ANPR model evaluation pipelines across 26 global deployments, later adopted as the standard validation workflow
- Led R&D on industrial pollution enforcement: drone-based effluent sampling, 20-25x increase in regulatory coverage
- ETL automation cutting consolidation from 10+ hrs to 2 hrs/week across ~30K weekly sightings

**Data Engineer · AECOM & Siri** `2021 - 2022`
- Forecasting and data integration pipelines for asset lifecycle management across 25+ locations

---

## Stack

`Python` `Java` `Spring Boot` `NLP` `SQL` `PostgreSQL` `PyTorch` `HuggingFace Transformers` `LangChain` `LangGraph` `Scikit-learn` `XGBoost` `DeBERTa` `LoRA/PEFT`
`MLflow` `FastAPI` `Pydantic` `Evidently` `Streamlit` `Docker` `Kubernetes` `AWS (S3 · EC2 · SageMaker)` `GitHub Actions`
`LLM-as-Judge` `FAISS` `Ollama` `Adversarial NLP` `text classification` `Prompt Engineering` `McNemar's test` `SHAP` `Data structures` `REST APIs`

---

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)** · Dec 2025
- **AWS Certified ML Engineer Associate** · In progress · Jun 2026

---

<div align="center">

*Open to Data Scientist · ML Engineer · AI Engineer · Software Engineer roles*

</div>
