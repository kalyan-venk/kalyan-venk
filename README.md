<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/kalyan-venk/kalyan-venk/9e96206423db587a435d549fe871a185e34a0e20/assets/name-dark.svg">
  <img src="https://raw.githubusercontent.com/kalyan-venk/kalyan-venk/9e96206423db587a435d549fe871a185e34a0e20/assets/name-light.svg" alt="Kalyan Venkatesh - Software Engineer" width="360" height="78">
</picture>

<p align="center">
  <a href="https://linkedin.com/in/kalyan-venk" title="LinkedIn"><img src="https://raw.githubusercontent.com/kalyan-venk/kalyan-venk/9e96206423db587a435d549fe871a185e34a0e20/assets/linkedin.svg" alt="LinkedIn" width="24" height="24"></a>&nbsp;&nbsp;&nbsp;
  <a href="mailto:adavivenkatesh@gmail.com" title="Email"><img src="https://raw.githubusercontent.com/kalyan-venk/kalyan-venk/9e96206423db587a435d549fe871a185e34a0e20/assets/email.svg" alt="Email" width="24" height="24"></a>&nbsp;&nbsp;&nbsp;
  <a href="https://kalyanvenk.com/" title="Portfolio"><img src="https://raw.githubusercontent.com/kalyan-venk/kalyan-venk/9e96206423db587a435d549fe871a185e34a0e20/assets/portfolio.svg" alt="Portfolio" width="24" height="24"></a>
</p>

</div>

Hey! I'm a Software Engineer with 2 years of work experience. I specialize in making AI systems reliable in production.

At sensen.ai I worked as a Software Engineer and served as the company's sole Data Scientist. I built a production model-evaluation framework across 26 parking deployments and worked with on-site teams and clients across 4 countries to turn operational failures into measurable engineering problems.

My Master's Research carried the same question into LLM systems. I built a multi-agent Planner-Critic-Fixer pipeline to detect and repair generated-code errors at inference time. My research paper is under conference review.

Lately I'm building an end-to-end system with AI agents for credit card fraud disputes, focusing on LLM evaluation, observability & guardrails.

<br>

## SKILLS

| Category | Skills |
|---|---|
| **Languages & Frameworks** | Python, SQL, TypeScript, React |
| **AI & ML** | PyTorch, AI Agents, Prompt Engineering, LLM Evaluation, Benchmarking, Observability |
| **Data** | PostgreSQL, Data Modeling, Data Pipelines, ETL, Pandas, NumPy, Data Quality / Validation |
| **Engineering** | System Design, Software Testing, AI-Assisted Development |
| **Backend & Delivery** | MLOps, FastAPI, Docker, AWS, Linux, Git |

<br>

## WORK EXPERIENCE

**sensen.ai | Software Engineer** · Jan 2023 - Aug 2024

- Owned ANPR vehicle entry & exit classifier for parking deployments, designed the labeling scheme, curated, annotated & augmented ~1,500 balanced production images & fine-tuned a CNN through transfer learning to achieve ~90% accuracy at initial deployment.
- Engineered a production ML evaluation framework & business-error metric that sensen adopted as standard across 26 parking deployments, running 24x7 against live ANPR data to surface ~5% unbillable parking sessions worth ~$6K per month per site.
- Designed a human-in-the-loop OCR correction pipeline that turned 400+ officer corrections per client each year into retraining data, lifting plate-read accuracy from ~90% to ~93% in the first production cycle.
- Served as sensen's sole Data Scientist, gathering requirements from clients & on-site stakeholders, scoping feasibility & building & deploying 300+ data products across 4+ countries on AWS, Azure & GCP servers.
- Owned analytical SQL for 80+ client deployments, turning ~30K weekly ANPR sightings into paired sessions, officer rankings & multi-level rollups through ~25 materialized views, window functions & parameterized PL/pgSQL functions from one shared codebase.

**sensen.ai | Software Engineer Intern** · Aug 2022 - Jan 2023

- Built 8 ticket-generation APIs backed by PL/pgSQL functions & designed an age-based image-retention policy, compressing old captures in Python at 10-30% level above the legal legibility floor, reclaiming 400+ GB & deferring server upgrades 4-5 months.

<br>

## PROJECTS

### [ChargeBack: AI agent for credit card fraud disputes built around evaluation, observability & guardrails](https://kalyanvenk.com/chargeback/)

- Built an LLM-powered dispute assistant using Python, FastAPI & PostgreSQL with streamed conversations for transaction lookup, risk scoring & filing, reducing median response latency by 20% through tool-result reuse.
- Developed reusable React & TypeScript components with typed props, shared state & controlled forms, rejecting invalid inputs & preserving dispute data across API failures with loading/error feedback.
- Prevented duplicate disputes in 100 repeated & concurrent filing attempts using PostgreSQL unique constraints & idempotency, enforcing customer isolation with server-side authorization & SQL ownership checks.
- Built pytest regression tests with deterministic LLM fixtures, JSON Schema validation & database assertions, catching invalid tool calls, runaway loops, timeouts & false success claims through tool traces.
- Cut tokens per completed dispute by 15% by filtering persisted conversation history into concise model context, retaining transaction details & tool results needed to resolve multi-turn follow-ups correctly.

### [Graduate Research: Runtime Hallucination Monitoring in Multi-Agent LLM Systems](https://kalyanvenk.com/inference-reliability)

*Under review*

- Architected a LangGraph Planner-Critic-Fixer pipeline with AST checks, selective reversion & MLflow tracking across 5 local 3B-8B model families, 10 experimental phases & 3 code benchmarks.
- Measured a +1.37-point average pass@1 gain across 9 conditions on a 3B planner but found naive monitoring reduced Qwen2.5 Coder 7B from 90% to 86% (p=0.020), showing it can harm stronger models.

<br>

## EDUCATION

<table>
  <tr>
    <td><strong>MS Computer Science</strong></td>
    <td>DePaul University · Chicago, IL · Sep 2024 - Jun 2026 · GPA 3.88</td>
  </tr>
  <tr>
    <td><strong>BTech Engineering</strong></td>
    <td>Visvesvaraya National Institute of Technology, Nagpur · Jul 2017 - May 2021 · GPA 7.85</td>
  </tr>
</table>

<br>

## CERTIFICATIONS

- **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/3cb43cfd-9b9c-42e1-a13b-26fa16bf0cbe/public_url)**
