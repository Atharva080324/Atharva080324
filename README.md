# Hi, I'm Atharva 👋
### AI/GenAI Engineer | Python · FastAPI · LLMs · RAG · AI Agents

Final-year CSE student building production-grade AI systems from the ground up — not tutorials, not wrappers.

---

## 🛠️ Stack

**AI/GenAI** — LangChain · LangGraph · RAG · Hybrid Retrieval · Reranking · RAGAS · HuggingFace · Groq · Gemini

**Backend** — FastAPI · SQLAlchemy 2.0 (async) · Pydantic v2 · JWT/OAuth2 · Celery · Alembic

**Databases** — PostgreSQL · pgvector · Redis · ChromaDB · Pinecone · FAISS

**Infra** — Docker · docker-compose · GitHub Actions · Railway · Render

---

## 🚀 Projects

### [Document QnA — Production RAG SaaS](https://github.com/Atharva080324/RAG-Based-Enterprise-Knowledge-assistant)
Multi-tenant Document QnA system built production-first across 8 phases.

- Hybrid retrieval — BM25 + dense vector search merged via Reciprocal Rank Fusion
- Reranking — cross-encoder on top-50 candidates before LLM
- Corrective RAG — LangGraph state machine with self-correction + web search fallback
- Auth — JWT + refresh tokens, tenant isolation enforced at query level
- Streaming — SSE streaming LLM responses
- Eval — RAGAS endpoints (faithfulness, relevancy, hallucination detection)
- **Stack** — FastAPI · PostgreSQL · pgvector · Redis · Celery · Docker · LangGraph

### [TrueScan](https://github.com/Atharva080324/TrueScan) · [AI Data Analyst](https://github.com/Atharva080324/ai-data-analyst) · [Live Demo](https://ai-data-analyst-self-nu.vercel.app)

---

## 🧠 What I Actually Know

Most people list frameworks. Here's what I can reason about:

- **Why hybrid retrieval beats pure dense** — dense embeddings lose exact tokens (error codes, IDs, names). BM25 catches them. RRF merges both ranked lists so chunks that score well in both rise to top.
- **Why pgvector over Pinecone for early-stage SaaS** — one Postgres instance handles structured data + vectors + full-text search. Simpler architecture, lower cost, easier backups.
- **Why Celery over BackgroundTasks for ingestion** — BackgroundTasks runs in-process, no retries, lost on crash. Celery persists jobs in Redis, retries independently.
- **Multi-tenant isolation** — authorization filter inside the query (`WHERE tenant_id = ?`), not post-retrieval. Structurally prevents leakage.
- **BOLA** — the #1 API vulnerability. Every endpoint checks resource ownership, not just authentication.

---

## 📫 Connect
[atharvadeshmukh2311@gmail.com](mailto:atharvadeshmukh2311@gmail.com) · [LinkedIn](https://www.linkedin.com/in/atharva-deshmukh-151589248/)
