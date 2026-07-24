# Simple RAG Project

A simple Retrieval-Augmented Generation (RAG) project built with **Python**, **LangChain**, **Ollama**, **ChromaDB**, and **Gradio**.

This project demonstrates the basic workflow of a RAG system, including document ingestion, embedding generation, vector storage, retrieval, and answer generation using a local Large Language Model (LLM).

---

## Features

* Load documents from a local dataset
* Split documents into chunks
* Generate embeddings using Ollama
* Store embeddings in ChromaDB
* Retrieve the most relevant documents
* Generate context-aware answers with a local LLM
* Simple web interface built with Gradio

---

## Tech Stack

* Python
* LangChain
* Ollama
* ChromaDB
* Gradio

---

## Project Structure

```text
.
├── app.py
├── ingest.py
├── answer.py
├── datasets/
├── activity_db/
└── README.md
```

---

## How It Works

1. Load documents.
2. Split documents into smaller chunks.
3. Generate embeddings for each chunk.
4. Store embeddings in ChromaDB.
5. Retrieve the most relevant chunks for a user's question.
6. Send the retrieved context to the LLM.
7. Return the generated answer.

---

## Running the Project

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Download the required Ollama models:

```bash
ollama pull llama3.2
ollama pull qwen3-embedding:4b
```

Create the vector database:

```bash
python ingest.py
```

Run the application:

```bash
python app.py
```

---

## Purpose

The goal of this project is to provide a **simple and educational implementation of Retrieval-Augmented Generation (RAG)**. It is intended for learning the core concepts behind document retrieval, embeddings, vector databases, and local LLM inference.

---

## License

This project is intended for educational purposes.
