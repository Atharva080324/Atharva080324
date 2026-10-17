# Hi, I'm Atharva 👋
### AI/GenAI Engineer | Python · FastAPI · LLMs · RAG · AI Agents

Final-year CSE student building production-grade AI systems from the ground up — not tutorials, not wrappers.

---

## 🛠️ Tech Stack

### AI, LLMs & Agentic Systems
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain" />
  <img src="https://img.shields.io/badge/LangGraph-FF6F00?style=for-the-badge&logo=diagram-project&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="Hugging Face" />
  <img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=fastapi&logoColor=white" alt="Groq" />
  <img src="https://img.shields.io/badge/Google_Gemini-8E75C2?style=for-the-badge&logo=googlegemini&logoColor=white" alt="Gemini" />
</p>

### Backend, Databases & Caching
<p align="left">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" alt="Celery" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector" />
  <img src="https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black" alt="DuckDB" />
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" alt="SQLAlchemy" />
</p>

### Frontend, Cloud & DevOps
<p align="left">
  <img src="https://img.shields.io/badge/React_18-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 18" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS" />
  <img src="https://img.shields.io/badge/Caddy-22B573?style=for-the-badge&logo=caddy&logoColor=white" alt="Caddy" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
</p>

---

## 🚀 Featured Projects

### 1. [RAG-Intel — Production Document Intelligence Platform](https://github.com/Atharva080324/RAG-Intel) · [Live Demo](https://rag-intel.vercel.app) · [API Docs](https://rag-intel.duckdns.org/docs)
End-to-end multi-format document intelligence platform with hybrid retrieval, agentic self-correction, and unbuffered streaming responses.

- **Hybrid Retrieval + RRF** — Merges `pgvector` dense cosine similarity with PostgreSQL full-text search (`tsvector`) via Reciprocal Rank Fusion ($k=60$).
- **Cross-Encoder Reranking** — Re-scores top-32 candidate chunks using `ms-marco-MiniLM-L6-v2` for precision.
- **Corrective RAG (LangGraph)** — State machine grades retrieval grounding and auto-rewrites queries upon low relevance (bounded retry).
- **Deterministic Table Analytics** — Markdown table extraction via `pdfplumber` with exact pandas aggregation (`sum`, `avg`, `min`, `max`) — eliminates LLM arithmetic hallucinations.
- **Streaming & Citations** — Unbuffered Server-Sent Events (SSE) direct to browser with clickable `[S1]` page-level citation inspector.
- **Full Lifecycle & Auth** — Async Celery background ingestion with live progress polling, document deletion cascades, Google OAuth 2.0, and instant Demo mode.
- **Stack** — FastAPI · PostgreSQL · pgvector · Redis · Celery · Docker Compose · Caddy · React 18 · TypeScript · Groq

---

### 2. [AI Data Analyst — Agentic Natural Language Analytics Engine](https://github.com/Atharva080324/ai-data-analyst) · [Live Demo](https://ai-data-analyst-self-nu.vercel.app)
Production-grade conversational data analysis platform converting natural language into executable SQL, analytical insights, and interactive charts over CSV and multi-sheet Excel files.

- **Multi-Step Agentic Graph** — ~20-node LangGraph pipeline with dynamic query routing, schema selection, and memory retrieval.
- **DuckDB Analytical Engine** — In-memory OLAP query execution providing sub-second aggregations over large structured datasets.
- **Self-Healing SQL Generator** — `sqlglot` syntactic validation with automated error recovery and self-correcting query retry loops (up to 3 retries).
- **Business Intelligence Generation** — Translates raw query results into executive takeaways, actionable recommendations, and dynamic data visualizations.
- **Session-Isolated State** — Strict tenant and session boundary isolation preventing cross-user query and dataset leakage.
- **Stack** — FastAPI · LangGraph · DuckDB · PostgreSQL · SQLAlchemy · Groq (LLaMA 3.1) · Pandas · sqlglot

---

### 3. [TrueScan — Autonomous AI News Journalist & Audio Synthesizer](https://github.com/Atharva080324/TrueScan)
AI-powered real-time news aggregation, verification, summarization, and audio generation system designed to combat information overload and support accessibility.

- **Live Multi-Source Scraping** — Autonomous retrieval pipeline fetching breaking global news and Reddit discussions using Bright Data MCP.
- **Agentic Workflow Control** — LangChain + LangGraph decision state machine orchestrating content verification, deduplication, and context-aware synthesis.
- **Executive Summarization** — Uses Google Gemini Flash to generate structured, fact-grounded briefings from multi-source articles.
- **Natural Voice Generation** — Integrates ElevenLabs Voice API to transform synthesized briefings into natural, lifelike audio podcasts for hands-free listening.
- **Stack** — FastAPI · Streamlit · LangGraph · LangChain · Google Gemini · ElevenLabs TTS · Bright Data MCP

---

## 🧠 What I Actually Know

- **Async FastAPI** — event loop lifecycle, dependency injection chains, unbuffered streaming responses, Celery vs BackgroundTasks
- **Production DB Layer** — async SQLAlchemy 2.0, Alembic schema migrations, Redis caching & atomic counters, pgvector HNSW similarity search
- **Auth & Security** — JWT access/refresh tokens, Google OAuth 2.0 authorization code flow, multi-tenant query-level isolation
- **Hybrid RAG & Agents** — dense + lexical search merged via RRF, cross-encoder reranking, corrective RAG with LangGraph, deterministic table analytics
- **Infrastructure & Cloud** — Docker multi-stage builds, Docker Compose orchestration, AWS EC2 deployment, Caddy automated TLS reverse proxy, Vercel frontend CI/CD
- **System Design** — CAP theorem, cache invalidation strategies, decoupled workers, RAG SaaS token & rate-limit economics

---

## 📫 Connect
[atharvadeshmukh2311@gmail.com](mailto:deshmukhatharva1123@gmail.com) · [LinkedIn](https://www.linkedin.com/in/atharva-deshmukh-151589248/)
