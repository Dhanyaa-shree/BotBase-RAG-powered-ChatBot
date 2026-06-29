# 🤖 BotBase — AI-Powered Support Chatbot Builder

> **Add an AI-powered support chatbot to any website in under 60 seconds — no coding required.**

BotBase is a modern **Retrieval-Augmented Generation (RAG)** platform that enables businesses to build intelligent AI support chatbots from their own documents. Simply upload your knowledge base, copy a single embed script, and provide instant AI-powered customer support on any website.

---

## 🌐 Live Demo

| Resource | Link |
|----------|------|
| 🚀 Live Application | https://rag-support-bot-wsq1.vercel.app |
| 💬 Chat Widget Demo | https://rag-support-bot-wsq1.vercel.app/demo.html |

---

# 📌 Overview

BotBase is a full-stack SaaS platform that allows businesses to create AI-powered customer support assistants without writing any code.

The platform combines **Retrieval-Augmented Generation (RAG)**, **semantic vector search**, and **Large Language Models (LLMs)** to answer customer questions accurately using company-specific documents.

Whether you're running a startup, an e-commerce website, a SaaS product, or an educational platform, BotBase helps automate customer support while maintaining high-quality, context-aware responses.

---

# ✨ Features

## 📄 Document Management

- Upload PDF, TXT, and Markdown files
- Automatic text extraction
- Intelligent document chunking
- Supports files up to 10 MB
- Multiple document support
- Easy document management

---

## 🧠 AI-Powered RAG Pipeline

- Retrieval-Augmented Generation (RAG)
- Context-aware AI responses
- Reduced hallucinations
- Intelligent knowledge retrieval
- Accurate document-based answers

---

## 🔍 Semantic Search

- Cohere Embeddings
- Vector similarity search
- Supabase pgvector
- High-speed retrieval
- Relevant context matching

---

## 💬 Embeddable Chat Widget

- One-line JavaScript integration
- Floating chatbot
- Responsive design
- Custom bot name
- Easy deployment on any website

---

## 📊 Analytics Dashboard

- Query analytics
- Usage statistics
- Resolution tracking
- AI response monitoring
- Chatbot performance insights

---

## 🔐 Secure Authentication

- Supabase Authentication
- Secure login
- Multi-tenant architecture
- Protected APIs
- Row Level Security (RLS)

---

## ⚡ Fast AI Responses

- Powered by Groq
- LLaMA 3.1 Language Model
- Low-latency inference
- High-quality AI responses

---

# 🚀 Technology Stack

## Frontend

- Next.js 14
- React
- TypeScript
- Tailwind CSS
- Supabase Authentication

---

## Backend

- Express.js
- TypeScript
- REST API
- Cohere Embeddings
- Groq API
- LLaMA 3.1

---

## Database

- Supabase PostgreSQL
- pgvector
- Row Level Security (RLS)

---

## Deployment

- Vercel
- Supabase
- GitHub

---

# ⚙️ System Architecture

```text
                     Business User
                           │
                           ▼
              Upload Documents (PDF/TXT/MD)
                           │
                           ▼
             Text Extraction & Chunking
                           │
                           ▼
          Generate Cohere Embeddings
                           │
                           ▼
        Store Embeddings in Supabase pgvector
                           │
──────────────────────────────────────────────────────
                    Website Visitor
                           │
                           ▼
              Ask Question via Chat Widget
                           │
                           ▼
            Generate Query Embedding
                           │
                           ▼
         Retrieve Similar Document Chunks
                           │
                           ▼
      Groq + LLaMA 3.1 Generates AI Response
                           │
                           ▼
          Response Displayed in Chat Widget
```

---

# 📁 Project Structure

```text
BotBase-RAG-powered-ChatBot/
│
├── backend/
│   ├── src/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── middleware/
│   │   ├── utils/
│   │   └── index.ts
│   │
│   ├── public/
│   │   └── widget.js
│   │
│   ├── package.json
│   └── vercel.json
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── public/
│   │   └── demo.html
│   ├── package.json
│   └── next.config.js
│
├── supabase/
│   └── schema.sql
│
├── .gitignore
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

Before running the project, make sure you have:

- Node.js 18+
- npm
- Supabase Account
- Cohere API Key
- Groq API Key

---

## Clone the Repository

```bash
git clone https://github.com/Dhanyaa-shree/BotBase-RAG-powered-ChatBot.git

cd BotBase-RAG-powered-ChatBot
```

---

# ⚙️ Backend Setup

```bash
cd backend

npm install

cp .env.example .env

npm run dev
```

Backend runs on:

```
http://localhost:5000
```

---

# 💻 Frontend Setup

```bash
cd frontend

