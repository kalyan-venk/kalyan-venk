<div align="center">

```
Research Engineer  ·  Multi-Agent Systems  ·  LLMs  ·  Computer Vision  ·  MSCS '26
```

# Kalyan Venkatesh

I just finished my Masters in Computer Science from DePaul University, Chicago in June 2026.
Over the past few years I've been focusing on one problem more or less: how to keep AI systems
reliable once they hit production.

At sensen.ai, the domain was Computer Vision. I built a vehicle direction classifier for one of
our parking clients by fine-tuning a CNN via transfer learning, and added the model validation
framework that checks whether a model is performing accurately or not. That went on to become the
company standard for ANPR evaluation.

My graduate research explored reliability in LLMs: is a multi-agent system more reliable than a
standalone agent at inference time? Knowing when to use monitoring and when not to is critical. I
built a 3-agent system, Planner, Critic and Fixer, in LangGraph. One thing that surprised me is
that great models often suffered because of monitoring. Have a glance at the work below or at
kalyanvenk.com.

Currently looking to join a team where I can solve some meaningful problems with my skills.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-kalyanvenk.com-8957e5?style=flat-square&logo=github)](https://kalyanvenk.com)

</div>

---

## Experience

### Graduate Research Engineer · DePaul University
*Sep 2025 - Jun 2026*

- Built a multi-agent system in LangGraph, pairing an LLM-as-a-judge critic with a self-correcting
  fixer for runtime hallucination detection in LLM code generation.
- Found monitoring benefit falls as model capability rises.

### Data Scientist · sensen.ai
*Aug 2022 - Aug 2024*

- Built an ANPR vehicle-direction classifier, a model-evaluation framework and a human-in-the-loop
  OCR flywheel.
- Built Brisbane's Officer Productivity scoring model and ticket-generation APIs, forward-deployed
  across sensen's entire global footprint.

### Data Engineer · Aecom & Siri
*May 2021 - Jul 2022*

- Built Python and Pandas ETL pipelines for data cleaning, monthly cost consolidation, and
  automated Excel, PDF and HTML reporting.
- Wrote analytical SQL across 2 infrastructure projects.

---

## Projects

### [Graduate Research: Multi-Agent Inference Reliability Framework](https://kalyanvenk.com/agentic-llmops)

Wanted to explore if a multi-agent system is more reliable than a standalone agent at inference
time. I picked code generation because the evaluation is straightforward, unlike natural language.
So I built a 3-agent system in LangGraph: a planner that writes the code, a critic that scores it
for hallucination, and a fixer that rewrites the code if the hallucination is above a threshold.
Across 5 model families and different phases of experimentation, monitoring benefit looks
inversely proportional to how capable the planner's own model is.

### [Inference-Lens: Adversarial Reliability of NLP Judges](https://kalyanvenk.com/inference-lens)

There are 3 ways to check the quality of AI work: force a fixed output format, which limits the
AI's capability; assign humans to review it, which doesn't scale; or have another AI grade the
work. It's easy to assume those judges are reliable. People are starting to think they can't be
trusted, but I tried to quantify it here: archetype classification with K-Means and DBSCAN,
encoders and tabular models trained to pick the better of 2 responses, then tested on a
purpose-built adversarial set. Full writeup on the site.

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
| **MS Computer Science** | DePaul University · Chicago, IL · Sep 2024 - Jun 2026 · GPA 3.88 |
| **BTech Engineering** | Visvesvaraya National Institute of Technology, Nagpur · Jul 2017 - May 2021 · GPA 7.85 |

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)** · Dec 2025 - Dec 2028
- **AWS Certified Machine Learning Engineer - Associate** · In progress

---

<div align="center">

*Open to AI Engineer · ML Engineer · Data Scientist · Data Engineer · Data Analyst · Research
Engineer · Forward Deployed Engineer roles · adavivenkatesh@gmail.com*

</div>
