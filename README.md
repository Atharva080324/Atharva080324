Hi, I'm Atharva 👋
AI/GenAI Engineer | Python · FastAPI · LLMs · RAG · AI Agents

Final-year Computer Science Engineering student building production-grade AI systems from the ground up — not tutorials, not wrappers.

Currently focused on: multi-tenant RAG SaaS, LangGraph agentic workflows, hybrid retrieval systems, and production FastAPI backends.

🛠️ Tech Stack

AI / GenAI

LangChain · LangGraph · RAG Pipelines · LLM Evaluation (RAGAS)
Hybrid Retrieval (Dense + BM25 + Reranking) · Embeddings · Agentic AI
HuggingFace · Groq · OpenAI · Gemini

Backend & APIs

FastAPI (async, production-grade) · SQLAlchemy 2.0 (async) · Pydantic v2
JWT/OAuth2 Auth · Dependency Injection · Middleware · Celery
Alembic Migrations · REST API Design

Databases & Vector Stores

PostgreSQL · pgvector · Redis · ChromaDB · Pinecone · FAISS · MongoDB

Infrastructure & Deployment

Docker · docker-compose · GitHub Actions (CI/CD)
Railway · Render · Uvicorn · Gunicorn

Languages

Python · JavaScript · TypeScript · SQL

Frontend

Streamlit · React
🚀 Featured Projects
🔹 Document QnA — Production RAG SaaS

Production-grade multi-tenant Document QnA system built across 8 phases.

Ingestion pipeline — table-aware PDF parsing, recursive chunking with overlap, pgvector storage
Hybrid retrieval — BM25 sparse + dense vector search merged via Reciprocal Rank Fusion
Reranking — cross-encoder reranking on top-50 candidates before passing to LLM
Corrective RAG — LangGraph state machine with self-correction loop and web search fallback
Auth — JWT access tokens + refresh tokens, tenant isolation (every query filtered by tenant_id)
Streaming — SSE streaming LLM responses to frontend
Eval — RAGAS evaluation endpoints (faithfulness, answer relevancy, hallucination detection)
Stack — FastAPI · PostgreSQL · pgvector · Redis · Celery · Docker · LangGraph
🔹 TrueScan

Agentic AI news generation and information processing pipeline using LLM tool calling and multi-step reasoning.

🔹 AI Data Analyst

LLM-powered data analysis platform. Ask questions about your data in plain English — get analysis, charts, and insights. Live: ai-data-analyst-self-nu.vercel.app

🧠 What I Actually Know (Not Just Listed)

Most people list frameworks. Here's what I can actually reason about:

Why hybrid retrieval beats pure dense search — dense embeddings lose exact tokens (error codes, names, IDs), BM25 catches them. RRF merges both ranked lists, chunks that perform well in both rise to top.
Why pgvector over Pinecone for early-stage SaaS — eliminates separate vector DB, one Postgres instance handles structured data + vectors + full-text search. Simpler architecture, lower cost, easier backups.
Why Celery over FastAPI BackgroundTasks for document ingestion — BackgroundTasks runs in-process, no retry mechanism, lost on crash. Celery persists jobs in Redis, supports retries, runs independently.
Multi-tenant isolation — authorization filter inside the query (WHERE tenant_id = ?), not post-retrieval filtering. Structurally prevents data leakage, not just "checked after the fact."
BOLA (Broken Object Level Authorization) — the #1 API vulnerability. Every resource endpoint checks ownership, not just authentication.
📚 Currently Building
Multi-tenant RAG SaaS — 8-phase production build (LangGraph + hybrid retrieval + RAGAS eval + Docker + Railway deployment)
Advanced RAG techniques — Corrective RAG, Self-RAG, proposition chunking, contextual compression
Open source contributions — exploring FastAPI, LangChain, pgvector ecosystems
🎓 Education & Certifications
B.Tech Computer Science Engineering — CSMSS Chh. Shahu College of Engineering, Aurangabad (2027)
Lateral entry from Government Polytechnic Jalgaon (Diploma in IT)
Google Cloud Certification
Infosys Certification
Deloitte Data Analytics Job Simulation (December 2025)
📫 Connect
Email: atharvadeshmukh2311@gmail.com
LinkedIn: Atharva Deshmukh

Building in public. If something I built or wrote helped you, a star means a lot.
