<!-- ====================== HEADER ====================== -->
<div align="center">

<!-- Animated waving banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6C8EBF,50:4B6BFB,100:29B5E8&height=210&section=header&text=Shailesh%20Tripathi&fontSize=52&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=AI%20Solutions%20Architect%20%C2%B7%20Agentic%20Systems%20%C2%B7%20Applied%20Research&descAlignY=58&descSize=18&descAlignX=50" width="100%" alt="Shailesh Tripathi — AI Solutions Architect" />

<a href="https://github.com/shaileshai"><img src="https://komarev.com/ghpvc/?username=shaileshai&label=Profile%20views&color=4B6BFB&style=flat" alt="Profile views" /></a>

<a href="https://shaileshtripathi.netlify.app">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3200&pause=900&color=6C8EBF&center=true&vCenter=true&width=820&lines=AI+Solutions+Architect;Agentic+Systems+%7C+Applied+Research+%7C+Data+Platforms;I+design+AI+systems+that+ship+%E2%80%94+and+I+measure+them." alt="Shailesh Tripathi — AI Solutions Architect" />
</a>

I architect production AI systems end-to-end — from retrieval and agent orchestration down to the token economics — and I publish the results with statistical rigor. ~10 years across BI/data consulting, full-stack engineering, and applied AI.

<a href="https://www.linkedin.com/in/shaileshtripathi003/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://shaileshtripathi.netlify.app"><img src="https://img.shields.io/badge/Portfolio-1a1a2e?style=for-the-badge&logo=firefox&logoColor=white" alt="Portfolio" /></a>
<a href="https://zenodo.org/records/19477107"><img src="https://img.shields.io/badge/Published_Research-Zenodo-4B6BFB?style=for-the-badge&logo=zenodo&logoColor=white" alt="Research" /></a>
<a href="mailto:shaileshtripathi003@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

</div>

---

## 🎯 What I Do

I sit at the intersection of **AI research and production engineering** — the seam where most AI initiatives stall. My focus:

- **Agentic architecture** — multi-agent orchestration, tool/function calling, MCP (Model Context Protocol), and the retrieval layers that make agents reliable at scale.
- **LLM systems economics** — treating tokens, latency, and context as first-class architectural constraints. My research quantifies these tradeoffs instead of hand-waving them.
- **Data platforms** — lakehouse and warehouse-native AI (Databricks, Snowflake), pipeline automation, and knowledge-graph-backed context.
- **From PoC to production** — the unglamorous 80%: evaluation harnesses, A/B experimentation, observability, and cost governance that turn a demo into a system a business can trust.

> I don't ship claims I can't measure. Two of my systems below are backed by controlled experiments with reported effect sizes and p-values.

---

## 📄 Published Research

Peer-reviewable preprints on LLM agent efficiency and self-improving retrieval systems. Both introduce novel, empirically-validated architectures.

