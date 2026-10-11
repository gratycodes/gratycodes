# Gratus Antin

Senior Software Engineer at PayPal, based in Chennai, India, with about 11 years of experience. I build agentic AI systems and LLM tooling, Java/Spring Boot and Kafka backends, payments platforms, and Next.js frontends. Before PayPal I was a Principal Software Engineer at Oracle, and earlier worked at Citi, DTCC, Cognizant and Hexaware. The projects below are personal projects.

**Stack:** Java, Spring Boot, Kafka, Python, Go, TypeScript, Node.js, React, Next.js, LLM and agent tooling.

## Projects

### Agents and AI observability

- [dispute-copilot](https://github.com/gratycodes/dispute-copilot): a chargeback triage system on synthetic data, where an agent calls read-only MCP tools to recommend a decision with cited evidence and a reviewer approves or overrides it in a React console, backed by a Spring Boot service with Postgres and Kafka.
- [agent-runtime-kit](https://github.com/gratycodes/agent-runtime-kit): a minimal Python agent loop with a tool registry, optional OpenTelemetry GenAI tracing, and record/replay for regression tests.
- [otel-genai-cost](https://github.com/gratycodes/otel-genai-cost): an OpenTelemetry Collector processor that prices GenAI spans in USD, records spend by model and custom dimensions, and alerts on daily budgets.
- [genai-trace-diff](https://github.com/gratycodes/genai-trace-diff): a browser-only React app that turns GenAI traces into a chat timeline and diffs two runs ([live demo](https://gratycodes.github.io/genai-trace-diff/)).
- [kafka-ops-mcp](https://github.com/gratycodes/kafka-ops-mcp): a Java/Spring Boot MCP server for safe Kafka and DLQ inspection, with dry-run-gated replay.

### Frontend

- [chat-fault-lab](https://github.com/gratycodes/chat-fault-lab): a Next.js app that injects stream failures (stalls, dropped connections, 429s, broken frames, split UTF-8, streamed tool calls) into an OpenAI-compatible chat and shows an accessible UI handling each one, with Playwright and axe tests ([live demo](https://gratycodes.github.io/chat-fault-lab/)).

### Backend and payments

- [payment-ledger-platform](https://github.com/gratycodes/payment-ledger-platform): a Spring Boot double-entry ledger API with idempotent posting and per-currency balance checks.
- [idempotency-spring-boot-starter](https://github.com/gratycodes/idempotency-spring-boot-starter): Stripe-style `Idempotency-Key` support and webhook dedupe for Spring Boot APIs.

### Platform and DevOps

- [kube-rightsize-diff](https://github.com/gratycodes/kube-rightsize-diff): a Go PR check that compares Kubernetes CPU and memory requests with Prometheus usage and comments with cost impact.
- [schema-evolution-gate](https://github.com/gratycodes/schema-evolution-gate): a Go CLI and GitHub Action that fails PRs breaking Kafka event schemas (Avro, JSON Schema) using Schema Registry compatibility rules and sample replay, no registry needed.
- [tfplan-triage](https://github.com/gratycodes/tfplan-triage): a Go CLI and GitHub Action that reviews Terraform/OpenTofu plans in one PR comment, ranking destroyed data stores, IAM widening, new internet exposure and drift across AWS, GCP and Azure, with label-based approvals.

### ML, evals and data

- [fraud-feature-pipeline](https://github.com/gratycodes/fraud-feature-pipeline): a fraud-scoring pipeline on synthetic card data with shared streaming and offline features (Kafka, Redis, DuckDB), a LightGBM model with leakage-safe training, a FastAPI scoring API, and train/serve skew and drift checks.
- [evaldelta](https://github.com/gratycodes/evaldelta): Python stats for LLM evals (bootstrap CIs, McNemar, power, judge agreement) and a GitHub Action that posts the result on a PR.
- [rag-evaluation-lab](https://github.com/gratycodes/rag-evaluation-lab): a small Python harness that scores RAG output for recall@k, MRR, citation coverage and lexical groundedness.

[LinkedIn](https://www.linkedin.com/in/gratusantin)
