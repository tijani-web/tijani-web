# Basit Tijani
### Senior Backend & Distributed Systems Engineer

Backend and infrastructure engineer focused on distributed systems, event-driven pipelines, and AI infrastructure. I build systems where correctness under failure matters: consensus engines, reactive event processors, GPU schedulers, and LLM gateways. I audit my own work and publish the results, including what I got wrong.

[basittijani.com](https://basittijani.com) · [LinkedIn](https://linkedin.com/in/basit-tijani) · [tijanibwebdev@gmail.com](mailto:tijanibwebdev@gmail.com)

---

### Core Technical Expertise
* **Languages:** Go, Java 21, Python, TypeScript, SQL
* **Distributed Systems & Storage:** Raft consensus, SWIM gossip, gRPC, LSM-tree engines (BadgerDB), PostgreSQL, TimescaleDB
* **Infrastructure & Kubernetes:** Custom operators, informers/indexers, scheduler framework plugins, admission webhooks, CRDs, Helm, ArgoCD, Terraform, Docker, Linux
* **Messaging & Processing:** Kafka, Kafka Streams, Spring WebFlux, Redis

---

### Featured Systems

* **[Phalanx](https://github.com/tijani-web/phalanx)**: a distributed key-value store in Go, replicated across 5 regions with a pure Raft consensus engine, SWIM gossip discovery (memberlist), and BadgerDB storage. Quorum of 3 out of 5, tolerating 2 node failures.
  *Evidence:* independently audited; 8 defects found and fixed test-first; 99 of 100 randomized fault-injection runs checked linearizable (1 under analysis).

* **[ARGUS](https://github.com/tijani-web/argus)**: a non-blocking event ingestion platform built with Spring WebFlux, Kafka Streams, atomic Redis Lua rate limiting, and TimescaleDB. Accepts an event, publishes it to Kafka, and returns `202`; no database write on the hot path.
  *Evidence:* design documented; 8-15K events/s on a single 4-vCPU Azure VM is author-reported, independent audit pending.

* **[Sentinel-AI](https://github.com/tijani-web/sentinel-ai)**: a multi-tenant LLM gateway built with Java 21 virtual threads, Spring AI, and PostgreSQL. Routes dynamically across Gemini, DeepSeek, and Claude based on prompt complexity, with a Redis vector-store semantic cache to reduce latency and inference cost.

* **[Meridian](https://github.com/tijani-web/meridian)**: a Kubernetes-native GPU fleet control plane in Go. Custom operators (shared informers, indexers, server-side apply, Lease-based HA leader election) and scheduler framework plugins (Filter, Score, Reserve, Permit) for gang scheduling, topology-aware placement, and fair-share queues with borrowing, plus checkpoint-aware preemption and an inference router.
  *Evidence:* benchmarked on simulated nodes (KWOK) and an emulated inference server; a real-vs-simulated table is published in the repo.

---

### Systems Architecture & Verification Report

<a href="./docs/Basit-Tijani-Systems-Architecture-Rev2-DARK.pdf">
  <img src="./docs/assets/architecture-cover.png" alt="Cover of the Systems Architecture and Verification Report" width="240" align="right">
</a>

**Distributed Systems & Infrastructure: Phalanx, ARGUS, Meridian**
First published May 2026 · Revised November 2026 (Rev. 2.0) · 32 pages

A plain-language, diagram-rich document covering how three systems were designed, how they fail, how they were tested, and where the evidence stops. Every result is labeled **Verified**, **Author-reported**, or **Not measured**.

Inside: concept primers (Raft, linearizability, Kafka, gang scheduling), architecture diagrams, an independent audit story with commit references, a production-style postmortem, scale analysis, known limitations, a glossary, and a reading list.

* **[Read the PDF (dark)](./docs/Basit-Tijani-Systems-Architecture-Rev2-DARK.pdf)**
* [Print-friendly PDF (light)](./docs/Basit-Tijani-Systems-Architecture-Rev2-LIGHT-print.pdf)
* [Markdown version](./docs/ARCHITECTURE.md) (renders in the browser, diagrams included)

<br clear="right">

---

### Engineering Writing

Notes on problems I ran into while building these systems:

- [Taming the Global Mesh: lessons from building a deterministic consensus engine in Go](https://basittijani.com/writing/deterministic-consensus-raft-go)
- [How one bad message can crash your entire Kafka pipeline](https://basittijani.com/writing/kafka-poison-pills-dlq)
- [The problem with blocking threads in a reactive world](https://basittijani.com/writing/reactive-blocking-paradigm)
- [How I cut AI inference costs by 90% with a semantic cache](https://basittijani.com/writing/semantic-cache-llm-costs)

---

### Connect

[basittijani.com](https://basittijani.com) · [linkedin.com/in/basit-tijani](https://linkedin.com/in/basit-tijani) · [tijanibwebdev@gmail.com](mailto:tijanibwebdev@gmail.com)