npm install

cp .env.local.example .env.local

npm run dev
```

Frontend runs on:

```
http://localhost:3000
```

---

# 🗄 Configure Supabase

Open the SQL Editor inside Supabase and execute:

```text
supabase/schema.sql
```

This creates the required tables, extensions, and vector database configuration.

---

# 🔑 Environment Variables

## Backend (.env)

```env
SUPABASE_URL=

SUPABASE_SERVICE_ROLE_KEY=

COHERE_API_KEY=

GROQ_API_KEY=

FRONTEND_URL=http://localhost:3000
```

---

## Frontend (.env.local)

```env
NEXT_PUBLIC_SUPABASE_URL=

NEXT_PUBLIC_SUPABASE_ANON_KEY=

NEXT_PUBLIC_BACKEND_URL=http://localhost:5000
```

---

# 💬 Embed the Chat Widget

Add this script before the closing `</body>` tag of your website.

```html
<script
src="https://your-backend.vercel.app/widget.js"
data-token="YOUR_API_TOKEN"
data-bot-name="Support Bot"
data-backend="https://your-backend.vercel.app"
defer>
</script>
```

Once added, a floating AI chatbot will automatically appear on your website.

---

## 📸 Screenshots

A quick overview of the BotBase platform and its core features.

---

### 🔐 Login Page

Secure authentication powered by Supabase Auth.

<p align="center">
  <img width="355" alt="Login Page" src="https://github.com/user-attachments/assets/2269933d-63c0-4d95-8182-fd46e87f4e58">
</p>

---

### 🏠 Dashboard

Monitor chatbot activity, document statistics, and overall usage from a centralized dashboard.

<p align="center">
  <img width="938" alt="Dashboard" src="https://github.com/user-attachments/assets/8c27ab8e-efc5-4b14-945f-13965dacf3a2">
</p>

---

### 📄 Document Upload

Upload and manage your knowledge base with support for PDF, TXT, and Markdown files.

<p align="center">
  <img width="953" alt="Document Upload" src="https://github.com/user-attachments/assets/7c53bedf-e4c3-4e4b-8632-51bbb18988fd">
</p>

---

### 💬 AI Chat Widget

Embeddable floating chatbot that provides instant AI-powered support on any website.

<p align="center">
  <img width="309" alt="Chat Widget" src="https://github.com/user-attachments/assets/8cf0f4f6-6bd0-403b-ba13-7977b57210b0">
</p>

---

### 📈 Analytics Dashboard

Analyze user queries, AI responses, confidence scores, and chatbot performance.

<p align="center">
  <img width="945" alt="Analytics Dashboard" src="https://github.com/user-attachments/assets/8f8b4a0e-227f-42a6-b30c-b81adfc45e9b">
</p>

---

### 💻 Embed Your Bot

Generate a single embed script and integrate your AI chatbot into any website within seconds.

<p align="center">
  <img width="938" alt="Embed Bot" src="https://github.com/user-attachments/assets/0ef3891b-a911-48db-b98e-e87f116da78f">
</p>
---

# 🔄 How BotBase Works

1. Upload your business documents.
2. Documents are parsed and split into chunks.
3. Cohere generates semantic embeddings.
4. Embeddings are stored inside Supabase pgvector.
5. A visitor asks a question through the chatbot.
6. The query is converted into an embedding.
7. Relevant document chunks are retrieved.
8. Groq + LLaMA 3.1 generates an answer using retrieved context.
9. The chatbot returns an accurate, grounded response.

---

# 🎯 Use Cases

- SaaS Customer Support
- Product Documentation
- Internal Knowledge Bases
- Educational Platforms
- Company FAQs
- Startup Help Centers
- HR Documentation
- Technical Documentation
- Developer Portals

---

# 🚀 Future Improvements

- 🎙️ Voice-enabled chatbot
- 🌍 Multilingual AI support
- 📝 Conversation history
- 📊 Advanced analytics dashboard
- 👥 Team collaboration
- 📱 WhatsApp integration
- 💬 Slack integration
- 💬 Discord integration
- 🌙 Dark mode
- 🔌 Plugin ecosystem

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve BotBase:

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push to your branch

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

## **Dhanyaa Shree**

**GitHub**

https://github.com/Dhanyaa-shree

**LinkedIn**

https://www.linkedin.com/in/dhanyaa-shree/

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

Your support motivates further development and helps others discover the project.

---

<div align="center">

## 🚀 Built with ❤️ using

**Next.js • React • Express.js • Supabase • Cohere AI • Groq • pgvector • Retrieval-Augmented Generation (RAG)**

### ⭐ If you like this project, don't forget to star the repository!

</div>
