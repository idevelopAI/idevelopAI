<div align="center">

<p><sub>AI ENGINEERING · EVALUATION · BACKEND SYSTEMS</sub></p>
<h1>Nika Akophiani</h1>
<h3>I build AI applications you can inspect, evaluate, and trust.</h3>
<p>AI/ML Engineer based in Germany.<br>Python services, reliable evaluation infrastructure, and useful applications built around LLMs.</p>

<p>
<a href="https://llm-eval-control-plane.nick0ne.chatgpt.site/"><img alt="Explore the evaluation dashboard demo" src="https://img.shields.io/badge/Explore_the_demo-2563EB?style=for-the-badge"></a>
<a href="https://github.com/idevelopAI?tab=repositories"><img alt="Browse all public repositories" src="https://img.shields.io/badge/Browse_the_code-161B22?style=for-the-badge&amp;logo=github&amp;logoColor=white"></a>
</p>

<p><sub>LLM evaluation · Retrieval-augmented generation · Text-to-SQL · API design · PostgreSQL · CI/CD</sub></p>

</div>

---

I work across the full application: model integration, data access, APIs, background workers, interfaces, and automated checks. My projects focus on **measuring AI behavior, protecting data, and making failures recoverable**.

## Explore my projects

| Project | What it solves | Start here |
| :--- | :--- | :--- |
| **[LLM Eval Control Plane](https://github.com/idevelopAI/llm-eval-control-plane)** | Evaluate AI changes and explain release decisions | [Public demo](https://llm-eval-control-plane.nick0ne.chatgpt.site/) |
| **[DataBridge AI](https://github.com/idevelopAI/databridge-ai)** | Ask PostgreSQL questions in English or German with read-only safeguards | [75-second walkthrough](https://github.com/idevelopAI/databridge-ai/blob/main/docs/demo.mp4) |
| **[GenAI Knowledge Base](https://github.com/idevelopAI/genai-knowledge-base)** | Ask questions across PDFs and inspect the sources | [Screenshots & setup](https://github.com/idevelopAI/genai-knowledge-base#screenshots) |

## 01 / LLM Eval Control Plane

**Evaluation infrastructure · Featured project**

Should an AI change ship? This control plane compares baseline and candidate runs, enforces release policies, and preserves the evidence behind each decision.

<a href="https://llm-eval-control-plane.nick0ne.chatgpt.site/"><img width="100%" alt="Synthetic release dashboard showing a blocked release, failed policy gate, and case-level scoring evidence" src="https://raw.githubusercontent.com/idevelopAI/llm-eval-control-plane/main/docs/assets/release-dashboard-fixture.jpg"></a>

<sub>Public demo uses synthetic evaluation evidence; no API or model calls.</sub>

- **Reproducible evaluation:** versioned datasets, immutable artifacts, and gates for specific safety and language groups.
- **Resilient execution:** PostgreSQL jobs, idempotent submissions, worker leases, cancellation, recovery, and fenced evidence publication.
- **Reviewable decisions:** case-level comparisons, redacted dashboard views, and telemetry that excludes evaluation content.

The documented offline DataBridge evaluation covers **56 English/German cases**: all seven baseline gates pass, and six gates block four deliberately introduced regressions.

`Python` `FastAPI` `PostgreSQL` `SQLAlchemy` `React` `TypeScript` `Docker`

**[Explore demo →](https://llm-eval-control-plane.nick0ne.chatgpt.site/)** &nbsp; [Source code](https://github.com/idevelopAI/llm-eval-control-plane) &nbsp; [Architecture](https://github.com/idevelopAI/llm-eval-control-plane/blob/main/docs/architecture.md) &nbsp; [Release checks](https://github.com/idevelopAI/llm-eval-control-plane/actions)

---

## 02 / DataBridge AI

**Applied AI · Database safety**

A natural-language interface for PostgreSQL that turns English or German questions into inspectable SQL, answers, tables, charts, and CSV exports.

<a href="https://github.com/idevelopAI/databridge-ai/blob/main/docs/demo.mp4"><img width="100%" alt="DataBridge AI interface with natural-language database questions and structured query results" src="https://raw.githubusercontent.com/idevelopAI/databridge-ai/main/docs/screenshot.jpg"></a>

- **Independent safeguards:** SQL validation, restricted database roles, query-plan limits, and privacy masking.
- **Clearer interactions:** ambiguity checks request clarification before a model call; bilingual business definitions guide queries.
- **Easy to review:** recorded demo mode exercises the real validation and database workflow without a model API key.

`Python` `FastAPI` `LangChain` `Gemini` `PostgreSQL` `SQLGlot` `Streamlit`

**[Watch the walkthrough →](https://github.com/idevelopAI/databridge-ai/blob/main/docs/demo.mp4)** &nbsp; [Source code](https://github.com/idevelopAI/databridge-ai) &nbsp; [Run the no-key demo](https://github.com/idevelopAI/databridge-ai#no-key-demo)

---

## 03 / GenAI Knowledge Base

**Retrieval-augmented generation · Document workflows**

A local RAG application for asking questions across PDFs, with document names, page references, and supporting excerpts attached to answers.

<a href="https://github.com/idevelopAI/genai-knowledge-base"><img width="100%" alt="GenAI Knowledge Base chat displaying an answer and expandable document source citations" src="https://raw.githubusercontent.com/idevelopAI/genai-knowledge-base/main/docs/screenshots/chat-with-sources.png"></a>

- **Traceable answers:** document-scoped retrieval, relevance filtering, and source citations.
- **Safer ingestion:** validated PDFs, bounded background jobs, and versioned indexes that preserve the active collection when a rebuild fails.
- **Failure handling:** response caching, provider circuit breaking, and an optional local generation fallback.

`Python` `FastAPI` `ChromaDB` `LangChain` `Gemini` `Streamlit` `Docker`

**[Explore the project →](https://github.com/idevelopAI/genai-knowledge-base)** &nbsp; [Evaluation approach](https://github.com/idevelopAI/genai-knowledge-base#evaluation) &nbsp; [Local setup](https://github.com/idevelopAI/genai-knowledge-base#local-setup)

## Engineering strengths

| Area | Demonstrated in these projects |
| :--- | :--- |
| **AI & evaluation** | LLM integration, RAG, text-to-SQL, deterministic scoring, regression checks |
| **Backend & data** | FastAPI, Pydantic, PostgreSQL, SQLAlchemy, durable jobs, API contracts |
| **Reliability & security** | Recovery, scoped authentication, read-only access, privacy-aware telemetry |
| **Delivery & interfaces** | Docker, GitHub Actions, automated tests, React, TypeScript, Streamlit |

<details>
<summary><strong>How the projects fit together</strong></summary>

DataBridge AI and GenAI Knowledge Base explore two practical AI workflows: querying structured data and retrieving document knowledge. LLM Eval Control Plane extends that work into evaluation infrastructure, including a PostgreSQL replay suite for DataBridge. Together, they show how I connect application development with evidence, safety checks, and operational reliability.

</details>

---

<div align="center">
<strong>Useful AI. Inspectable behavior. Careful engineering.</strong>
<p><a href="https://github.com/idevelopAI?tab=repositories">Explore all public repositories</a> · <a href="https://github.com/idevelopAI/idevelopAI">Profile source</a></p>
</div>
