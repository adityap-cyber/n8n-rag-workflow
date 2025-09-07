# 🤖 RAG Workflow with n8n, Google Gemini & Supabase

This project demonstrates a **Retrieval-Augmented Generation (RAG) pipeline** built in **n8n**.  
It integrates **Google Gemini**, **Supabase Vector DB**, and **document loaders** to deliver **context-aware AI responses**.  

---

## ⚙️ Workflow Overview
1. **Document Ingestion** – Load files from Google Drive (or other sources).  
2. **Embeddings Generation** – Google Gemini converts text into vector embeddings.  
3. **Vector Storage** – Store embeddings in Supabase Vector DB.  
4. **AI Agent** – Uses RAG to retrieve context before answering queries.  
5. **Chat Trigger** – Enables chatbot-like interactions.  

---

## 🛠️ Tech Stack
- [n8n](https://n8n.io/) – workflow orchestration  
- [Google Gemini](https://ai.google/) – embeddings + LLM  
- [Supabase](https://supabase.com/) – vector storage & retrieval  
- LangChain nodes inside n8n  

---

## 🚀 Setup Instructions

### 1️⃣ Run n8n
```bash
# Option 1: Using npm
npx n8n start

# Option 2: Using Docker
docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
