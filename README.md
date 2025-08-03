# 🧠 Multi-Agent System for Product Intelligence 

This project implements an **Autonomous AI Agent System** to collect, understand, index, and retrieve **real-time patent data** using **state-of-the-art open-source LLMs**, **vector databases**, and **multi-agent frameworks**. The system is designed for **automated research**, **semantic search**, and **contextual retrieval** using **chunked RAG pipelines**, enabling advanced language planning, reasoning, and decision-making.

---

## ✅ Core Features

🔍 **Real-time Patent Data Collection** using [SerpAPI](https://serpapi.com/)
🧬 **Dense Embedding Generation Locally** using [Ollama](https://ollama.com/) and custom Docker containers
🧠 **DeepSeek LLM Integration via Ollama** for local inference and natural language understanding
🔑 **Keyword, Semantic, and Hybrid Retrieval** with [OpenSearch Vector DB](https://opensearch.org/)
🤖 **Agentic Planning & Reasoning** using [CrewAI](https://github.com/joaomdmoura/crewAI), [LangChain](https://www.langchain.com/), and DeepSeek
📦 **Chunked RAG Pipeline** to ensure efficient and relevant contextual information retrieval

---

## 🏗️ System Architecture

### 📥 Data Acquisition Layer
- Integration with **SerpAPI** to fetch real-time search results from patent databases.
- Extract relevant **textual fields** like title, abstract, inventors, and claims from JSON responses.

### 🔍 Embedding & Vectorization
- Use **Ollama** to generate dense embeddings for textual fields.
- Embeddings are generated locally using **DeepSeek** or other supported models.

### 🗃️ Vector Database Setup
- **OpenSearch** (with k-NN plugin) used as the **Vector DB**.
- Supports **cosine similarity** and **dot product** for semantic retrieval.
- Docker-based OpenSearch setup with custom **index mapping**.

### 🔄 Chunked RAG Pipeline
- Token-aware chunking using `tiktoken` for efficient ingestion.
- Embedding of document chunks and ingestion into Vector DB.
- Support for **hybrid search**: keyword + semantic.

### 🤖 Autonomous Agent Framework
- Powered by **CrewAI** for building multi-agent systems.
- Supports complex task breakdown, delegation, and execution using LLMs.
- Uses LangChain tools and memory for reasoning over patent data.

---

## 🔧 Technologies Used

| Category | Tools/Frameworks |
|---------|------------------|
| LLMs & Embeddings | Ollama, DeepSeek |
| Agent Framework | CrewAI, LangChain |
| Retrieval | OpenSearch Vector DB |
| Chunking | tiktoken |
| Data Collection | SerpAPI |
| Runtime | Docker, Python |
| Planning & Reasoning | Multi-agent architecture |

---




