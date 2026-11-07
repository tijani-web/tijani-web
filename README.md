# Basit Tijani
### Senior Backend & Distributed Systems Engineer

Backend and infrastructure engineer specializing in high-throughput data platforms, event-driven architectures, and distributed systems. I build resilient, low-latency systems designed to handle real production load under strict concurrency and failure constraints.

---

### Core Technical Expertise
* **Languages:** Go, Java 21, Python, TypeScript, SQL
* **Kubernetes & Infrastructure:** Custom operators, informers/indexers, scheduler framework plugins, admission webhooks, CRDs, Helm, ArgoCD, Terraform, Docker, Linux
* **Distributed Systems & Storage:** Raft consensus, SWIM gossip, gRPC, LSM-tree engines (BadgerDB)
* **Messaging & Backend:** Kafka, Kafka Streams, Spring WebFlux, Redis, PostgreSQL, TimescaleDB

---

### Featured Projects

* **[Meridian](https://github.com/tijani-web/meridian)** — Kubernetes-native GPU fleet control plane[cite: 2]. Built custom operators (shared informers, indexers, server-side apply, Lease-based HA leader election) and a scheduler framework plugin set (Filter, Score, Reserve, Permit) delivering gang scheduling, topology-aware placement, and fair-share queues with borrowing[cite: 2]. Includes a high-throughput inference router with load shedding and canary rollouts[cite: 2].
* **[Phalanx](https://github.com/tijani-web/phalanx)** — A globally distributed key-value store built in Go featuring custom Raft consensus (leader election, log replication), SWIM gossip membership and failure detection, and lease-based linearizable reads backed by BadgerDB[cite: 1]. Engineered for zero data loss under concurrent regional node failures[cite: 1].
* **[ARGUS](https://github.com/tijani-web/argus)** — A non-blocking telemetry ingestion and behavioral analytics pipeline built with Spring WebFlux, Kafka, and TimescaleDB[cite: 1]. Scaled to 15,000 events per second on a single 4-vCPU virtual machine with Kafka Streams backpressure handling and dead-letter queue (DLQ) poison pill isolation[cite: 1].
* **[Sentinel-AI](https://github.com/tijani-web/sentinel-ai)** — A multi-tenant LLM gateway built using Java 21 virtual threads, Spring Boot, and Spring AI[cite: 2]. Features dynamic routing across Gemini, DeepSeek, and Claude based on prompt complexity, combined with a Redis vector store semantic cache that significantly reduces latency and inference costs[cite: 2].

---

### Engineering Writing

I write about production-tested solutions, low-level mechanics, and architectural trade-offs:

* **[Taming the Global Mesh — Lessons from building a deterministic consensus engine in Go](https://basittijani.com/writing/deterministic-consensus-raft-go)**
* **[How one bad message can crash your entire Kafka pipeline](https://basittijani.com/writing/kafka-poison-pills-dlq)**
* **[The problem with blocking threads in a reactive world](https://basittijani.com/writing/reactive-blocking-paradigm)**
* **[How I cut AI inference costs by 90% with a semantic cache](https://basittijani.com/writing/semantic-cache-llm-costs)**

---

### Connect

[basittijani.com](https://basittijani.com) · [linkedin.com/in/basit-tijani](https://linkedin.com/in/basit-tijani) · [tijanibwebdev@gmail.com](mailto:tijanibwebdev@gmail.com)
