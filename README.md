# Hi, I'm Atharva 👋
### AI/GenAI Engineer | Python · FastAPI · LLMs · RAG · AI Agents

Final-year CSE student building production-grade AI systems from the ground up — not tutorials, not wrappers.

---

## 🛠️ Stack

**AI/GenAI** — LangChain · LangGraph · Agentic Workflows · Hybrid Retrieval (Vector + FTS) · Cross-Encoder Reranking · RAGAS · HuggingFace · Groq · Gemini

**Backend** — FastAPI (Async) · SQLAlchemy 2.0 · Pydantic v2 · JWT / OAuth 2.0 · Celery · Redis · Alembic

**Databases** — PostgreSQL · pgvector · Redis · ChromaDB · Pinecone · FAISS

**Frontend** — React 18 · TypeScript · Vite · TanStack Query · TailwindCSS · Vanilla CSS

**Infra & Cloud** — AWS (EC2) · Oracle Cloud · Docker & Compose · Caddy (TLS/Reverse Proxy) · GitHub Actions · Vercel · Railway

---

## 🚀 Featured Projects

### [RAG-Intel — Production Document Intelligence Platform](https://github.com/Atharva080324/RAG-Intel) · [Live Demo](https://rag-intel.vercel.app) · [API Docs](https://rag-intel.duckdns.org/docs)
End-to-end multi-format document intelligence platform with hybrid retrieval, agentic self-correction, and streaming responses.

- **Hybrid Retrieval + RRF** — Merges `pgvector` dense cosine similarity with PostgreSQL full-text search (`tsvector`) via Reciprocal Rank Fusion ($k=60$).
- **Cross-Encoder Reranking** — Re-scores top-32 candidate chunks using `ms-marco-MiniLM-L6-v2` for precision.
- **Corrective RAG (LangGraph)** — State machine grades retrieval grounding and auto-rewrites queries upon low relevance (bounded retry).
- **Deterministic Table Analytics** — Markdown table extraction via `pdfplumber` with exact pandas aggregation (`sum`, `avg`, `min`, `max`) — eliminates LLM arithmetic hallucinations.
- **Streaming & Citations** — Unbuffered Server-Sent Events (SSE) direct to browser with clickable `[S1]` page-level citation inspector.
- **Full Lifecycle & Auth** — Async Celery background ingestion with live progress polling, document deletion cascades, Google OAuth 2.0, and instant Demo mode.
- **Stack** — FastAPI · PostgreSQL · pgvector · Redis · Celery · Docker Compose · Caddy · React 18 · TypeScript · Groq

---

### [Document QnA — Production RAG SaaS](https://github.com/Atharva080324/RAG-Based-Enterprise-Knowledge-assistant)
Multi-tenant Document QnA system built production-first across 8 phases.

- Hybrid retrieval — BM25 + dense vector search merged via Reciprocal Rank Fusion
- Reranking — cross-encoder on top-50 candidates before LLM
- Corrective RAG — LangGraph state machine with self-correction + web search fallback
- Auth — JWT + refresh tokens, tenant isolation enforced at query level
- Streaming — SSE streaming LLM responses
- Eval — RAGAS endpoints (faithfulness, relevancy, hallucination detection)
- **Stack** — FastAPI · PostgreSQL · pgvector · Redis · Celery · Docker · LangGraph

---

### Other Projects
- **[TrueScan](https://github.com/Atharva080324/TrueScan)** — Document verification and scanning engine.
- **[AI Data Analyst](https://github.com/Atharva080324/ai-data-analyst)** · [Live Demo](https://ai-data-analyst-self-nu.vercel.app) — Natural language data analysis and chart generation.

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
[atharvadeshmukh2311@gmail.com](mailto:atharvadeshmukh2311@gmail.com) · [LinkedIn](https://www.linkedin.com/in/atharva-deshmukh-151589248/)
