## Giorgi Giorgobiani

**Senior AI Platform Engineer** — I build the infrastructure that agent systems run on:
orchestration, retrieval, evaluation, and the cost and latency controls that decide whether a
system survives contact with production.

Nine years of production engineering, the last several on LLM and agent platforms.

---

### In production

A **multi-tenant conversation-intelligence platform** turning ~100 hours of calls a week into
structured business intelligence — nine queue-driven workers across seven queues each with its own
dead-letter queue, retrieval over 3,072-dimension embeddings in pgvector, a 24-tool
function-calling assistant, and an MCP server exposing the intelligence layer to external agents.
Tenant isolation by Postgres row-level security in a single deployment. Compute cost down ~94% by
moving off per-task serverless containers to capacity providers tuned per workload shape,
autoscaled on queue backlog per task rather than CPU.

A **10-agent NLP pipeline** on a decentralized data platform — a meta-orchestrator fanning out to
seven stateless model agents in parallel, merging through a single writer into a social graph.
Content-hash idempotency made the whole thing replayable: wipe Postgres, rebuild from source
events, get identical output. Pipelines declared as infrastructure-as-code, so a new one ships as a
stack file without recompiling any service.

An **embedded AI companion platform** — custom ESP32-S3 hardware, four memory layers across Redis,
Postgres and a graph store, and a streaming voice loop under 500ms. Every session reprocesses the
full prior history rather than reading a fixed window, so recall doesn't degrade as the window
slides.

Earlier: founding engineer at a legal-AI startup through SOC 2 Type 2, and ML platform tooling in
biotech.

---

### What's pinned

**Keeping agents accountable while they build** — the problem I keep returning to. Agents that
write code are easy; agents you can trust unattended are not.

- **[loop-kit](https://github.com/Zuzuna54/loop-kit)** — a portable autonomous build loop. Fresh
  context per iteration, builder separated from judge, and evidence-gated marking so a feature
  can't go green unless it re-proves green.
- **[sprint-harness](https://github.com/Zuzuna54/sprint-harness)** — Shape Up + SPARC with drift
  control, using inject-violation-catch-restore to verify the guardrails actually fire.
- **[inspector-hook](https://github.com/Zuzuna54/inspector-hook)** — cross-IDE visibility into what
  AI coding assistants are doing to your files, in real time.

**Agentic systems**

- **[jobsearch-automation](https://github.com/Zuzuna54/jobsearch-automation)** — a local-first
  automation OS: ingest, score, tailor, then a hard human gate before anything is sent. Next.js
  dashboard over Postgres, with an LLM harness that runs faithfulness checks against fabrication.
- **[Topic-Modelling](https://github.com/Zuzuna54/Topic-Modelling)** — real-time chat analysis into
  a social graph with relationship intelligence and LLM-driven topic modelling.

**Architecture**

- **[systems-architecture-studies](https://github.com/Zuzuna54/systems-architecture-studies)** —
  C4, sequence, and component diagrams for two production systems, written as pattern studies.
  Autoscaling on backlog-per-task, fan-out reads with a single writer, a promotion ladder that
  never demotes, content-hash idempotency.

---

### Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/CDKTF%20%2F%20Pulumi-844FBA?style=flat-square&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%20%2B%20pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)

| | |
|---|---|
| **AI & LLM** | Multi-agent orchestration · agentic workflows · agent runtimes · RAG pipelines · vector search (pgvector) · embeddings · semantic clustering · Model Context Protocol (MCP) servers · streaming STT/TTS pipelines · prompt versioning · LLM observability · cost and latency optimization · OpenAI / Anthropic / Gemini / Mistral APIs · open-weight TTS/STT |
| **Cloud & Infra** | AWS (ECS, SQS, Lambda, S3, RDS, AppSync, CloudWatch, ECR, EC2, VPC, CloudFront) · Pulumi (TypeScript) · CDKTF · Docker · Kubernetes · GitHub Actions · Serverless · GCP |
| **Data** | PostgreSQL 17 (Row Level Security, pgvector) · Redis · FalkorDB · Neo4j · DynamoDB · MongoDB · Elasticsearch · Kafka · Prisma · TypeORM |
| **Languages** | TypeScript · JavaScript · Python · C/C++ (embedded firmware) · Java · SQL · Cypher |
| **Backend & API** | Node.js · Express · FastAPI · GraphQL · AppSync · Flask · Vert.x |
| **Frontend** | React · Next.js · React Native · Redux · Tailwind · D3.js |

---

📍 New York, NY · Remote (US) &nbsp;&nbsp;·&nbsp;&nbsp; 🔎 Open to Senior AI Platform / AI Infrastructure roles

[Website](https://zuzuna54.github.io/) ·
[Résumé](https://zuzuna54.github.io/resume.pdf) ·
[LinkedIn](https://www.linkedin.com/in/giorgi-giorgobiani-282883153) ·
[Email](mailto:giorgigiorgobiani54@gmail.com)
