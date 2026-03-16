# Basit Tijani

Backend engineer focused on distributed systems and AI infrastructure.

I build things that handle real load — event pipelines, LLM gateways, enforcement engines. The problems I find interesting are usually somewhere between concurrency, failure modes, and systems that have to be correct under pressure.

---

### Work

**[ARGUS](https://github.com/tijani-web/argus)** — Real-time behavioral analytics platform. Spring WebFlux + Kafka + TimescaleDB. 8,000–15,000 events/sec on a single VM. Reactive ingestion, Kafka Streams processing, Redis live counters, DLQ poison pill protection.

**[Sentinel-AI](https://github.com/tijani-web/sentinel-ai)** — Multi-tenant LLM gateway. Intelligent routing across Gemini, DeepSeek, and Claude based on prompt complexity. Semantic vector cache cuts response time from seconds to milliseconds and reduces inference cost by ~90%. Per-token billing engine with atomic PostgreSQL decrements.

**[CONTROL](https://github.com/tijani-web/control)** — Android sleep enforcement app. System-level overlay that cannot be dismissed — 60-second breathing timer backed by AccessibilityService detection, a 3-tier watchdog stack, and a state machine that survives Android 14's background killing. Supabase auth + Stripe billing.

**[MeshGate](https://github.com/tijani-web/meshgate)** — Microservices platform. Spring Cloud Gateway, Netflix Eureka, RabbitMQ event-driven onboarding, idempotent consumers via the Outbox pattern. Six independent services, one docker compose up.

---

### Writing

I write about problems I've actually hit in production.

- [How one bad message can crash your entire Kafka pipeline](https://basittijani.com/writing/kafka-poison-pills-dlq)
- [The problem with blocking threads in a reactive world](https://basittijani.com/writing/reactive-blocking-paradigm)
- [How I cut AI inference costs by 90% with a semantic cache](https://basittijani.com/writing/semantic-cache-llm-costs)
- [Why your microservice will process the same message twice](https://basittijani.com/writing/idempotency-distributed-systems)
- [Why I stopped polling and started listening on Android](https://basittijani.com/writing/polling-vs-listening-android)

---

[basittijani.com](https://basittijani.com) · [linkedin.com/in/basit-tijani](https://linkedin.com/in/basit-tijani) · tijanibwebdev@gmail.com
