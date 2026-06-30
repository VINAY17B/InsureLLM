# 🛡️ InsureLLM

An AI-powered Retrieval-Augmented Generation (RAG) chatbot that answers insurance-related queries using Large Language Models (LLMs), semantic search, and vector databases. The application retrieves relevant information from a knowledge base before generating accurate, context-aware responses.

## 🚀 Features

- Retrieval-Augmented Generation (RAG)
- Semantic document search using embeddings
- Vector database for efficient similarity search
- Context-aware responses using LLMs
- Automatic document ingestion and indexing
- Interactive chatbot interface
- Evaluation pipeline for response quality
- Modular and extensible architecture

---

## 🏗️ Project Architecture

```
                +----------------------+
                |  Insurance Documents |
                +----------+-----------+
                           |
                    Document Ingestion
                           |
                    Text Chunking
                           |
                    Embedding Model
                           |
                    Vector Database
                           |
                  User Question
                           |
                  Similarity Search
                           |
                 Retrieved Context
                           |
                  Large Language Model
                           |
                  AI Generated Answer
```

---

## 🛠️ Tech Stack

### Programming Language
- Python

### LLM Frameworks
- LangChain
- LiteLLM

### Embeddings
- OpenAI Embeddings

### Vector Database
- ChromaDB

### LLM Providers
- OpenAI
- Ollama (Local Models)

### Frontend
- Streamlit

### Evaluation
- Custom evaluation scripts

---

## 📂 Project Structure

```
InsureLLM/
│
├── app.py                 # Streamlit application
├── ingest.py              # Document ingestion pipeline
├── answer.py              # Question answering pipeline
├── eval.py                # Response evaluation
├── test.py                # Testing utilities
├── requirements.txt
├── README.md
│
├── data/                  # Knowledge base documents
├── vector_db/             # Vector database
├── prompts/               # Prompt templates
├── utils/                 # Helper utilities
└── screenshots/
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/VINAY17B/InsureLLM.git
cd InsureLLM
```

Create a virtual environment

```bash
python -m venv venv
```

Activate it

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

Example:

```env
OPENAI_API_KEY=your_api_key
```

If using Ollama:

```env
OLLAMA_BASE_URL=http://localhost:11434
MODEL=llama3.2:3b
```

---

## ▶️ Running the Application

### Step 1: Ingest Documents

```bash
python ingest.py
```

### Step 2: Launch the Chatbot

```bash
streamlit run app.py
```

---

## 📊 Evaluation

Evaluate chatbot responses using

```bash
python eval.py
```

---


## 🎯 Future Improvements

- Conversation memory
- Multi-document retrieval
- Hybrid search (BM25 + Vector Search)
- Citation generation
- PDF upload from UI
- Authentication
- Docker support
- REST API deployment
---

## 👨‍💻 Author

**Vinay Bhalerao**
