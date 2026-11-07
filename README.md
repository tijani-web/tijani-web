# Basit Tijani
### Senior Backend & Distributed Systems Engineer

Backend and infrastructure engineer focused on distributed systems, event-driven pipelines, and AI infrastructure. I build things that handle real load—distributed consensus engines, reactive event processors, and intelligent LLM gateways. The problems I find interesting are usually somewhere between concurrency, failure modes, and systems that have to be correct under pressure.

---

### Core Technical Expertise
* **Languages:** Go, Java 21, Python, TypeScript, SQL
* **Distributed Systems & Storage:** Raft consensus, SWIM gossip, gRPC, LSM-tree engines (BadgerDB), PostgreSQL, TimescaleDB
* **Infrastructure & Kubernetes:** Custom operators, informers/indexers, scheduler framework plugins, admission webhooks, CRDs, Helm, ArgoCD, Terraform, Docker, Linux
* **Messaging & Processing:** Kafka, Kafka Streams, Spring WebFlux, Redis

---

### Featured Production Systems

* **[Phalanx](https://github.com/tijani-web/phalanx)** — A globally distributed key-value store built in Go across 5 geographic regions, running a pure Raft consensus engine, SWIM gossip discovery (Memberlist), and lease-based linearizable reads backed by BadgerDB[cite: 1, 2, 3]. Engineered for zero data loss with $N=5, Q=3$ quorum fault tolerance[cite: 2].
* **[ARGUS](https://github.com/tijani-web/argus)** — A high-throughput, non-blocking telemetry ingestion and behavioral analytics platform built with Spring WebFlux, Kafka Streams, Redis Lua atomics, and TimescaleDB[cite: 1, 5, 6]. Capable of scaling to 8,000–15,000 events/sec on a single 4-vCPU Azure VM[cite: 1, 5].
* **[Sentinel-AI](https://github.com/tijani-web/sentinel-ai)** — A multi-tenant LLM gateway built using Java 21 virtual threads, Spring AI, and PostgreSQL[cite: 1]. Features intelligent dynamic routing across Gemini, DeepSeek, and Claude based on prompt complexity, combined with a Redis vector store semantic cache that significantly reduces latency and inference costs.
* **[Meridian](https://github.com/tijani-web/meridian)** — A Kubernetes-native GPU fleet control plane[cite: 2]. Built custom operators (shared informers, indexers, server-side apply, Lease-based HA leader election) and a scheduler framework plugin set (Filter, Score, Reserve, Permit) delivering gang scheduling, topology-aware placement, and fair-share queues with borrowing.

---

### System Design & Architecture Artifacts

* **[System Design & Production Architecture (PDF)](./Basit_Tijani_System_Architecture_Written_Artifact.pdf)** — A comprehensive deep-dive document detailing the production architecture, failure modes, data flows, 10x scale bottlenecks, and cost models for Phalanx and ARGUS.

---

### Engineering Writing

I write about problems I've actually hit in production:

- [Taming the Global Mesh — Lessons from building a deterministic consensus engine in Go](https://basittijani.com/writing/deterministic-consensus-raft-go)
- [How one bad message can crash your entire Kafka pipeline](https://basittijani.com/writing/kafka-poison-pills-dlq)
- [The problem with blocking threads in a reactive world](https://basittijani.com/writing/reactive-blocking-paradigm)
- [How I cut AI inference costs by 90% with a semantic cache](https://basittijani.com/writing/semantic-cache-llm-costs)

---

### Connect

[basittijani.com](https://basittijani.com) · [linkedin.com/in/basit-tijani](https://linkedin.com/in/basit-tijani) · [tijanibwebdev@gmail.com](mailto:tijanibwebdev@gmail.com)
