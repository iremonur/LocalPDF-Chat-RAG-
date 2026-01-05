# LocalPDF-Chat-RAG

LocalPDF-Chat is a lightweight Retrieval-Augmented Generation (RAG) chatbot that lets you upload a PDF and ask questions about its content. The app runs fully locally using a HuggingFace open-source model and Chroma / FAISS vector storage, with a Gradio web UI.

No IBM Cloud, no external API keys, no internet inference.

---

## ✨ Features

- 📄 Upload any PDF and query its content
- 🔎 Text chunking + embeddings + vector search (RAG)
- 🤖 Open-source local language model (HuggingFace)
- 🧠 LangChain-based retrieval pipeline
- 🖥️ Simple Gradio web interface
- 🔌 Runs offline after model download

---

## 🧱 Tech Stack

- Python 3.10
- LangChain (RAG pipeline)
- FAISS / Chroma vector DB
- Transformers (HuggingFace)
- SentenceTransformers embeddings
- Gradio UI

---

## 🚀 Running the Project

Clone the repository:

```bash
git clone https://github.com/<your-username>/LocalPDF-Chat.git
cd LocalPDF-Chat
