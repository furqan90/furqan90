### Hi, I'm Furqan 👋

I build full-stack systems and the AI-agent tooling around them — from retrieval and observability infrastructure for LLM agents to industrial production monitoring platforms, across Python, .NET, and TypeScript depending on what the project calls for. Below are five projects that show that work in more depth than a repo list can.

Some of my other work lives in private client/employer repos and isn't included here for confidentiality reasons.

---

### 🔍 [Retrieval Systems Platform](https://github.com/furqan90/retrieval_systems_platform)
A general-purpose retrieval platform combining sparse (BM25) and dense (vector) search over any corpus type, with an agentic layer that autonomously benchmarks and recommends embedding models for a given dataset. Organized as a monorepo with a shared core library, an experimentation/evaluation tier (RAGAS, multi-model benchmarking, Airflow + Celery), and a minimal production-serving tier — documented with a full C4 architecture model.

**Stack:** Python · LangChain-style agent tooling · Airflow · Celery · Kafka · Kubernetes/Helm

### 📡 [Agentic Observability Platform](https://github.com/furqan90/agentic-observability-platform)
Observability infrastructure purpose-built for AI agent workloads: agents anywhere (Kubernetes, a chat bot, a client VM) phone home over OpenTelemetry to a collector that fans out to LangFuse (trace/eval/cost analytics) and Prometheus + Grafana (RED metrics correlated against the infrastructure agents run on). Ships as a one-command local Docker Compose stack with a thin SDK facade so tracing backends can be swapped without touching agent code.

**Stack:** OpenTelemetry · LangFuse · Prometheus · Grafana · Docker Compose · Python SDK

### 🏭 [Production Monitoring Platform](https://github.com/furqan90/production-monitoring-platform-web-portal)
A full-stack factory production monitoring / OEE system across three repos: [API services](https://github.com/furqan90/production-monitoring-platform-api) (auth, work orders, real-time KPI calculation), a [subscriber client](https://github.com/furqan90/production-monitoring-platform-subscriber-client-app) that ingests MQTT device telemetry from factory floor sensors, and this Angular dashboard for live production views, work order tracking, and OEE/TEEP analytics.

**Stack:** ASP.NET Core · PostgreSQL · IdentityServer · Hangfire · MQTT · Angular · Kendo UI

### 🤖 [DevEnv Agent](https://github.com/furqan90/ai_mediated_platform_engineering)
An AI-mediated platform-engineering tool: given a natural-language project description, it validates a structured spec and produces a runnable scaffold — repo, CI pipeline, IdP realm/clients, Docker Compose stack, and docs — through a planner that turns the spec into a gated, multi-phase execution plan with pluggable "skills" per capability.

**Stack:** Python · JSON Schema · Spring Boot code generation · pytest

### 💬 [SC Routing Assistant](https://github.com/furqan90/sc-routing-assistant)
A Django app wrapping a LangGraph conversational agent (OpenAI GPT-4o) with tool use — live web search and date-aware reasoning — and per-user persistent memory via SQLite checkpointing. Containerized with Docker + Nginx and deployed through a GitHub Actions → AWS ECR/EC2 pipeline.

**Stack:** Django · LangGraph · LangChain · Docker · GitHub Actions · AWS

---

📫 Reach me at mfurqanmasood@gmail.com
