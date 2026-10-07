<div align="center">

# AYUSH PRASAD

### AI Engineer · Generative AI · Inference Engineering

**MSc Data Science @ University of Milano-Bicocca · Milan, Italy 🇮🇹**

I build LLM systems that can be **evaluated, tested, monitored and deployed**, not just demoed.

<br>

<a href="https://www.linkedin.com/in/ayush-prasad-ds/">
  <img src="https://img.shields.io/badge/LinkedIn-Profile-292929?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="https://ayushprasad.dev/">
  <img src="https://img.shields.io/badge/Portfolio-Website-292929?style=flat-square&logo=google-chrome&logoColor=white" alt="Portfolio">
</a>
<a href="mailto:ayush@ayushprasad.dev">
  <img src="https://img.shields.io/badge/Email-ayush@ayushprasad.dev-292929?style=flat-square&logo=gmail&logoColor=white" alt="Email">
</a>

<br><br>

**Open to AI / ML Engineer roles in Europe**

</div>

---

## 🚀 Featured Projects

| Project | What it is | Highlights |
|---|---|---|
| [**LedgerLens**](https://github.com/Ayush-Prasad4/ledgerlens) | Agentic RAG over SEC 10-K filings | Every number verified against its source quote · sealed test splits · 200+ tests |
| [**LNexusAi**](https://github.com/Ayush-Prasad4/nexusai) | Multi-agent platform for async AI workflows | Redis Streams + workers · idempotency, retries, dead-letter queue · 120+ tests |
| [**InferX**](https://github.com/Ayush-Prasad4/inferx) | LLM / Transformer inference optimization | ONNX Runtime ~71% lower latency · KV-cache ~4.5× throughput |

---

### [LedgerLens](https://github.com/Ayush-Prasad4/ledgerlens)

**Agentic RAG assistant for SEC 10-K filings, built evaluation-first**

Answers questions about company filings with citations, and calculates figures only from numbers it has verified.

* **Hybrid retrieval** (dense + BM25, rank fusion) with automatic ticker and fiscal-year filtering
* **LangGraph agent** that routes each question to lookup or calculation. For calculations, an LLM extracts figures, **code verifies each number against the exact filing quote**, and a safe calculator computes the result
* **Evaluation-first:** hand-written golden sets with sealed test splits. Evaluation caught a real bug (a bracketed loss losing its minus sign), which was fixed and covered by tests
* **Honest reporting:** failed experiments (a reranker that gave no net gain) are documented, not hidden
* FastAPI service, Docker, GitHub Actions CI, 200+ automated tests. An OWASP-style red-team harness is in progress

`Python` · `LangGraph` · `RAG` · `Qdrant` · `FastAPI` · `Docker` · `GitHub Actions`

---

### [LNexusAi](https://github.com/Ayush-Prasad4/nexusai)

**Multi-agent intelligence and decision platform for reliable asynchronous AI workflows**

Turns a question into a verified, critiqued analysis, running as background jobs that survive crashes and retries.

* **Multi-agent pipeline (LangGraph):** research, verification, conflict detection, analysis, critique and synthesis, with durable checkpoints in PostgreSQL
* **Distributed execution:** FastAPI API, Redis Streams queue, dedicated workers
* **Reliability:** atomic idempotency, retries with backoff, dead-letter handling, stale-job recovery, failure-safe state transitions
* **Security and operations:** JWT auth with RBAC, rate limiting, request tracing, Prometheus/Grafana monitoring, Docker deployment, CI testing
* **Validation:** 120+ automated tests and a 50-user infrastructure baseline: 9,065 requests, 0% failures, 151.56 req/s, 8 ms P95 latency

`Python` · `LangGraph` · `FastAPI` · `Redis Streams` · `PostgreSQL` · `Docker` · `Prometheus` · `Grafana`

---

### [InferX](https://github.com/Ayush-Prasad4/inferx)

**AI inference and model optimization platform**

Benchmarks and speeds up Transformer and LLM workloads, then serves them through a monitored API.

* ONNX Runtime reduced representative Transformer latency by **~71%** vs PyTorch Eager
* INT8 brought average ONNX latency down to **1.531 ms**
* FP16 improved measured LLM generation throughput by **~49%**
* KV-cache optimization improved measured LLM throughput by **~4.5×**
* Dynamic batching scheduler reached **~893 req/s** in the tested workload
* FastAPI inference API with monitoring and load testing, containerized with Docker

`PyTorch` · `Transformers` · `ONNX Runtime` · `INT8 / FP16 / BF16` · `FastAPI` · `Docker` · `AWS`

---

## 🧠 What I Work On

| Generative AI | AI Systems |
|---|---|
| LLM applications | Inference optimization and quantization |
| Retrieval-Augmented Generation | Batching, concurrency, benchmarking |
| AI agents and agentic workflows (LangChain, LangGraph) | Async job systems, APIs, monitoring |
| LLM evaluation | Load testing, CI/CD, containerized deployment |

---

## 🛠️ Technical Stack

**Languages:** `Python` `SQL` `Java`

**Generative AI:** `LangChain` `LangGraph` `RAG` `AI Agents` `LLM Evaluation`

**ML / Inference:** `PyTorch` `Hugging Face Transformers` `ONNX Runtime` `Scikit-learn` `TensorFlow` `vLLM`

**Backend & Data:** `FastAPI` `PostgreSQL` `Redis` `Qdrant` `Pandas` `NumPy`

**DevOps & Observability:** `Docker` `GitHub Actions` `Pytest` `Prometheus` `Grafana` `Locust` `AWS` `Kubernetes` `Git`

---

## 🔬 How I Work

Define the problem, build the simplest thing that could work, **measure it honestly**, and fix what the numbers show. I care about the layer around the model: evaluation, testing, reliability, monitoring and deployment.

`Problem → Data → Model / LLM → Retrieval / Inference → Evaluation → API → Monitoring → Deployment`

---

## 🎓 Education

**MSc Data Science**, University of Milano-Bicocca · Milan, Italy
**B.Tech Computer Science & Engineering**, Siksha 'O' Anusandhan · Bhubaneswar, India

---

## 🤝 Let's Connect

I'm looking for **AI Engineering, Generative AI and ML Engineering** roles in Europe. If your team ships LLM features and cares about reliability, reach out: **[LinkedIn](https://www.linkedin.com/in/ayush-prasad-ds/)** · **[Email](mailto:ayush@ayushprasad.dev)** · **[Portfolio](https://ayushprasad.dev/)**
