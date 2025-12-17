MiniRAG
Lightweight Retrieval-Augmented Generation Framework in Python

MiniRAG is a lightweight and modular implementation of Retrieval-Augmented Generation (RAG) that demonstrates how external knowledge can be integrated into language model responses. The project is designed with clarity and simplicity in mind, making it suitable for learning, experimentation, and small-scale applications.

Project Overview

Retrieval-Augmented Generation enhances language models by retrieving relevant information from a knowledge source before generating responses. MiniRAG implements an end-to-end RAG pipeline that includes document ingestion, semantic retrieval, and context-aware text generation.

The primary objective of this project is to provide a clean and understandable implementation of RAG without relying on heavy frameworks or production-level infrastructure.

Key Features

Lightweight and minimal RAG implementation

Modular pipeline with clearly separated components

Semantic vector-based document retrieval

Configurable parameters for experimentation

Easy to read and extend Python codebase

System Architecture

User Query
→ Query Embedding
→ Vector Similarity Search
→ Top-K Context Retrieval
→ Context-Augmented Generation
→ Final Response

Repository Structure

MiniRAG--Lightweight-Retrieval-Augmented-Generation/
├── data/ Sample documents and datasets
├── src/
│ ├── loaders/ Document loading and preprocessing
│ ├── embeddings/ Text embedding generation
│ ├── retrievers/ Vector-based retrieval logic
│ ├── generators/ Context-aware response generation
│ └── utils/ Utility functions
├── app.py End-to-end execution script
├── config.yaml Configuration file
├── requirements.txt Project dependencies
└── README.md Project documentation