### Karna: Reducing LLM Coding-Agent Token Consumption by 58% via Persistent Code Knowledge Graphs
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19433427-4B6BFB?style=flat-square&logo=doi)](https://zenodo.org/records/19433427)

A persistent **code knowledge graph** that delivers structured codebase context to AI agents over **MCP**, replacing brute-force file reads.
- **57.9% input-token savings** over a file-reading baseline in a controlled A/B experiment on a **1,125-file codebase** (Claude Sonnet 4).
- Statistically decisive: **p < 0.007, Cohen's d = 2.96** (a very large effect size).
- Formalizes the **"conversation-history tax"** — the *O(T²)* growth in cumulative input tokens as agent turn-count rises — a cost driver that affects every tool-augmented LLM system.

### Self-Evolving Context Layers: Implicit Learning from Agent Behavior in Code Knowledge Graphs
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19477107-4B6BFB?style=flat-square&logo=doi)](https://zenodo.org/records/19477107)

A three-loop **self-improvement system** built on Karna that learns from how agents actually use context — no manual tuning.
- Introduces **"gap signals"**: implicit metrics derived from the discrepancy between what a context tool *returns* and what the agent *uses*.
- Validated across **70 live agent sessions** (A/B, Claude Sonnet 4 via Cursor Agent CLI): the adaptive system produced **79.3% more exploratory tool calls** (p = 0.010) and surfaced **46.4% more relevant entities per session**.

<sub>📚 Full author profile & citations → **[Zenodo](https://zenodo.org/search?q=Tripathi%2C%20Shailesh)** &nbsp;·&nbsp; 💻 Reference implementation → **[karna-ai](https://github.com/shaileshai/karna-ai)**</sub>

---

## 🏗️ Selected Systems

Architecture and engineering I've led — from open-source frameworks to enterprise platforms.

| System | What it is | Architecture highlights |
|---|---|---|
| **[Karna](https://github.com/shaileshai/karna-ai)** 🔬 | Persistent code knowledge graph for LLM agents (MCP server) | Entity resolution · graph-backed retrieval · 58% token reduction (peer-reviewed) |
| **[Zeus](https://github.com/shaileshai/zeus)** ⚡ | Autonomous data-foundation agent | Provisions **Fivetran → BigQuery** pipelines under **human-in-the-loop** approval |
| **Vesh Agents** 🤖 | Open-source agentic framework (Apache 2.0, `pip install vesh-agents`) | 6-agent orchestration for revenue intelligence · pluggable tools |
| **Vesh AI Platform** 📊 | Managed intelligence layer for enterprise revenue teams | Multi-tenant · retrieval + agents over business data |
| **Odin AI · CodeOps** 🛠️ | Enterprise developer-automation & CI/CD intelligence | Agentic workflows over engineering systems |
| **DataGuardian AI** 🛡️ | AI-powered data-quality management | Anomaly detection · governance at the warehouse layer |
| **CreditIntel.AI** 💳 | Multi-agent AI credit-scoring system | Explainable, agent-orchestrated decisioning |

<sub>Several enterprise systems live in private repos — happy to walk through architecture and tradeoffs in conversation.</sub>

---

## 🧰 Architecture & Platform Stack

**AI / LLM Systems**
<br>
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-000000?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_%26_Vector_Search-5A67D8?style=flat-square)
![Agents](https://img.shields.io/badge/Multi--Agent_Orchestration-6C8EBF?style=flat-square)

**Cloud & Data Platforms**
<br>
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat-square&logo=googlebigquery&logoColor=white)
![Fivetran](https://img.shields.io/badge/Fivetran-1A73E8?style=flat-square)

**Engineering**
<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

---

## 📈 GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=shaileshai&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub Stats" />
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=shaileshai&theme=tokyonight&hide_border=true" alt="GitHub Streak" />

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shaileshai&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" />

<!-- Animated contribution activity graph -->
<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=shaileshai&theme=tokyo-night&hide_border=true&area=true&custom_title=Contribution%20Activity" alt="Activity Graph" />

<!-- Animated contribution snake (generated by the workflow in .github/workflows) -->
<img width="98%" src="https://raw.githubusercontent.com/shaileshai/shaileshai/output/snake-dark.svg" alt="Contribution Snake" />

<!-- Profile trophies -->
<img src="https://github-profile-trophy.vercel.app/?username=shaileshai&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&row=1&column=7" alt="Trophies" />

</div>

---

<div align="center">

### 🤝 Let's build the next generation of AI systems

I'm exploring **AI Solutions Architect** roles where research-grade thinking meets production scale.

<a href="https://www.linkedin.com/in/shaileshtripathi003/"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://shaileshtripathi.netlify.app"><img src="https://img.shields.io/badge/View_Portfolio-1a1a2e?style=for-the-badge&logo=firefox&logoColor=white" alt="Portfolio" /></a>

<sub><i>Architecture is the art of measurable tradeoffs. I bring the receipts.</i></sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:29B5E8,50:4B6BFB,100:6C8EBF&height=120&section=footer" width="100%" alt="" />
