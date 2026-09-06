# Sunny Patel

**AI Engineer** · Agentic AI, Production RAG & LLM Evaluation

I build AI agents that survive contact with production — with guardrails, evaluation evidence, and a human in the loop when the stakes are high.

Currently at Deligence Technologies, where I own the AI stack end to end: architecture, guardrails, evals and deployment. Across 3 live client deployments I cut hallucination rate 35%, validated with RAGAS context precision and faithfulness against a versioned golden dataset.

📍 Delhi NCR, India · 📧 patel844732sunny@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/sunny-patel-346936220)

---

## 🚀 Featured Projects

### [Enterprise Knowledge Agent](REPO-LINK-HERE)
Self-correcting 6-agent RAG system on LangGraph — SafetyCheck → Router → Retriever → Rewriter → FactCheck → Synthesizer. When retrieved context isn't good enough, the graph autonomously reformulates the query and retries.

- **97.9% answer relevancy**, 75% context precision (RAGAS, on a curated golden set)
- Dual ingestion: LlamaIndex semantic chunking + LangChain parent-child splitting into Qdrant hybrid dense + BM25 collections
- LLM-based contextual compression filters irrelevant chunks before synthesis
- Full LangSmith tracing across all 6 nodes · Dockerised · GitHub Actions CI/CD · sub-2s P95

`LangGraph` `LlamaIndex` `Qdrant` `FastAPI` `React` `LangSmith` `RAGAS` `Docker`

### [MCP-Native Agent Gateway](REPO-LINK-HERE)
Gateway between LLM agents and enterprise tools: authenticated MCP servers, per-agent least-privilege scoping, tiered human approval, and a full audit trail.

- Tool risk tiers — `read` auto-executes, `write` pauses for human approval, `destructive` is blocked
- Guardrail middleware: prompt-injection detection, Presidio PII redaction, Pydantic output-schema validation
- Red-teamed against a 100-prompt suite built on the OWASP LLM Top 10
- Human-in-the-loop via LangGraph `interrupt()` · immutable audit log of every tool call

`FastMCP` `LangGraph` `FastAPI` `Postgres` `Redis` `Langfuse` `Docker`

### [RAG-Eval Studio](REPO-LINK-HERE)
Autonomous RAG benchmarking platform — a 7-node LangGraph pipeline that ingests documents, auto-generates eval Q&A via LLM synthesis, retrieves contexts and scores across 4 RAGAS dimensions.

- Side-by-side comparison of 3 chunking strategies × 2 embedding models on a live leaderboard
- Wired into GitHub Actions as a **regression gate** — a config change that drops faithfulness below threshold fails the build
- Per-node token and latency observability via LangSmith

`LangGraph` `RAGAS` `Qdrant` `Streamlit` `FastAPI` `LangSmith`

### [Biomedical RAG](REPO-LINK-HERE)
Domain-specific medical document retrieval using BioMistral and PubMedBERT embeddings over Qdrant — domain-tuned embedding selection rather than a general-purpose model.

`BioMistral` `PubMedBERT` `Qdrant` `LangChain` `Python`

### [AI Legal Consultancy ChatSupport](REPO-LINK-HERE)
Semantic retrieval over a 10,000+ document legal corpus — LlamaIndex sentence-window chunking with LLaMA 3 on Pinecone. 92% answer relevance on curated QA benchmarks; metadata-filtered re-ranking cut mean retrieval latency 45%.

`LlamaIndex` `LLaMA 3` `Pinecone` `Flask` `AWS EC2` `Docker`

---

## 🛠️ Stack

**Agents & Orchestration** — LangGraph · LangChain · LlamaIndex · CrewAI · Model Context Protocol (MCP) / FastMCP · OpenAI Agents SDK · function calling · multi-agent patterns

**RAG & Retrieval** — Agentic RAG · hybrid search (dense + BM25) · semantic / parent-child chunking · query rewriting · re-ranking · contextual compression · Qdrant · Pinecone · FAISS · Chroma · pgvector

**Evaluation & Observability** — RAGAS · LLM-as-judge · golden datasets · regression evals as CI gates · LangSmith · Langfuse · OpenTelemetry

**Safety & Governance** — prompt-injection defence · input/output guardrails · PII redaction · tool-call allow-listing · human-in-the-loop approval gates · OWASP LLM Top 10

**LLMs** — GPT-4o · Claude · Gemini · LLaMA 3.3 70B · Mistral · Groq · Azure OpenAI · LoRA/PEFT fine-tuning · Hugging Face

**Backend & Infra** — Python 3.12 · async FastAPI · Pydantic v2 · Celery · PostgreSQL · MongoDB · Redis · Docker · Kubernetes · AWS (EC2, Lambda, S3, CloudWatch) · GitHub Actions

---

## 📜 Certifications

- Claude Certified Architect – Foundation, Anthropic

---

## 📊 Stats

![](https://github-readme-stats.vercel.app/api?username=sunny84patel&theme=dark&hide_border=true&include_all_commits=true&count_private=true&show_icons=true)
![](https://github-readme-stats.vercel.app/api/top-langs/?username=sunny84patel&theme=dark&hide_border=true&include_all_commits=true&count_private=true&layout=compact&langs_count=8)

---

**Open to AI Engineer / Generative AI Engineer / Agentic AI Engineer roles.** 30-day notice · Delhi NCR or remote.
