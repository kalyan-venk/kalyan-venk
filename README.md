<div align="center">

```
Research Engineer  ·  LLMs  ·  AI Agents  ·  Evaluation & Reliability
```

# Kalyan Venkatesh

I recently completed an MS in Computer Science at DePaul University.

I build reliable AI systems across production engineering and graduate
research.

At sensen.ai I worked as a Software Engineer and served as the company's sole
Data Scientist. I built a production model-evaluation framework across 26 ANPR
deployments and worked with on-site teams and clients across 4 countries to
turn operational failures into measurable engineering problems.

My Master's Research carried that reliability question into LLM systems. I
built and evaluated a LangGraph Planner-Critic-Fixer pipeline across 5 local
model families, 10 experimental phases and 3 code benchmarks.

I am now building ChargeBack, an AI agent for card-fraud disputes built around
evaluation, observability and guardrails.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kalyan--venk-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/kalyan-venk)
[![Email](https://img.shields.io/badge/Email-adavivenkatesh@gmail.com-EA4335?style=flat-square&logo=gmail)](mailto:adavivenkatesh@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-kalyanvenk.com-8957e5?style=flat-square&logo=github)](https://kalyanvenk.com)

</div>

---

## Experience

### sensen.ai

#### Software Engineer
*Jan 2023 - Aug 2024*

- Owned an ANPR vehicle entry and exit classifier by designing the labeling
  scheme and fine-tuning a CNN on about 1,500 production images to about 90%
  accuracy.
- Engineered the production ML evaluation framework and business-error metric
  adopted across 26 parking deployments to surface about 5% unbillable sessions
  worth about $6K per month per site.
- Served as sensen's sole Data Scientist and forward-deployed technical contact
  across 4 countries while gathering requirements, mentoring 2 interns and
  self-deploying 300+ data products on AWS, Azure and GCP servers.
- Owned analytical SQL for 80 client deployments and turned about 30K weekly
  ANPR sightings into paired sessions, officer rankings and multi-level rollups.

#### Software Engineer Intern
*Aug 2022 - Jan 2023*

- Built 8 ticket-generation APIs on PL/pgSQL functions behind Spring Boot
  and designed an image-retention policy in Python that reclaimed 400+ GB and
  deferred server upgrades 4 to 5 months.

## Projects

### [ChargeBack](https://kalyanvenk.com/chargeback/) · [Source](https://github.com/kalyan-venk/chargeback-bro)

- Built a FastAPI chat service with streamed responses, multi-turn PostgreSQL
  memory and 3 tools for transaction lookup, fraud scoring and dispute filing.
- Modeled the workflow in 9 PostgreSQL tables and wrote a 2-pass Python ETL to
  load 555K+ transactions with linked cardholders, cards and merchants.
- Added policy guardrails, structured tool traces and a 7-case end-to-end
  evaluation suite that verifies dispute records and escalation paths.

### [Graduate Research: Multi-Agent LLM Systems & Reliability](https://kalyanvenk.com/inference-reliability)

- Built a LangGraph Planner-Critic-Fixer pipeline with AST checks, selective
  reversion and MLflow tracking across 5 local 3B-8B model families, 10
  experimental phases and 3 code benchmarks.
- Measured a +1.37-point average pass@1 gain across 9 conditions on a 3B planner
  but found monitoring reduced Qwen2.5 Coder 7B from 90% to 86%.

The first-author paper is under conference review. The code and detailed
observations remain anonymized to preserve double-blind review.

## Skills

**Languages** `Python` `SQL` `TypeScript`

**AI and Machine Learning** `LLMs` `LLM Agents` `LLM Evaluation`
`Multi-Agent Systems` `LangGraph` `MLflow` `PyTorch` `scikit-learn`
`Computer Vision` `CNNs` `Transfer Learning`

**Data and Backend** `PostgreSQL` `PL/pgSQL` `ETL` `FastAPI` `REST APIs` `Docker` `AWS` `Git` `Testing`

## Education

| | |
|---|---|
| **MS Computer Science** | DePaul University · Chicago, IL · Sep 2024 - Jun 2026 · GPA 3.88 |
| **BTech Engineering** | Visvesvaraya National Institute of Technology, Nagpur · Jul 2017 - May 2021 · GPA 7.85 |

## Certifications

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)** · Dec 2025 - Dec 2028

<div align="center">

*Open to Research Engineer and Software Engineer roles in LLMs, AI Agents and reliable production systems · adavivenkatesh@gmail.com*

</div>
