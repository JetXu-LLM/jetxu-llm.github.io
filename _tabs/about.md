---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
---

## Hi there! 👋

I'm **Jet Xu**, an engineer passionate about building **AI systems that understand code at scale**. My work focuses on **Repository Graph RAG architectures**, **LLM context engineering**, and **evidence-based code intelligence** — making AI agents truly comprehend software repositories through structured knowledge graphs.

I believe the future of automated development lies in **Code Graph RAG** — where AI agents reason about codebases through persistent knowledge graphs capturing classes, methods, dependencies, and call relationships. That's the core of what I'm building.

---

## 🎯 Core Research & Engineering Focus

### Repository Graph RAG Architectures
Building next-generation retrieval systems specifically for code understanding:
- **Code Knowledge Graphs** capturing structural relationships (classes, methods, imports, call graphs)
- **Hybrid retrieval pipelines** combining graph traversal, semantic search, and LLM-powered reasoning
- **Multi-source context assembly** from self repositories, public codebases, issues, and discussions
- **Production-grade graph databases** (ArangoDB) for efficient traversal and complex query patterns

### LLM Context Engineering for Automated Development
Designing intelligent context retrieval that powers AI-driven development workflows:
- **Evidence-based reasoning** grounding AI insights in actual code snippets and architectural context
- **Multi-stage retrieval** with embedding models, rerankers, and confidence scoring
- **Task-aware context selection** adapting retrieval strategies based on development task complexity
- **Repository pool caching** for real-time performance in multi-agent systems

### Privacy-Preserving Code Intelligence
Building secure architectures for enterprise code analysis:
- **Zero-knowledge storage** using cryptographic blind indexing (HMAC-SHA256)
- **Ephemeral processing** where code content never persists, only graph structures
- **Federated learning approaches** for cross-repository insights without data sharing

---

## 🚀 Featured Projects

### [LlamaPReview](https://jetxu-llm.github.io/LlamaPReview-site/) — Evidence-Based AI Code Review

A GitHub App delivering **Graph RAG-powered PR reviews** with context retrieval and severity gating for low-noise, high-impact insights.

**Core Architecture:**
- 🧠 **Context Retrieval Engine**: Finds related, unchanged code to surface ripple effects early
- 📊 **Evidence-Backed Findings**: Every high-priority issue ties to real code snippets with confidence scores
- 🎯 **Severity Gating**: Deterministic filtering reduces false positives and review fatigue
- 🔒 **Secure Knowledge Graph**: Professional tier uses ArangoDB for persistent code structure analysis

**Technical Innovations:**
- **Repository Graph RAG**: Classes, methods, dependencies, and call graphs enable deep semantic understanding
- **Zero-Knowledge Architecture**: Code content is ephemeral; only cryptographic fingerprints persist
- **Self-Adaptive Review**: Learns from your team's review patterns over time
- **Multimodal Analysis**: Inline suggestions, architectural diagrams (Mermaid), and structured summaries

**Current Adoption:**
- 🌟 **3,000+ active repositories** (32,000+ combined stars)
- 🆓 **Free for public repos** with automatic advanced analysis on complex PRs
- 🚀 **Professional tier** (launching soon) with full knowledge graph capabilities

