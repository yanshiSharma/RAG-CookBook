<div align="center">

# 📚 RAG-CookBook

### A practical, hands-on collection of Retrieval-Augmented Generation patterns — from Naive to Agentic.

[![GitHub Stars](https://img.shields.io/github/stars/yanshiSharma/RAG-CookBook?style=flat-square)](https://github.com/yanshiSharma/RAG-CookBook/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/yanshiSharma/RAG-CookBook?style=flat-square)](https://github.com/yanshiSharma/RAG-CookBook/network/members)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

</div>

---

## 🧠 What is RAG-CookBook?

**RAG-CookBook** is a curated, beginner-to-advanced repository of Retrieval-Augmented Generation (RAG) implementations. Each notebook is a self-contained recipe — covering a specific RAG pattern, complete with setup, explanation, and runnable code.

Whether you're just learning what RAG is or building production-grade pipelines, this repo gives you a structured path through all major RAG paradigms.

> **Stack used across notebooks:** Supabase (vector DB) · PyMuPDF · Sentence Transformers (`BAAI/bge-small-en-v1.5`) · Groq (LLM inference) · LangChain · Python

---

## 🗂️ Repository Structure

```
RAG-CookBook/
├── 1__Naive-RAG.ipynb
├── 2__RAG-With-Memory.ipynb
├── 3__Query-Transformation-RAG.ipynb
├── 4__HyDE-RAG.ipynb
├── 5__Self-RAG.ipynb
├── 6__Corrective-RAG.ipynb
├── 7__Agentic-RAG.ipynb
├── README.md
└── CONTRIBUTING.md
```

---

## 📖 RAG Patterns at a Glance

| # | RAG Type | Notebook | Core Idea | Best Used For | Project Description |
|---|----------|----------|-----------|---------------|---------------------|
| 1 | **Naive RAG** | `1__Naive-RAG.ipynb` | Embed docs → retrieve top-K → answer | Prototyping, simple Q&A over docs | Coming Soon! |
| 2 | **RAG with Memory** | `2__RAG-With-Memory.ipynb` | Adds conversation history to context window | Coming Soon! |
| 3 | **Query Transformation RAG** | `3__Query-Transformation-RAG.ipynb` | Rewrite/expand/decompose query before retrieval | Ambiguous queries, multi-intent searches | Coming Soon! |
| 4 | **HyDE RAG** | `4__HyDE-RAG.ipynb` | Generate a hypothetical answer, embed that instead | Sparse queries, domain-specific corpora | Coming Soon! |
| 5 | **Self-RAG** | `5__Self-RAG.ipynb` | Model evaluates its own retrieval and generation | High-accuracy Q&A, fact-critical applications | Coming Soon! |
| 6 | **Corrective RAG** | `6__Corrective-RAG.ipynb` | Detect bad retrieval → correct via web search fallback | Dynamic knowledge domains, up-to-date Q&A | Coming Soon! |
| 7 | **Agentic RAG** | `7__Agentic-RAG.ipynb` | LLM decides which tools to invoke dynamically | Complex workflows, multi-source retrieval | Coming Soon! |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- A [Supabase](https://supabase.com/) account (free tier works)
- A [Groq](https://console.groq.com/) API key (free tier works)
- Google Colab or a local Jupyter environment

### Quick Start

```bash
# Clone the repo
git clone https://github.com/yanshiSharma/RAG-CookBook.git
cd RAG-CookBook

# Open any notebook in Colab or Jupyter
# Start with 1__Naive-RAG.ipynb for the basics
```

Each notebook is fully self-contained with its own install step (`!pip install ...`). Follow the steps sequentially within each notebook — they are numbered clearly.

### Environment Setup

Before running any notebook, set the following:

```python
# Groq
GROQ_API_KEY = "your_groq_api_key"

# Supabase
SUPABASE_URL = "your_supabase_project_url"
SUPABASE_KEY = "your_supabase_service_role_key"
```

> **Tip:** Use Google Colab's Secrets (🔑 icon in the sidebar) to store API keys safely instead of hardcoding them.

---

## 🛣️ Learning Path

If you're new to RAG, follow this order:

```
Naive RAG  →  RAG with Memory  →  Query Transformation  →  HyDE
                                                               ↓
                               Agentic RAG  ←  Corrective RAG  ←  Self-RAG
```

Each notebook builds conceptually on the previous ones, but they are all independently runnable.

---

## 🔮 Coming Soon

| Pattern | Status |
|---------|--------|
| Graph RAG | 🔜 Coming Soon |
| Modular RAG | 🔜 Coming Soon |
| Multi-Modal RAG (images + text) | 🔜 Coming Soon |
| RAG Evaluation Framework (RAGAS) | 🔜 Coming Soon |
| Long-Context RAG | 🔜 Coming Soon |
| Adaptive RAG | 🔜 Coming Soon |
| Speculative RAG | 🔜 Coming Soon |

---

## 🤝 Contributing

Contributions are what make this cookbook grow! Whether you want to add a new RAG pattern, fix a bug, or improve documentation — you're welcome here.

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for full guidelines.

---

## ⭐ Show Your Support

If this repo helped you, please consider giving it a **star** — it helps others discover it!

---


<div align="center">
Made by <a href="https://github.com/yanshiSharma">Yanshi Sharma</a>
</div>
