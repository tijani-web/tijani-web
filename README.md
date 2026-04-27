# Basit Tijani

Backend engineer focused on distributed systems and AI infrastructure.

I build things that handle real load — distributed consensus engines, event pipelines, and LLM gateways. The problems I find interesting are usually somewhere between concurrency, failure modes, and systems that have to be correct under pressure.

---

### Work

**[Phalanx](https://github.com/tijani-web/phalanx)** — High-availability distributed consensus engine in Go. 5-node global mesh with double-fault tolerance. Implements Raft (§5/§6/§8/§9.6), SWIM gossip discovery, and lease-based linearizable reads over BadgerDB. Deployed at the edge to handle cross-continental latency.

**[ARGUS](https://github.com/tijani-web/argus)** — Real-time behavioral analytics platform. Spring WebFlux + Kafka + TimescaleDB. 15,000 events/sec on a single VM. Reactive ingestion, Kafka Streams processing, Redis live counters, and DLQ poison pill protection.

**[Sentinel-AI](https://github.com/tijani-web/sentinel-ai)** — Multi-tenant LLM gateway. Intelligent routing across Gemini, DeepSeek, and Claude based on prompt complexity. Semantic vector cache cuts response time from seconds to milliseconds and reduces inference cost by ~90%.

**[CONTROL](https://github.com/tijani-web/control-android)** — Android sleep enforcement app. System-level overlay with a 60-second breathing timer — backed by AccessibilityService detection, a 3-tier watchdog stack, and a state machine that survives Android 14's background killing.

---

### Writing

I write about problems I've actually hit in production.

- [Taming the Global Mesh — Lessons from building a deterministic consensus engine in Go](https://basittijani.com/writing/deterministic-consensus-raft-go)
- [How one bad message can crash your entire Kafka pipeline](https://basittijani.com/writing/kafka-poison-pills-dlq)
- [The problem with blocking threads in a reactive world](https://basittijani.com/writing/reactive-blocking-paradigm)
- [How I cut AI inference costs by 90% with a semantic cache](https://basittijani.com/writing/semantic-cache-llm-costs)

---

[basittijani.com](https://basittijani.com) · [linkedin.com/in/basit-tijani](https://linkedin.com/in/basit-tijani) · tijanibwebdev@gmail.com
