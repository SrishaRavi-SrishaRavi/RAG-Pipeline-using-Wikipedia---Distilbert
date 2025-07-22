# 🧠 RAG Pipeline using Wikipedia + FAISS + Hugging Face QA

This project implements a simple **Retrieval-Augmented Generation (RAG)** pipeline using:

- 🌐 Wikipedia as the knowledge base
- 🔍 FAISS for fast similarity search
- 🤖 Sentence Transformers for text embeddings
- 🧠 Hugging Face Question Answering (QA) model for answer extraction

---

## 📌 What it Does

1. Takes a **Wikipedia topic** from the user.
2. Downloads the **raw content** of that Wikipedia page.
3. Splits the content into **token-based overlapping chunks**.
4. Uses **Sentence Transformers** to convert chunks into embeddings.
5. Uses **FAISS** to retrieve the top-k most relevant chunks for a **user’s question**.
6. Uses a **Hugging Face QA model** to extract an accurate answer from the retrieved chunks.

---

## 🚀 Demo (Example Flow)

```bash
Enter a topic you want to learn about: Indian Democracy
Number of chunks: 48

Ask a question about this topic: When was the Constitution of India adopted?
Retrieved Chunks:
- The Constitution of India was adopted on 26 November 1949...
Answer: 26 November 1949
