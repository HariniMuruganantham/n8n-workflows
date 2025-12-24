# ⚙️ n8n Automation Portfolio

A curated collection of **production-ready workflow automations** built using **n8n**, covering AI agents, business operations, and RAG pipelines.

This repository demonstrates real-world automation patterns using LLMs, vector databases, and cloud integrations.

---

## 📂 Repository Structure

```
.
├── AI-News-digest/
├── Customer-Support/
├── Email-Workflow/
├── Invoice-Workflow/
├── RAG-&-Vector-DB/
└── README.md
```

---

## 🧠 Featured Workflows

| Folder | Description |
|-------|-------------|
| **AI-News-digest** | Daily AI news aggregator using Perplexity + OpenAI with deduplication |
| **Customer-Support** | AI-powered customer support system with Gmail + vector search |
| **Email-Workflow** | Chat-driven AI email assistant using OpenAI + Gmail |
| **Invoice-Workflow** | Invoice extraction, database logging, and billing notification automation |
| **RAG-&-Vector-DB** | Retrieval-Augmented Generation system for answering questions from private documents |

---

## 🚀 How to Use Any Workflow

1. Open your **n8n** instance  
2. Click **Import Workflow**  
3. Upload the `.json` file from the desired folder  
4. Configure required credentials  
5. Activate the workflow  

Each folder contains a detailed `README.md` with setup instructions.

---

## 🛡️ Security Best Practices

- No API keys or credentials are committed  
- All workflows are **credential-agnostic**  
- Environment variables are used for sensitive values  

---

## 🧰 Technologies Used

- n8n
- OpenAI / LLM Agents
- Perplexity AI
- Pinecone Vector Database
- Google Sheets API
- Gmail API
- Google Drive API

---

## 👩‍💻 Author

**Harini Muruganantham**  
DevOps | Cloud Automation