<p align="center">
  <img src="./assets/profile-banner.svg" alt="Hi, I'm Ramesh — Backend, Distributed Systems, and AI Infrastructure Engineering. A coordinator fans out to three search shards." width="100%" />
</p>

<p align="center">
  <a href="https://distributed-search-portfolio-demo.onrender.com/"><img alt="Open distributed search demo" src="https://img.shields.io/badge/Live-DISTRIBUTED_SEARCH-81e6c3?style=for-the-badge&labelColor=14243a" /></a>
  &nbsp;
  <a href="https://distributed-search-portfolio-demo-rvv6.onrender.com/"><img alt="Open developer documentation search" src="https://img.shields.io/badge/Live-DEV_DOCS_SEARCH-98bfff?style=for-the-badge&labelColor=14243a" /></a>
</p>

<p align="center">
  <strong>One hand-built search engine. Two public, working applications.</strong><br />
  Building dependable backends, retrieval infrastructure, and practical AI foundations.
</p>

---

## 🚀 Featured projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>01 · Distributed Search Engine</h3>
      <p><strong>The search infrastructure.</strong> Custom inverted index and BM25 ranking, with a FastAPI coordinator distributing queries across three HTTP shard processes.</p>
      <p>🔍 Ranked results &nbsp;·&nbsp; 🧩 Scatter–gather &nbsp;·&nbsp; 🛡️ Circuit breakers</p>
      <p><a href="https://distributed-search-portfolio-demo.onrender.com/"><strong>↗ Live demo</strong></a> &nbsp;·&nbsp; <a href="https://github.com/Ramesh-codex/distributed-search-engine/tree/deployment-demo">Source code</a> &nbsp;·&nbsp; <a href="https://distributed-search-portfolio-demo.onrender.com/docs">API docs</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>02 · Developer Documentation Search</h3>
      <p><strong>A real application on top of that engine.</strong> Search <strong>188 indexed excerpts</strong> from 20 official FastAPI, HTTPX, and Docker documentation pages.</p>
      <p>📚 Source filters &nbsp;·&nbsp; 🔗 Original documentation links &nbsp;·&nbsp; ⚡ BM25 results</p>
      <p><a href="https://distributed-search-portfolio-demo-rvv6.onrender.com/"><strong>↗ Live app</strong></a> &nbsp;·&nbsp; <a href="https://github.com/Ramesh-codex/distributed-search-engine/tree/developer-docs-search">Source code</a> &nbsp;·&nbsp; <a href="https://distributed-search-portfolio-demo-rvv6.onrender.com/docs">API docs</a></p>
    </td>
  </tr>
</table>

> **Try them:** Search `circuit breaker` in the engine demo, or `dependency injection` in DevDocs Search. Both run publicly over HTTPS. Free hosting may need a cold start after inactivity.

## ⚙️ Under the hood

- **Retrieval:** Hand-written inverted index and BM25 scoring rather than a managed search engine.
- **Distribution:** Consistent-hash document partitioning, parallel HTTP scatter–gather, and top-K result merging.
- **Resilience:** Circuit breakers, timeouts, and explicit degraded/partial-result reporting.
- **Delivery:** Reproducible Docker builds, prebuilt indexes, GitHub Actions integration tests, and Render deployments.

<details>
<summary><strong>▸ View the search architecture</strong></summary>
<br />

```mermaid
flowchart TD
    U[Browser or API client] --> C[FastAPI coordinator]
    C -->|Parallel HTTP| S1[Shard 01]
    C -->|Parallel HTTP| S2[Shard 02]
    C -->|Parallel HTTP| S3[Shard 03]
    S1 -->|Ranked hits| C
    S2 -->|Ranked hits| C
    S3 -->|Ranked hits| C
    C --> R[Merge top-K BM25 results]
    R --> U
```

</details>

## 🧰 Technologies I use

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-253E5C?style=flat-square&logo=python&logoColor=white" />
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-253E5C?style=flat-square&logo=fastapi&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-253E5C?style=flat-square&logo=docker&logoColor=white" />
  <img alt="nginx" src="https://img.shields.io/badge/nginx-253E5C?style=flat-square&logo=nginx&logoColor=white" />
  <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-253E5C?style=flat-square&logo=githubactions&logoColor=white" />
  <img alt="REST APIs" src="https://img.shields.io/badge/REST_APIs-253E5C?style=flat-square" />
  <img alt="BM25 retrieval" src="https://img.shields.io/badge/BM25_Search-253E5C?style=flat-square" />
  <img alt="Render" src="https://img.shields.io/badge/Render-253E5C?style=flat-square&logo=render&logoColor=white" />
</p>

## ✅ Tested and deployed

Both applications have passed GitHub Actions Docker and HTTP integration checks. The documentation search application also passed a **public HTTPS test** covering real FastAPI, HTTPX, and Docker searches across all three shards.

**[View public API verification ↗](https://github.com/Ramesh-codex/distributed-search-engine/actions/runs/41043841430)** &nbsp;·&nbsp; **[Read implementation notes ↗](https://github.com/Ramesh-codex/distributed-search-engine/tree/developer-docs-search/docs_app)**

<sub>**Engineering note:** The hosted applications run three independent HTTP shard *processes* within one free Render instance—not on three separate machines. Their small demo datasets and hosting conditions are different from the original engine's larger benchmark corpus.</sub>

---

<p align="center"><strong>Interested in backend engineering, distributed systems, search infrastructure, and AI platform roles.</strong><br />
<a href="https://github.com/Ramesh-codex/distributed-search-engine">Explore my engineering work ↗</a></p>
