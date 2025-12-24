# 💬 Customer Support Automation – n8n Workflow

An AI-powered customer support system that automatically reads incoming Gmail messages, classifies them, searches a knowledge base using vector search, and replies with an intelligent response.

---

## 🔄 Workflow Logic

| Step | Node | Purpose |
|------|------|---------|
| 1 | Gmail Trigger | Detects new customer emails |
| 2 | Text Classifier | Identifies customer support emails |
| 3 | AI Agent | Generates support responses using knowledge base |
| 4 | Pinecone Vector Store | Retrieves policy data using embeddings |
| 5 | Gmail – Reply to Message | Sends automatic reply to customer |

---

## 🖼️ Workflow Diagram

![Customer Support Workflow](Customer-Support-Service\Customer-support-service.png)

---

## ⚙️ Setup Instructions (End-to-End)

### 1️⃣ Import Workflow

Open **n8n** → **Import Workflow** → Upload:

```
customer-support.json
```

---

### 2️⃣ Prepare Knowledge Base

1. Create a document folder with your company policies (PDF / TXT).
2. Upload policy documents to your Pinecone vector DB.
3. Use namespace:

```
policies
```

---

### 3️⃣ Configure Credentials

Create the following credentials in n8n:

| Service | Purpose |
|--------|---------|
| Gmail OAuth2 | Read & reply to customer emails |
| OpenAI API | LLM response generation |
| Pinecone API | Vector DB search |

---

### 4️⃣ Attach Credentials to Nodes

| Node | Credential |
|------|------------|
| Gmail Trigger | Gmail OAuth2 |
| OpenAI Chat Model | OpenAI API |
| Pinecone Vector Store | Pinecone API |
| Reply to a message | Gmail OAuth2 |

---

### 5️⃣ Activate Workflow

Turn the workflow toggle to **Active**.

---

### 🔟 Test Flow

Send a test email to your connected Gmail inbox with a policy-related question.

The workflow will automatically generate and reply with the correct policy answer.

