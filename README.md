<!-- Paste into github.com/Rishav-R03/Rishav-R03/README.md -->
<!-- Replace every [FILL: ...] with a MEASURED number before publishing. Delete the line if you can't measure it. -->

# Rishav Raj

**Backend engineer: Go and Python, data pipelines, and the infrastructure behind LLM products.**

I build services where correctness is measurable: idempotent APIs, transactional outbox pipelines, rate limiting for LLM endpoints, and AI extraction that validates its own output. Every project below has a one-command Docker setup, load-test numbers and a documented list of known limitations.

📍 New Delhi, India · 📫 rishav042023@gmail.com · [LinkedIn](https://www.linkedin.com/in/rishav-raj-15b077249/)

**Stack:** Go · Python (FastAPI, asyncio) · PostgreSQL (pgvector) · Redis · RabbitMQ · Docker · Prometheus/Grafana · AWS (ECS, S3, SQS, Terraform) · OpenAI / Gemini APIs

---

## Featured projects

### [DocIntel](https://github.com/Rishav-R03/DocIntel): document-to-JSON extraction API
Headless, self-hostable service that turns PDFs and images into schema-validated JSON using an LLM. Async FastAPI + SQS worker, encrypted S3 staging, Alembic migrations, Terraform-defined AWS infra, contract-tested OpenAPI.
- [FILL: extraction accuracy on N labelled documents, e.g. "94% field-level accuracy on 50 invoices"]
- [FILL: p50 / p95 end-to-end latency per document and cost per document]
- [FILL: % of LLM outputs passing schema validation on first try vs after retry]

`Python` `FastAPI` `PostgreSQL` `SQS` `S3` `Terraform` `ECS` `Gemini`

### [Order → Analytics CDC Pipeline](https://github.com/Rishav-R03/food_delivery_Analytics_Platform): transactional outbox, OLTP → OLAP in Go
Orders are written transactionally, captured by a Postgres trigger into an outbox, delivered at-least-once by a worker, and loaded idempotently into a separate analytics store. A reconciliation job proves both databases agree to the paisa.
- 19,594 orders under k6 load (100 VUs): **0% errors, p95 20 ms, p99 32 ms**
- 10 concurrent requests with one `Idempotency-Key` created exactly **1** order
- Worker killed mid-load: **50/50** orders recovered, **0** reconciliation mismatches

`Go` `PostgreSQL` `LISTEN/NOTIFY` `Prometheus` `k6` `Docker`

### [Distributed Rate Limiter for LLM endpoints](https://github.com/Rishav-R03/distributed-rate-limiter)
Atomic sliding-window limiter in Redis + Lua protecting downstream model APIs from traffic spikes. Degrades gracefully if Redis is down.
- **31,000+ req/s**, sub-2 ms p99 [FILL: confirm hardware and tool used, e.g. k6 on 8-core laptop]
- Prometheus + Grafana dashboards for allow/deny rate and decision latency

`Go` `Redis` `Lua` `Prometheus` `Grafana`

<!-- Optional 4th slot: add the WAL message broker or LLM gateway ONLY if the repo is public, has a README with benchmarks, and CI passing. -->

---

## What I'm doing now
Building an LLM-powered assistant for HR appraisal workflows in production (FastAPI, OpenAI, 560+ automated tests). Previously interned on Go/QUIC network services and RabbitMQ pipelines at Hashed Tokens.

## Working on next
- Finishing DocIntel's AI extraction phase with a published accuracy/cost evaluation
- Adding integration tests and CI to the CDC pipeline
- Writing up the outbox-vs-log-based-CDC trade-offs [FILL: link when published]

## Background
B.Tech CSE, VIT Bhopal (2022–2026), CGPA 8.56.
