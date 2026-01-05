# 📘 LocalPDF-Chat

> **Local, privacy-preserving PDF Question-Answering Chatbot powered by RAG & open-source LLMs**

LocalPDF-Chat allows you to upload a PDF and ask questions about its content. The application runs fully **offline** after the first model download — no API keys, no vendor lock-in, no cloud inference.

The project demonstrates how to build a practical Retrieval-Augmented Generation (RAG) pipeline using LangChain, HuggingFace models, Chroma / FAISS vector search, and a Gradio web UI.

---

## 📖 Project Explanation

LocalPDF-Chat enables document-grounded question answering by combining text retrieval and generative AI.

When a PDF is uploaded:

1) The document is parsed  
2) Text is split into small overlapping chunks  
3) The chunks are converted into embeddings  
4) Embeddings are stored in a vector database  
5) A user question is converted into an embedding  
6) The most relevant chunks are retrieved  
7) A local language model generates an answer based on those chunks

This ensures answers are:

- grounded in the original document  
- context-aware  
- private and fully local  

Typical use cases include:

- reading research papers  
- searching technical manuals  
- querying legal / financial reports  
- exploring ebooks or specifications

The project is useful in environments where:

- external cloud access is restricted
- data privacy is critical
- offline operation is required
- transparent open-source tooling is preferred

---

## 🧭 Short Description (for GitHub header)

> Local, offline PDF Question-Answering Chatbot using RAG, LangChain, HuggingFace models and Gradio. Upload a PDF and ask questions — all processing stays on your machine.

---

## ✨ Features

- 📄 Upload a PDF & query its content
- 🔎 RAG pipeline (chunking → embeddings → retrieval)
- 🧠 Open-source local LLM (no API keys)
- 🗃️ Chroma or FAISS vector storage
- 🖥️ Gradio browser-based UI
- 🔌 Fully offline after initial model download
- 🛡️ Private & secure document processing

---

## 🧱 Tech Stack

- Python 3.10
- LangChain
- HuggingFace Transformers
- SentenceTransformers
- Chroma / FAISS vector DB
- Gradio UI

---

## 📁 Project Structure

.
├── qabot.py # Main application script
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── .gitignore

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/<your-username>/LocalPDF-Chat.git
cd LocalPDF-Chat

###Create & activate virtual environment:
python3.10 -m venv rag_env
source rag_env/bin/activate

###Install dependencies:
pip install -r requirements.txt

###Run the application:
python qabot.py

###Open the UI in your browser:
http://127.0.0.1:7860
