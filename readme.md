
# 💰 Agentic Finance Assistant using Google ADK

This project demonstrates a **simple agentic AI workflow** built using the **Google Agent Development Kit (ADK)**.  
It focuses on **agent delegation**, where one agent handles user interaction and delegates specific tasks to another agent when required.

The goal of this project is to understand **how agents collaborate**, not to build a full financial system.

---

## 🚀 Project Overview

The system consists of **two agents**:

1. **Finance Assistance Agent**  
   - Acts as the main interface for the user  
   - Answers general finance-related questions  
   - Retrieves predefined personal finance details (salary, expenses, savings)

2. **Investment Plan Agent**  
   - Handles market-related queries  
   - Uses **Google Search** to fetch real-time financial data  
   - Assists in investment and savings planning

This separation keeps responsibilities clear and makes the workflow easy to extend.

---

## 🧠 Agent Workflow

```

User
↓
Finance Assistance Agent
↓ (delegation)
Investment Plan Agent (Google Search)

```

---

## 🤖 Agent Responsibilities

### 1️⃣ Finance Assistance Agent
- Responds to general finance questions
- Retrieves user finance data such as:
  - Salary
  - Monthly expenses
  - Savings capacity
- Delegates market-related queries to the Investment Plan Agent

### 2️⃣ Investment Plan Agent
- Uses Google Search for:
  - Stock prices
  - Market data
  - Financial news
  - Latest or current financial information
- Provides factual, up-to-date responses based on search results

---

## 🧩 Tools Used

| Tool | Purpose |
|----|--------|
| `get_user_personal_finance_details` | Returns predefined finance data |
| `google_search` | Fetches real-time market information |
| `AgentTool` | Enables agent-to-agent delegation |

---

## 🤖 Model Used

- **Gemini 2.5 Flash**

Gemini works particularly well with ADK because:
- It has strong tool-calling discipline
- It handles delegation and search-based tasks reliably
- It produces stable and structured outputs

---

## 📁 Project Structure

```

project_root/
│
├── agent.py
├── investment_plan_agent/
│   └── agent.py
├── requirements.txt
└── README.md

````

---

## ⚙️ Setup Instructions

### 1️⃣ Create a Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate      # Linux / Mac
venv\Scripts\activate         # Windows
````

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Run the ADK Web UI

```bash
adk web
```

Open the interface at:

```
http://127.0.0.1:8000
```

---

## 🎯 Key Learnings from This Project

* Understanding **agent delegation**
* Separating responsibilities across agents
* Combining static user data with real-time search
* Learning how ADK manages tools and agent communication

---

## 📌 Notes

* This project is intentionally simple
* Finance values are mock data for demonstration
* Designed as a learning step before building larger multi-agent systems

---


## 👤 Author
**Muthuraj M**  
AI & Machine Learning Engineer | Data Analyst  

📧 Email: maruthumuthu04@gmail.com  
🔗 GitHub: https://github.com/muthutony2110  

---

## 📄 License

This project is intended for learning and experimentation with agentic AI using Google ADK.

```
