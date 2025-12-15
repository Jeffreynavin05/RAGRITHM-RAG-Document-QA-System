

# RAGRITHM – RAG-Based AI Document Q&A System 📄🤖

RAGRITHM is an advanced **Retrieval-Augmented Generation (RAG)** based Artificial Intelligence system that enables intelligent question-answering over document repositories. Users can upload PDF documents and ask natural language questions to receive accurate, context-aware answers with clear source attribution.

---

## 📌 Project Overview

Traditional keyword-based search systems fail to capture semantic meaning and context in large document collections. RAGRITHM solves this problem by combining **vector embeddings, graph-based retrieval, and large language models** to provide high-quality answers from documents.

---

## 🚀 Key Features

- PDF document upload and processing  
- Token-based semantic text chunking  
- Vector similarity search for relevant context  
- Graph-based knowledge storage  
- Multi-stage retrieval with fallback mechanisms  
- Context-aware answer generation  
- Source attribution with similarity scores  
- Real-time processing feedback  

---

## 🧠 RAG Pipeline Architecture

1. **Document Ingestion**
   - PDF text extraction using PyPDF2  
   - Token-based chunking with overlap  

2. **Embedding Generation**
   - Semantic embeddings using Google Vertex AI  
   - Automatic retry and rate-limit handling  

3. **Vector Storage**
   - Neo4j graph database with vector indexing  
   - Cosine similarity search  

4. **Retrieval-Augmented Generation**
   - Primary vector search  
   - Keyword-based fallback retrieval  
   - Context construction from top-k chunks  
   - Response generation using Gemini  

---

## 🛠️ Technology Stack

### Frontend
- React  
- TypeScript  
- Vite  
- Bootstrap  

### Backend
- Python 3.10+  
- FastAPI  

### AI / ML
- Google Vertex AI  
  - Gemini 2.5 Pro  
  - text-embedding-004 / 005  

### Database
- Neo4j (Graph Database with Vector Search)

### Utilities
- PyPDF2  
- tiktoken  
- NumPy  

---

# RAGRITHM

## Setup

**Create a Virtual Env**

```bash
$ python -m venv .venv
```

**Switch to virtualenv**

- Linux / OSX

```bash
$ source .venv/bin/activate
```

- Windows

```cmd
.venv\Scripts\activate.bat
```

**Install Packages**

```bash
$ pip install -r requirements.txt
```



**Run FastAPI**