[**Try LlamaPReview →**](https://github.com/marketplace/llamapreview) | [**Website →**](https://jetxu-llm.github.io/LlamaPReview-site/)

---

### [llama-github](https://github.com/jetxu-llm/llama-github) — Foundation for Automated AI-Driven Development

An open-source Python library for **efficient GitHub knowledge retrieval**, designed as the context retrieval module for future **automated development systems** powered by multi-agent LLMs.

**Vision: Automated AI-Driven Development**

The library serves as a foundational component in a larger architecture (see diagram above) that enables:
- **Multi-Agent Orchestration**: LLM-based agents collaborating on complex coding tasks
- **Retrieval-Augmented Development Loop**: Continuous context retrieval from self repos and public knowledge
- **Task & State Management**: Intelligent task allocation, scheduling, and state tracking
- **Development Tools Integration**: File editing, testing, version control, and deployment automation

**Current Capabilities:**
- 📚 **Dual-Mode Retrieval**: Self repositories + public GitHub resources (code, issues, discussions)
- 🎯 **LLM-Powered Query Analysis**: Intelligent search strategy generation
- 🔄 **Advanced Ranking**: Embedding similarity + reranker scores + LLM relevance scoring
- ⚡ **Production-Ready**: Async processing, repository pool caching, flexible authentication
- 🗄️ **Vector Database Integration**: Efficient storage and retrieval at scale

**Quick Start:**
```bash
pip install llama-github
```

```python
from llama_github import GithubRAG

github_rag = GithubRAG(
    github_access_token="your_token",
    openai_api_key="your_key"
)

# Retrieve context for development tasks
query = "How to implement async context managers in Python?"
context = github_rag.retrieve_context(query)
```

**Future Development:**
While currently focused on LlamaPReview development, llama-github will evolve to support the full automated development vision — enabling AI agents to autonomously accomplish complex coding tasks through intelligent context retrieval and tool orchestration.

**License:** Apache 2.0 | **Status:** Available on PyPI

[**View on GitHub →**](https://github.com/jetxu-llm/llama-github)

---

## 🛠️ Technical Expertise

### AI/ML & Code Intelligence
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/-LangChain-121212?style=flat-square)
![Hugging Face](https://img.shields.io/badge/-Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

- **Repository Graph RAG**: ArangoDB for code knowledge graphs, graph traversal algorithms
- **LLM APIs & Models**: OpenAI GPT-4o, Anthropic Claude, Google Gemini, Mistral AI
- **Embedding & Reranking**: Jina AI embeddings and rerankers, sentence-transformers
- **Code Analysis**: AST parsing, static analysis, tree-sitter, semantic understanding
- **Vector Databases**: Efficient storage and retrieval for embedding-based search

### Enterprise Architecture & Cloud-Native Systems
![Java](https://img.shields.io/badge/-Java-007396?style=flat-square&logo=java&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Cloud-Native Architecture**: Microservices, containerization, auto-scaling, high availability
- **Cloud Platforms**: Alibaba Cloud, AWS (compute, storage, serverless)
- **High-Concurrency Systems**: Distributed architectures, message queues, caching strategies
- **Domain-Driven Design**: Modular architecture, service boundaries, API design

### Search & Data Technologies
- **Semantic Search**: Multimodal search (text, image, voice), embedding-based retrieval
- **Graph Databases**: ArangoDB for complex relationship modeling and traversal
- **Databases**: MySQL, MongoDB, Redis, distributed data systems
- **Data Platforms**: Customer data platforms, real-time processing, analytics

---

## 📝 What I Write About

On this blog, you'll find deep dives into:

- **Repository Graph RAG**: Architectures for building code knowledge graphs that power AI agents
- **LLM Context Engineering**: Strategies for intelligent context retrieval in automated development
- **Code Intelligence Systems**: Building AI that reasons about software architecture, not just syntax
- **Privacy-Preserving AI**: Cryptographic techniques for secure code analysis without persistent storage
- **Production ML Systems**: Lessons learned from deploying AI tools at scale (3,000+ repos)
- **Multi-Agent Orchestration**: Designing systems where LLM-based agents collaborate on complex tasks

I also share insights from enterprise architecture, digital transformation, and the intersection of AI with real-world software engineering challenges.

---

## 🌟 Current Initiatives

### Short-Term (Q4 2025)
- 🚀 Launching **LlamaPReview Professional** with ArangoDB-powered knowledge graphs for private repos
- 📊 Publishing benchmarks: **Code Graph RAG vs. vector-only RAG** for software understanding tasks
- 📝 Writing comprehensive guides on **Repository Graph RAG architectures**

### Long-Term Vision: Automated AI-Driven Development
Building towards **fully automated development systems** (as illustrated in the architecture diagram) that combine:
- **Multi-Agent Orchestration**: LLM-based agents collaborating through intelligent task allocation
- **Repository Graph RAG**: Persistent code knowledge graphs enabling deep architectural reasoning
- **Development Tools Integration**: Seamless file editing, testing, version control, and deployment
- **Continuous Learning**: Self-adaptive systems that improve from developer feedback
- **Privacy-First Design**: Zero-knowledge architectures for enterprise adoption

The vision: AI agents that can autonomously accomplish complex coding tasks by intelligently retrieving context from self repositories and public knowledge, while maintaining human oversight through conversation management.

---

## 💡 Philosophy

> **"The best AI tools are evidence-based — they ground insights in real code structures, not hallucinations."**

I believe in building AI systems that:
- ✅ **Reason through graphs** — Code understanding requires structural knowledge, not just embeddings
- ✅ **Ground in evidence** — Every insight ties back to actual code snippets and relationships
- ✅ **Prioritize signal over noise** — Severity gating and confidence scoring reduce false positives
- ✅ **Respect privacy** — Cryptographic blind indexing, zero-knowledge storage, ephemeral processing
- ✅ **Learn continuously** — Adapt to team patterns, improve through usage

---

## 🎓 Background

With **15+ years** spanning enterprise architecture and AI/ML engineering, I bring a unique perspective to building practical AI systems:

- **AI/ML Engineering**: Hands-on development of LLM-powered applications, Graph RAG systems, and AI agents
- **Enterprise Architecture**: Designing mission-critical platforms (CRM, CDP, e-commerce) serving millions of users
- **Technical Leadership**: Leading cross-functional teams (architecture, DevOps, QA) in multinational environments
- **Open Source Contribution**: Building developer tools (llama-github, LlamaPReview) used by the global community

My experience includes architecting **cloud-native platforms** with auto-scaling and high availability, implementing **semantic search engines** with multimodal capabilities (image, voice), and designing **privacy-compliant data systems** for regulated industries.

I've also led digital transformation initiatives from 0 to 1, including:
- **China Unified Services Platform** at Kering (luxury retail's strategic business mid-platform)
- **Digital Mid-Platform** at Volvo Cars (20+ microservices, 10+ system integrations)
- **Social Network Mobile App** as founder/CEO (millions of users, ML-powered personalization)

This combination allows me to bridge cutting-edge AI research and production-ready systems that developers actually want to use.

---

## 🏆 Recognition & Achievements

- 🥇 **First Award** at National Olympiad in Informatics in Provinces (NOIP)
- ⭐ **Top Contributor** (Top 5%) at IBM for three consecutive years (2012-2014)
- 🚀 **3,000+ repositories** actively using LlamaPReview
- 📦 **Open-source maintainer** of llama-github (Apache 2.0 license)

---

## 📫 Get in Touch

I'm always interested in discussing:
- **Repository Graph RAG architectures** for code intelligence
- Challenges in building **production LLM systems** with privacy guarantees
- **Multi-agent orchestration** for automated development
- **Collaboration opportunities** on open-source AI tooling
- Feedback on **LlamaPReview** and **llama-github**

**Connect with me:**
- 💼 **LinkedIn**: [Jiantong Xu](https://www.linkedin.com/in/jiantongxu/)
- 🐙 **GitHub**: [@jetxu-llm](https://github.com/jetxu-llm)
- 📧 **Email**: jiantong.xu@foxmail.com
- 🌐 **Projects**:
  - [LlamaPReview GitHub App](https://github.com/marketplace/llamapreview)
  - [LlamaPReview Website](https://jetxu-llm.github.io/LlamaPReview-site/)
  - [llama-github Library](https://github.com/jetxu-llm/llama-github)

---

## 📚 Acknowledgments

My work builds on the shoulders of giants. Special thanks to:
- **[ArangoDB](https://www.arangodb.com/)** for the powerful multi-model database enabling complex graph queries
- **[Jina AI](https://jina.ai/)** for excellent embedding models and reranker APIs
- **[LangChain](https://www.langchain.com/)** for the foundational LLM application framework
- **The open-source community** for countless libraries, tools, and shared knowledge

---

## 🔖 Fun Facts

- 🦙 The "Llama" in my project names honors Meta's Llama models and the open-source LLM movement
- 🎓 Double bachelor's degree in **Biological Sciences & Computer Sciences** from Fudan University
- 🎯 My goal: Build AI agents that can autonomously accomplish complex coding tasks through intelligent context retrieval
- 📖 Firm believer that **code understanding requires graphs, not just embeddings**

---

**Last Updated:** October 2025

*This page is a living document. Check back for updates on Repository Graph RAG research and automated development progress!*