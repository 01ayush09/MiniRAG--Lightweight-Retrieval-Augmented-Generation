MiniRAG — Lightweight Retrieval-Augmented Generation

A lightweight Python implementation of Retrieval-Augmented Generation (RAG) — enabling you to build document search and QA systems with minimal setup and dependencies.

📦 MiniRAG implements core RAG components like document loading, embedding generation, retrieval, and contextual generation, optimized for simplicity and ease of use.

Inspired by research on efficient and lightweight RAG systems that use graph-based indexing and topology-enhanced retrieval for low-resource deployment.

🚀 Features

🧠 Modular RAG Pipeline – Load documents, embed, retrieve, and generate answers.

📄 Support for various data sources (e.g., text, PDFs) via custom loaders.

⚡ Lightweight and easy to extend with new retrievers or models.

🐍 Simple Python API designed for rapid prototyping.

📁 Repository Structure
MiniRAG--Lightweight-Retrieval-Augmented-Generation/
├── data/                # Sample data or datasets
├── src/                 # Source code for MiniRAG components
│   ├── embeddings/      # Embedding models
│   ├── retrievers/      # Retrieval modules
│   ├── generators/      # Generation logic
│   └── utils/           # Utilities and helpers
├── app.py               # Example application / CLI script
├── config.yaml          # Config file for settings
├── requirements.txt     # Python dependencies
└── README.md            # Project overview

💡 How It Works

MiniRAG combines retrieval and generation to answer user queries based on external knowledge:

Document Loading & Chunking – Ingest and split large texts into manageable chunks.

Embedding Generation – Convert text chunks into vector representations.

Retrieval – Use nearest neighbor search (or graph-based methods) to find relevant chunks.

Generation – Feed the query + retrieved context into a language model to generate responses.

This pipeline enables your application to ground its answers in provided documents instead of only model-internal knowledge.



Intended primarily for learning, research, and prototyping
