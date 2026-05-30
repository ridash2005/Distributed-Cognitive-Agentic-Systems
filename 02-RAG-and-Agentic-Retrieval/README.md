# 🔍 Module 2: RAG & Agentic Retrieval

Welcome to the second module of the **Agentic AI Masterclass**! This module covers **Grounding, Semantic Search, Pipeline Evaluation, and Agentic Retrieval**. Moving beyond basic prompts, this section shows you how to hook LLMs to enterprise knowledge stores safely, search documents semantically, evaluate retrieval quality, and build reasoning-based retrieval loops.

---

## 🗺️ Topics Covered

In this module, you will learn how to:
1. Parse and chunk complex documents (including structured PDFs and multi-page tables).
2. Build semantic indices without full database servers (Vectorless RAG).
3. Set up a high-performance, ultra-fast production search indexing system using **Typesense**.
4. Quantitatively evaluate retrieval pipelines on metrics like **faithfulness**, **answer relevance**, and **context recall**.
5. Move from basic retrieval to **Agentic RAG**, where the retriever acts as a dynamic tool that a reasoning agent can choose to loop over, query, or critique until it finds the optimal grounded answer.
6. Package your RAG pipelines into a professional, modular Python codebase (`src/` layout) ready for production deployment.

---

## 📂 Notebook & Code Directory

* **`PageIndex_Vectorless_RAG_CrashCourse (1).ipynb`**: Querying custom documentation collections with zero database dependencies.
* **`notebook/document.ipynb`**: Principles of chunking, metadata extraction, splitting, and vector representations.
* **`notebook/pdf_loader.ipynb`**: Extracting clean text, outlines, and structured tabular data from PDF files.
* **`typesense.ipynb`**: Dynamic semantic indexing and hybrid search integration using the lightweight Typesense engine.
* **`1-rag_evaluation.ipynb`**: Running automated testing on your RAG pipelines to evaluate faithfulness and correctness.
* **`agenticrag/1-agenticrag.ipynb`**: Converting naive RAG into a stateful agentic system that evaluates its own retrieval inputs and decides when to stop or fetch more context.
* **`src/`**: The core modular codebase for your enterprise RAG application:
  * `data_loader.py` - Loading and parsing document datasets.
  * `embedding.py` - Interfacing with semantic embedding models.
  * `vectorstore.py` - Managing indexes, schemas, and metadata stores.
  * `search.py` - Executing semantic and keyword hybrid queries.
* **`app.py`**: A clean API/script wrapper demonstrating how to run the entire modular RAG codebase in one line.

---

## 🚀 How to Run

1. Ensure your virtual environment is active:
   ```bash
   .venv\Scripts\Activate.ps1   # Windows
   # source .venv/bin/activate  # macOS/Linux
   ```
2. Install the specific requirements for this module:
   ```bash
   pip install -r requirements.txt
   ```
3. Typesense Server Setup:
   Typesense requires a running server instance. You can launch one locally using Docker or sign up for a free cloud sandbox at [Typesense Cloud](https://cloud.typesense.org/). Add your credentials (`TYPESENSE_API_KEY`) to the `.env` file at the root.
4. Launch your Jupyter environment and start exploring document ingestion!
   ```bash
   jupyter notebook
   ```