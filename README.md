<p align="center">
  <img src="./assets/profile-banner.svg" alt="Ramesh Mandamanedi — backend, distributed systems and AI infrastructure engineering, illustrated as a search coordinator and three shards" width="100%" />
</p>

<h2 align="center">Ramesh Mandamanedi</h2>
<p align="center">
  <strong>Computer Science master's graduate | Backend & distributed systems | AI engineering & reliability</strong><br />
  I build measurable systems: event-driven services, search infrastructure, and AI tools with verification and human control.<br />
  <strong>Open to full-time Software Engineer, Backend Engineer, and AI/Infrastructure Engineer roles.</strong>
</p>

<p align="center">
  <a href="https://distributed-search-portfolio-demo.onrender.com/"><img alt="Search engine live demo" src="https://img.shields.io/badge/DEMO-Distributed_Search-81e6c3?style=for-the-badge&labelColor=14243a" /></a>
  &nbsp;
  <a href="https://distributed-search-portfolio-demo-rvv6.onrender.com/"><img alt="Developer documentation search live demo" src="https://img.shields.io/badge/DEMO-Developer_Docs_Search-98bfff?style=for-the-badge&labelColor=14243a" /></a>
</p>

<p align="center">
  <a href="https://github.com/Ramesh-codex/ramesh-codex.github.io">Portfolio source</a> ·
  <a href="https://www.linkedin.com/in/ramesh-mandamanedi-180878239/">LinkedIn</a> ·
  <a href="https://github.com/Ramesh-codex?tab=repositories">All repositories</a>
</p>

---

## Selected engineering projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Ramesh-codex/fleetops">01 · FleetOps</a></h3>
      <p><strong>Event-driven backend + human-approved AI decisions</strong></p>
      <p>School-bus GPS simulation using Kafka, PostgreSQL/PostGIS, FastAPI, and an AI-assisted breakdown recovery workflow. The model proposes a replacement; deterministic checks and a dispatcher control the actual assignment.</p>
      <p><strong>Evidence:</strong> 18 crash-injection runs between database and Kafka commits produced <strong>0 duplicate or missing parent alerts</strong> in the documented tests. Synthetic data only.</p>
      <p><a href="https://github.com/Ramesh-codex/fleetops">Code and findings ↗</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Ramesh-codex/agent-bugfixer">02 · Agent Bugfixer</a></h3>
      <p><strong>Evaluation and safety for AI coding agents</strong></p>
      <p>LangGraph Researcher → Coder → Reviewer workflow, a 15-bug adversarial test zoo, offline scoring against pristine tests, network-disabled Docker runs, and human approval before any draft PR.</p>
      <p><strong>Evidence:</strong> Reviewer v2 fixed <strong>40/45 attempts</strong>; all <strong>40 approvals matched the scorer</strong>, with 5 failed attempts escalated. It did <em>not</em> outperform the single agent's fix rate.</p>
      <p><a href="https://github.com/Ramesh-codex/agent-bugfixer">Code, evaluation and limits ↗</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Ramesh-codex/distributed-search-engine">03 · Distributed Search Engine</a></h3>
      <p><strong>Search and distributed-systems fundamentals built from scratch</strong></p>
      <p>Custom inverted index and BM25 ranking, consistent-hash partitioning, three search shards, a FastAPI coordinator, scatter–gather and circuit breakers.</p>
      <p><strong>Evidence:</strong> <strong>1.53 ms p50</strong> local single-node search latency at 100K documents; measured consistent-hash maximum deviation fell from <strong>35.6% to 0.8%</strong> as virtual nodes increased.</p>
      <p><a href="https://distributed-search-portfolio-demo.onrender.com/">Search demo ↗</a> · <a href="https://distributed-search-portfolio-demo-rvv6.onrender.com/">Docs search app ↗</a> · <a href="https://github.com/Ramesh-codex/distributed-search-engine">Code ↗</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Ramesh-codex/modelforge">04 · ModelForge AI</a></h3>
      <p><strong>LLM gateway and failure-aware request handling</strong></p>
      <p>One streaming interface for OpenAI-, Anthropic-, and Gemini-style providers, with usage/cost estimates, timeouts, bounded retries, fallback, rate limits and classification of potential double-billing risk.</p>
      <p><strong>Status:</strong> v0.2 (Phases 1–2). Mock providers and offline tests are implemented; live real-provider calls have <strong>not</strong> been verified. Context budgeting and dashboard are future work.</p>
      <p><a href="https://github.com/Ramesh-codex/modelforge">Code and roadmap ↗</a></p>
    </td>
  </tr>
</table>

**More work worth exploring**

- **[Stock Sentiment Pipeline](https://github.com/Ramesh-codex/stock-sentiment-pipeline)** — Redis Streams → FinBERT → FastAPI, with Prometheus/Grafana observability. CPU-only dependency selection reduced the documented Docker image from **11.7 GB to 1.6 GB**.
- **[Infrastructure Automation for AI Workloads](https://github.com/Ramesh-codex/infra-automation-ai-workloads)** — Redis-backed scheduler, workers and operational metrics. Concurrency limits and retry backoff reduced **simulated** task failures by about **52%** in measured local windows.
- **[Engineering portfolio](https://github.com/Ramesh-codex/ramesh-codex.github.io)** — Responsive static portfolio with Studio, Terminal and Editorial views, project summaries and a résumé.

## How I approach engineering

I try to make system behavior **measurable and explainable**, not just demo-ready. My repositories document failure injections, regressions, latency distributions, observability bugs, and cases where an approach **didn't** improve the result.

For AI-powered workflows, my emphasis is on **scoped tools, deterministic validation, isolated execution, and human approval** for consequential actions. For backend services, it is on **correctness under failures, event processing, query performance and practical observability**.

## Tools and technologies

| Area | Technologies used in these projects |
|---|---|
| **Backend & data** | Python, FastAPI, REST APIs, PostgreSQL, PostGIS, Redis, Kafka |
| **Search & AI** | BM25, inverted indexes, LangGraph, FinBERT, streaming LLM adapters |
| **Infrastructure** | Docker, Docker Compose, nginx, Render, GitHub Actions |
| **Testing & observability** | pytest, fault injection, benchmarks, Prometheus, Grafana |

## Connect

If you're hiring for backend engineering, distributed systems, AI engineering or infrastructure roles, I'd be glad to discuss the designs, tradeoffs and test evidence behind these projects.

**[LinkedIn](https://www.linkedin.com/in/ramesh-mandamanedi-180878239/)** · **[Portfolio repository](https://github.com/Ramesh-codex/ramesh-codex.github.io)** · **[GitHub projects](https://github.com/Ramesh-codex?tab=repositories)**

<sub>**Measurement scope:** Search p50 is from the 100K-document local benchmark, not the public demo. The hosted search demo's three shard processes share one free Render instance; they are not a multi-machine deployment. FleetOps uses synthetic data, the infrastructure-failure experiment is simulated, and ModelForge's real-provider adapters have not been live-verified. Demo links may cold-start on free hosting.</sub>
