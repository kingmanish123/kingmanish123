# Manish Goyal

**CTO at Fonix Technologies — building AI-powered products end to end.**

I work across FastAPI backends, multi-agent LLM systems, and Next.js frontends. I lead three engineering teams and stay hands-on daily. The repositories here are what I build outside of work to go deeper on applied LLM engineering — RAG that is actually evaluated, agent systems that are actually orchestrated, and pipelines that run in production rather than in a demo.

📍 Jaipur, India · Open to remote roles

---

## Selected projects

### 🐛 [silentbug](https://github.com/kingmanish123/silentbug) — the bugs linters can't see
Finds code that is valid Python, passes review, and then fails quietly in production. An `except` that returns success so nothing ever retries. A permission check that passes when its cache is down. A deterministic AST pass flags candidates, then one isolated LLM call per candidate decides whether it is a real defect or intentional. Six detectors, each taken from a bug I actually hit. Scored against a labelled corpus: **precision 0.78, recall 1.00** — published, because most tools in this space publish neither.

`Python` · `AST` · `Anthropic` · `pytest` · `GitHub Actions`

### 🔍 [documind](https://github.com/kingmanish123/documind) — production-minded RAG engine
Hybrid retrieval (BM25 + dense + reciprocal rank fusion), grounded citations, LLM guardrails, and an evaluation harness measuring hit@k and faithfulness. Provider-agnostic, and runs fully offline with zero configuration.

`Python` · `FastAPI` · `RAG` · `Anthropic / OpenAI`

### 🧠 [cto-brief-analyzer](https://github.com/kingmanish123/cto-brief-analyzer) — multi-agent planning suite
Turns raw client conversations and a BRD into a complete engineering planning suite — user flows, tech docs, timelines, sprint plans, risk assessments. 12+ specialized agents routed across three LLM providers, with human approval gates between stages and live cost telemetry.

`Python` · `FastAPI` · `Next.js` · `Multi-agent orchestration`

### 🛠️ [localsmith](https://github.com/kingmanish123/localsmith) — local-first agentic coding assistant
A VS Code extension: streaming chat, an autonomous multi-file agent, inline edits and tab completion, all running on your own Ollama models. Nothing leaves the machine by default. The interesting part is the safety model — `write_file` refuses to blank or drastically shrink a file, every write is reviewed before it touches disk, the agent loop is bounded by a hard step cap, and MCP servers and workspace hooks each require explicit approval before anything is spawned.

`TypeScript` · `VS Code API` · `Ollama` · `Tool calling` · `MCP`

### 🎬 [ai-story-video-factory](https://github.com/kingmanish123/ai-story-video-factory) — story to finished video
An end-to-end pipeline that takes a story idea to an upload-ready YouTube video: trending-topic research, scriptwriting, character sheets for visual consistency, image generation, voice synthesis, thumbnails, assembly, and upload. Around 15 specialized agents behind a single orchestrator.

`Python` · `FastAPI` · `Multi-agent` · `TTS / image generation`

### 🤖 [jarvis](https://github.com/kingmanish123/jarvis) — autonomous macOS assistant
A local, single-owner agent that actually operates the machine: opens apps, reads and writes files, drives the UI, runs shell commands, and watches system health. A multi-agent orchestrator on a local Ollama model does the planning, and every action passes a safety gate that classifies it by reversibility before it runs.

`Python` · `FastAPI` · `Ollama` · `Tool calling`

### 📈 [stock_prediction](https://github.com/kingmanish123/stock_prediction) — applied-LLM reasoning pipeline
Reads the overnight Indian-market news firehose, extracts themes with Gemini, reasons over candidates with Claude, and emits a ranked Nifty-100 watchlist with the full chain of reasoning attached to every pick. An educational research project — not financial advice.

`Python` · `Gemini` · `Claude` · `NLP`

---

## Stack

| | |
|---|---|
| **AI / LLM** | Multi-agent orchestration, RAG, prompt engineering, tool calling, streaming, structured output, evaluation |
| **Backend** | Python, FastAPI, SQLAlchemy, Alembic, PostgreSQL, MySQL, Redis, Celery, WebSockets |
| **Frontend** | TypeScript, Next.js, React, React Native, Tailwind CSS |
| **Infra** | Docker, AWS (S3, SES, Cognito), Nginx, CI/CD, JWT / OAuth, RBAC |

---

## At work

At Fonix I architect and ship AI SaaS end to end — a 40+ agent AI design-generation platform in private beta, a multi-tenant AI training platform serving 150+ users, and a Playwright-based engine that converts live websites into editable Figma designs. I led a full security rebuild with zero incidents since migration.

---

📫 **goyalmanish3333@gmail.com** · [LinkedIn](https://linkedin.com/in/manish-goyal-3911b6194)
