# 🚀 Groq RAG Chatbot 

An AI-powered document analysis chatbot built with **Gradio** and **Groq LLMs**, featuring side-by-side Retrieval-Augmented Generation (RAG) and non-RAG chat, a modern UI, and support for PDF, Word, CSV, JSON, and text files. Upload documents and compare Groq LLM answers with and without RAG context—no setup beyond your Groq API key!

---

## 🌐 Technology Stack

### 🧠 Backend

| Layer           | Technology / Library                          | Purpose                                      |
|-----------------|------------------------------------------------|----------------------------------------------|
| **Python 3.8+** | Core language                                 | Main application logic                       |
| **LangChain**   | `langchain.vectorstores`, `embeddings`, `text_splitter` | Document processing, vector DB, embeddings   |
| **Chroma**      | In-memory vector store                        | Stores and retrieves document embeddings     |
| **HuggingFace Transformers** | `sentence-transformers/all-MiniLM-L6-v2` | Text embeddings for similarity search        |
| **Groq API**    | REST endpoint with OpenAI-compatible schema   | Fast inference using Groq-hosted LLMs        |
| **PyPDF2**      | PDF parser (optional)                         | Extract text from PDF files                  |
| **python-docx** | Word file parser (optional)                   | Extract text from DOCX documents             |
| **CSV / JSON**  | Built-in Python modules                       | Read and parse structured data               |

### 🎨 Frontend

| Layer         | Technology         | Purpose                                 |
|---------------|--------------------|------------------------------------------|
| **Gradio**     | UI framework       | Build web interface in Python            |
| **Custom CSS** | Styling            | Modern layout, colors, responsiveness    |
| **Gradio Blocks API** | UI layout  | Organize inputs, file upload, chat UI    |
| **Responsive Design** | CSS media queries | Mobile-friendly layout               |

---

## ✅ Supported Groq LLM Models

| Model Name                                  | Type            | Description                          |
|---------------------------------------------|------------------|--------------------------------------|
| `llama-3.1-8b-instant`                      | Meta LLaMA 3     | Lightweight, fast inference          |
| `llama-3.1-70b-versatile`                  | Meta LLaMA 3     | Larger context, more capable         |
| `llama-3.3-70b-versatile`                  | Meta LLaMA 3.3   | Updated with better performance      |
| `mixtral-8x7b-32768`                       | Mistral (MoE)    | Long context, mixture-of-experts     |
| `gemma2-9b-it`                             | Google Gemma     | Instruction-tuned model              |
| `llama3-groq-70b-8192-tool-use-preview`    | Meta + tools     | Advanced capabilities (tool use)     |
| `llama3-groq-8b-8192-tool-use-preview`     | Meta + tools     | Smaller preview model                |

---

## 🔍 Features

- 📂 Upload and parse `.pdf`, `.docx`, `.txt`, `.csv`, `.json`
- 🧠 Ask questions using context-aware RAG retrieval
- 📊 Real-time document preview and status updates
- 🪄 Supports Groq's fastest inference LLMs via simple API key
- 🖼 Clean, responsive modern UI (dark mode compatible)
- 🔐 Secure: no data stored or sent to external servers

---

## 🛠 Installation

### 1. Install Python Dependencies

```bash
pip install -r requirements.txt
