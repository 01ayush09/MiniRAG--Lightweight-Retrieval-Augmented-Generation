MiniRAG
Lightweight Retrieval-Augmented Generation Framework in Python

MiniRAG is a lightweight and modular implementation of Retrieval-Augmented Generation (RAG) designed to demonstrate the core principles of grounding large language model (LLM) responses using external knowledge sources.
The project focuses on clarity, minimalism, and extensibility, making it suitable for learning, experimentation, and small-scale deployments.

📌 Project Overview

Retrieval-Augmented Generation (RAG) enhances language models by retrieving relevant context from a knowledge base before generating responses.
MiniRAG implements a compact RAG pipeline that includes:

Document ingestion and preprocessing

Text embedding and vector indexing

Semantic retrieval of relevant chunks

Context-aware response generation

The goal of this project is to provide a clear, end-to-end RAG workflow without heavy frameworks or unnecessary abstractions.

✨ Key Features

Minimal and lightweight design – easy to understand and modify

Modular architecture – independent retrieval and generation components

Semantic search-based retrieval using vector embeddings

Configurable pipeline for experimenting with different models and parameters

Python-first implementation suitable for research and learning purposes

🏗️ System Architecture
User Query
    ↓
Query Embedding
    ↓
Vector Retrieval (Top-K Relevant Chunks)
    ↓
Context Aggregation
    ↓
Language Model Generation
    ↓
Final Answer


Each stage is implemented as a separate, reusable module to ensure clean separation of concerns.

📂 Repository Structure
MiniRAG--Lightweight-Retrieval-Augmented-Generation/
├── data/                  # Sample documents / datasets
├── src/
│   ├── loaders/           # Document loading and preprocessing
│   ├── embeddings/        # Embedding generation logic
│   ├── retrievers/        # Vector-based retrieval mechanisms
│   ├── generators/        # Response generation module
│   └── utils/             # Helper utilities
├── app.py                 # End-to-end execution script
├── config.yaml            # Configuration for models and parameters
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation

⚙️ Installation

Clone the repository and install dependencies:

git clone https://github.com/01ayush09/MiniRAG--Lightweight-Retrieval-Augmented-Generation.git
cd MiniRAG--Lightweight-Retrieval-Augmented-Generation
pip install -r requirements.txt

🚀 Usage

Run the main application:

python app.py


The script performs the following steps:

Loads and preprocesses documents

Builds vector embeddings and an index

Accepts a user query

Retrieves relevant document chunks

Generates a response grounded in retrieved context

🧠 Example Workflow (Conceptual)
# Load documents
documents = load_documents("data/")

# Create vector index
index = build_index(documents)

# Retrieve context
context = retrieve(query, index, top_k=5)

# Generate response
answer = generate(query, context)

🔧 Configuration

Key parameters can be adjusted in config.yaml, such as:

Embedding model selection

Number of retrieved chunks (Top-K)

Chunk size and overlap

Generation model parameters

This allows controlled experimentation with retrieval quality and response grounding.

📊 Use Cases

Document-based Question Answering

Knowledge-grounded chat systems

Research experiments on RAG pipelines

Educational demonstration of LLM augmentation techniques

🧪 Limitations

Designed for small to medium-scale datasets

Not optimized for production-scale distributed systems

Intended primarily for learning, research, and prototyping
