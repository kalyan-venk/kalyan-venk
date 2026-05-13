# Kalyan Venkatesh

Data Scientist · AI/ML Engineer · MS Computer Science, DePaul University (June 2026, GPA 3.84)
3+ years of production ML at sensen.ai before the research pivot.

[LinkedIn](https://linkedin.com/in/kalyan-venk) · [adavivenkatesh@gmail.com](mailto:adavivenkatesh@gmail.com)

---

## One thread connects everything I build

Most LLM reliability work assumes the problem is the model.
I think the problem is often the *system around the model* — the evaluation loop, the pipeline architecture, the assumptions baked into how we measure failure.

---

## Research

### [Multi-Agent Inference Reliability Framework](https://github.com/kalyan-venk/agentic-llmops)
*Supervised by Prof. Vahid Alizadeh · DePaul University · Jan 2026 – Present*

> Can a lightweight 3-agent runtime (Planner → Critic → Fixer) fix LLM failures without touching the model weights? Yes. But not the way you'd expect.

Built with LangGraph across **6 phases · 4 model families · 36 experimental conditions**.

**What I found:**

| Finding | What it means |
|---|---|
| Critic 3B → 8B upgrade made **18 conditions net-negative** | Stronger critics are confidently wrong in new ways |
| **Inverse Capability Hypothesis** validated across all 4 families | Interventions help low-capability models (+32 pp for Code Llama 7B). They hurt strong ones. Crossover: ~65% pass@1 |
| **Selective Reversion Gate** reverts 73.4% of degraded outputs | +4.85 pp pass@1 (p=0.01), latency cut from 7.89s → 4.79s |
| Threshold sweep across 6 values, τ=0.70 optimal | Trigger rate down 78% without sacrificing reliability |

Full implementation, all experiment results, and the research report are in the repo.

---

### [Inference-Lens](https://github.com/kalyan-venk/Inference-Lens)
*Supervised by Prof. Bamshad Mobasher · DePaul University · May 2026 – Present*

> LLM-as-judge is the default eval paradigm now. Almost nobody is asking how easily the judge can be deceived. I am.

Built a system to stress-test evaluator reliability under systematic judge deception.

**What I built:**

- Benchmarked **Logistic Regression · XGBoost · DeBERTa-v3** across 419 LLM-Bar adversarial inputs
- Clustered **170K+ Anthropic HH-RLHF** preference pairs (K-Means, DBSCAN, hierarchical) to find which response archetypes are structurally most exploitable
- 5-fold cross-validated supervised pipeline targeting **AUC-ROC > 0.82**, tracked via MLflow
- Deployed as a Streamlit interface for real-time LLM output evaluation

The goal is not just "can we fool the judge." It's finding *which classes of outputs are vulnerable* — so you can build evaluators that aren't.

---

## Stack

```
Languages     Python · SQL · PostgreSQL · Oracle SQL
AI / ML       PyTorch · TensorFlow · Scikit-learn · LangChain · LangGraph · vLLM
MLOps         MLflow · Docker · Kubernetes · Airflow · dbt · AWS (S3, EC2, SageMaker)
Infra         GitHub Actions · CI/CD
```

---

## Before the research

**sensen.ai** `2022 – 2024` · Data Scientist
- ANPR accuracy analytics across 26 projects; automated benchmarking and drift detection across 5 KPIs
- ETL pipelines via dbt that nearly doubled processing efficiency
- Led R&D on industrial pollution anomaly detection using drone GPS, sensor telemetry, and server-based ingestion

**AECOM & Siri** `2021 – 2022` · Data Engineer
- Forecasting and data integration pipelines for asset lifecycle management across 25+ locations

---

## Certifications

- AWS Certified Cloud Practitioner `Dec 2025`
- AWS Certified Machine Learning Engineer Associate `In progress · Jun 2026`

---

Available on OPT from June 2026. Open to **Data Scientist**, **ML Engineer**, and **AI Engineer** roles.
[LinkedIn](https://linkedin.com/in/kalyan-venk) · [adavivenkatesh@gmail.com](mailto:adavivenkatesh@gmail.com)
