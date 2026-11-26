# Enterprise Operations SOP Copilot

> Hybrid Retrieval-Augmented Generation (RAG) system with Server-Sent Events (SSE) token streaming, semantic Redis caching, and token-cost telemetry for operational SOPs.

## 🏗️ Planned Architecture
`Next.js UI` → `FastAPI Async Gateway` → `Redis Semantic Cache` → `Hybrid Search (PostgreSQL pgvector + BM25)` → `LLM Streaming Response`

## 🛠️ Tech Stack
- **Backend:** Python, FastAPI, Pydantic, LlamaIndex
- **Storage & Caching:** PostgreSQL (`pgvector`), Redis
- **Frontend & Infra:** Next.js, Tailwind CSS, Docker, AWS (EC2 / S3)

## 📂 Repository Structure
- `backend/` — FastAPI routes, RAG retrieval pipeline, and cost telemetry
- `frontend/` — Next.js streaming chat interface with clickable citations
- `docs/` — Architecture diagrams and latency benchmarks
