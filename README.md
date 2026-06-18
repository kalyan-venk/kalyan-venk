<div align="center">

```
ML Engineer  ·  LLM Evaluation  ·  AI Systems
```

# Kalyan Venkatesh

**Most LLM reliability work assumes the problem is the model.**
I think the problem is the system around the model - the evaluation loop, the pipeline architecture,
the assumptions baked into how we measure failure.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Research-agentic--llmops-58a6ff?style=flat-square&logo=github)](https://kalyan-venk.github.io/agentic-llmops/)

</div>

---

| | |
|---|---|
| **MS Computer Science** | DePaul University · Jun 2026 · GPA 3.84 |
| **Production ML** | 3+ years · sensen.ai · 26 global deployments |
| **Research** | LLM inference reliability · 2 systems under faculty supervision |
| **Availability** | OPT eligible Jun 2026 · Open to DS / MLE / AI Engineer roles |

---

## Research

### [Multi-Agent Inference Reliability Framework](https://kalyan-venk.github.io/agentic-llmops/) &nbsp; `LangGraph` `Ollama` `HumanEval`
*DePaul University · Supervised by Prof. Vahid Alizadeh · Jan 2026 – Present*

> Can a lightweight 3-agent runtime (Planner → Critic → Fixer) fix LLM failures without touching model weights?
> Yes. But not the way you'd expect.

Built across **6 phases · 4 model families · 36 experimental conditions**.

| Finding | Result |
|---|---|
| Upgrading the Critic (3B → 8B) made **18 conditions net-negative** | Stronger critics are confidently wrong in new ways |
| **Inverse Capability Hypothesis** -- interventions help weak models, hurt strong ones | Validated across all 4 families. Crossover at ~65% pass@1 |
| **Selective Reversion Gate** reverts 73.4% of degraded fixer outputs | **+4.85 pp pass@1** (95% CI [+3.36, +6.34], p = 0.010) |
| Threshold sweep across 6 values, τ = 0.70 optimal | Latency: 7.89s → 4.79s · Trigger rate down 78% |

Statistically validated across 3 independent trials. Targeting ICSE 2027.

---

### [Inference-Lens](https://kalyan-venk.github.io/Inference-Lens/) &nbsp; `DeBERTa-v3` `XGBoost` `MLflow` `LLM-Bar`
*DePaul University · Supervised by Prof. Bamshad Mobasher · May 2026 – Present*

> LLM-as-judge is the default eval paradigm. Almost nobody is asking how easily the judge can be deceived.

Built a system to stress-test evaluator reliability under systematic adversarial pressure.

| What I Built | Scale |
|---|---|
| Benchmarked LR · XGBoost · DeBERTa-v3 against adversarial inputs | 419 LLM-Bar pairs across 4 perturbation categories |
| Response archetype clustering to map structural vulnerability | 170K+ Anthropic HH-RLHF preference annotations |
| 5-fold CV supervised pipeline + MLflow artifact versioning | AUC-ROC target > 0.82 |
| Real-time Streamlit evaluation interface | Per-feature verdict breakdowns |

The goal isn't just "can we fool the judge." It's finding *which classes of outputs are vulnerable* -- so you can build evaluators that aren't.

---

## Industry

**Data Scientist · [sensen.ai](https://sensen.ai)** `2022 – 2024`
- ANPR model evaluation pipelines across 26 global deployments -- adopted as the standard validation workflow
- Led R&D on industrial pollution enforcement: drone-based effluent sampling, 20-25x increase in regulatory coverage
- ETL automation cutting consolidation from 10+ hrs to 2 hrs/week across ~30K weekly sightings

**Data Engineer · AECOM & Siri** `2021 – 2022`
- Forecasting and data integration pipelines for asset lifecycle management across 25+ locations

---

## Stack

`Python` `SQL` `PyTorch` `HuggingFace Transformers` `LangChain` `LangGraph` `Scikit-learn` `XGBoost` `DeBERTa` `LoRA/PEFT`
`MLflow` `FastAPI` `Streamlit` `Docker` `Kubernetes` `AWS (S3 · EC2 · SageMaker)` `GitHub Actions`
`LLM-as-Judge` `FAISS` `Ollama` `Adversarial ML` `Prompt Engineering` `McNemar's test` `SHAP`

---

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)** · Dec 2025
- **AWS Certified ML Engineer Associate** · In progress · Jun 2026

---

<div align="center">

*Open to Data Scientist · ML Engineer · AI Engineer roles*

</div>
