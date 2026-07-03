### Hi, I'm Furqan 👋

I build AI-agent systems, retrieval platforms, and the developer tooling around them — mostly Python, with Django and TypeScript where the project calls for it. Below are a few projects that show that work in more depth than a repo list can.

Some of my other work lives in private client/employer repos and isn't included here for confidentiality reasons.

---

### 🔍 [Retrieval Systems Platform](https://github.com/furqan90/retrieval_systems_platform)
A general-purpose retrieval platform combining sparse (BM25) and dense (vector) search over any corpus type, with an agentic layer that autonomously benchmarks and recommends embedding models for a given dataset. Organized as a monorepo with a shared core library, an experimentation/evaluation tier (RAGAS, multi-model benchmarking, Airflow + Celery), and a minimal production-serving tier — documented with a full C4 architecture model.

**Stack:** Python · LangChain-style agent tooling · Airflow · Celery · Kafka · Kubernetes/Helm

### 🤖 [DevEnv Agent](https://github.com/furqan90/ai_mediated_platform_engineering)
An AI-mediated platform-engineering tool: given a natural-language project description, it validates a structured spec and produces a runnable scaffold — repo, CI pipeline, IdP realm/clients, Docker Compose stack, and docs — through a planner that turns the spec into a gated, multi-phase execution plan with pluggable "skills" per capability.

**Stack:** Python · JSON Schema · Spring Boot code generation · pytest

### 🏭 [Production Monitoring Platform](https://github.com/furqan90/production-monitoring-platform-web-portal)
A full-stack factory production monitoring / OEE system across three repos: [API services](https://github.com/furqan90/production-monitoring-platform-api) (auth, work orders, real-time KPI calculation), a [subscriber client](https://github.com/furqan90/production-monitoring-platform-subscriber-client-app) that ingests MQTT device telemetry from factory floor sensors, and this Angular dashboard for live production views, work order tracking, and OEE/TEEP analytics.

**Stack:** ASP.NET Core · PostgreSQL · IdentityServer · Hangfire · MQTT · Angular · Kendo UI

### 💬 [SC Routing Assistant](https://github.com/furqan90/sc-routing-assistant)
A Django app wrapping a LangGraph conversational agent (OpenAI GPT-4o) with tool use — live web search and date-aware reasoning — and per-user persistent memory via SQLite checkpointing. Containerized with Docker + Nginx and deployed through a GitHub Actions → AWS ECR/EC2 pipeline.

**Stack:** Django · LangGraph · LangChain · Docker · GitHub Actions · AWS

---

📫 Reach me at mfurqanmasood@gmail.com
