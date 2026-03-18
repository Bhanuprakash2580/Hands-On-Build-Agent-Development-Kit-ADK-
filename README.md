# 🤖 Hands-On: Agent Development Kit (ADK)
### Multi-Agent AI System · Gemini 2.5 Flash · Vertex AI · Google Cloud

<p align="center">
  <img src="https://img.shields.io/badge/Google%20Cloud-ADK-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Gemini-2.5%20Flash-8E44AD?style=for-the-badge&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/Vertex%20AI-Enabled-34A853?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

---

## 📌 Overview

This project demonstrates building and running **production-ready AI agents** using the **Google Cloud Agent Development Kit (ADK)** powered by **Gemini 2.5 Flash** on Vertex AI.

ADK is a modular framework that lets you compose specialized agents into hierarchies, equip them with tools, and orchestrate workflows using both predictable pipelines and dynamic LLM-driven routing.

> ✅ Completed as part of **Google Cloud GENAI104** — *Get Started with Agent Development Kit (ADK)*

---

## 🏗️ Project Structure

```
adk_project/
├── my_google_search_agent/       # Real-time RAG agent with Google Search
│   ├── __init__.py
│   └── agent.py
│
├── app_agent/                    # Programmatic agent with structured output
│   ├── __init__.py
│   └── agent.py
│
├── llm_auditor/                  # Multi-agent fact-checking system
│   ├── __init__.py
│   ├── agent.py
│   └── sub_agents/
│       ├── critic_agent/         # Automated fact-checker
│       └── reviser_agent/        # Corrects inaccurate responses
│
└── requirements.txt
```

---

## 🤖 Agents at a Glance

| Agent | Type | Description |
|-------|------|-------------|
| `my_google_search_agent` | LLM + Tool | Real-time Google Search (RAG-based) |
| `app_agent` | LLM + Schema | Structured JSON output via Pydantic |
| `llm_auditor` | Multi-Agent | Fact-checking & correction pipeline |

---

## ✨ Key Features

- 🔎 **Real-Time RAG** — Google Search tool integration for grounded, up-to-date responses
- 🧠 **Structured Outputs** — Pydantic schemas enforce typed, predictable JSON responses
- 🔁 **Multi-Agent Orchestration** — `SequentialAgent` pipelines for automated critic → reviser workflows
- 🖥️ **Three Execution Modes** — Browser UI, Python script, and CLI chat interface
- 🔍 **Execution Tracing** — Step-by-step debugging of tool calls and agent interactions
- ☁️ **Vertex AI Auth** — Seamless authentication without API keys

---

## 📸 Screenshots

### 🏗️ Project Structure (VS Code)
> Organized project folders with modular agent design

![Project Structure](assets/project-structure.png)

---

### 🖥️ ADK Web UI Dashboard
> Interactive interface to run, monitor, and inspect agents

![Web UI](assets/web-ui.png)

---

### 🔎 Google Search Agent — Real-Time RAG
> Tool usage with live data retrieval and search suggestions

![Search Agent](assets/search-agent.png)

---

### 📊 Execution Trace View
> Internal execution flow for debugging latency and tool calls

![Trace](assets/execution-trace.png)

---

### 💻 CLI Chat Interface
> Quick agent interaction directly from the terminal

![CLI](assets/cli.png)

---

### 🐍 Python Agent — Structured Output
> Programmatic execution returning typed JSON via Pydantic schema

![Python Output](assets/python-output.png)

---

### 🔁 Multi-Agent System — LLM Auditor
> `critic_agent` detects errors · `reviser_agent` corrects output

![Multi Agent](assets/multi-agent-output.png)

---

### 🔄 Agent Workflow Graph
> Visual representation of agent interactions and execution flow

![Agent Graph](assets/agent-graph.png)

---

## ⚙️ Prerequisites

- Python 3.9+
- Google Cloud account with **Vertex AI API enabled**
- `gcloud` CLI authenticated

---

## 🔧 Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Bhanuprakash2580/Hands-On-Build-Agent-Development-Kit-ADK-
cd adk_project
```

### 2. Install Dependencies

```bash
pip install --upgrade pip
pip install google-adk -r requirements.txt
```

### 3. Configure Environment Variables

```bash
export GOOGLE_GENAI_USE_VERTEXAI=TRUE
export GOOGLE_CLOUD_PROJECT=<your-project-id>
export GOOGLE_CLOUD_LOCATION=global
export MODEL=gemini-2.5-flash
```

Or create a `.env` file inside each agent's directory:

```env
GOOGLE_GENAI_USE_VERTEXAI=TRUE
GOOGLE_CLOUD_PROJECT=<your-project-id>
GOOGLE_CLOUD_LOCATION=global
MODEL=gemini-2.5-flash
```

---

## 🚀 Running the Agents

### 🖥️ Browser UI (Recommended for testing & debugging)

```bash
adk web
```
Open: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

### 💻 CLI Chat Interface

```bash
adk run my_google_search_agent
```

---

### 🐍 Python Script (Programmatic execution)

```bash
python3 app_agent/agent.py
```

---

## 🔑 Core ADK Concepts

| Concept | Description |
|---------|-------------|
| **Agent** | LLM-powered building block that reasons, plans, and uses tools |
| **Tools** | Extend agents beyond text — APIs, search, code execution |
| **Session** | Manages conversation history and working memory |
| **Runner** | Orchestrates execution flow and agent interactions |
| **Callbacks** | Custom hooks for logging, validation, or behavior modification |
| **Artifacts** | Binary data (files, images, PDFs) managed per session |

---

## 🧪 Example Interactions

**Google Search Agent:**
```
User: What are some new movies released in India in the past month?
Agent: [Uses Google Search → returns grounded, real-time results]
```

**LLM Auditor (Multi-Agent):**
```
User: Earth is further away from the Sun than Mars.
critic_agent: [Fact-checks using Google Search — FALSE]
reviser_agent: Earth is closer to the Sun than Mars.
```

---

## 🏆 Skills Demonstrated

- ✅ Multi-agent architecture design
- ✅ Tool integration (Google Search / RAG)
- ✅ Structured outputs with Pydantic
- ✅ Sequential workflow orchestration
- ✅ Execution trace debugging
- ✅ Vertex AI authentication & deployment patterns
- ✅ Three execution modes: UI · CLI · Python

---

## 📜 Lab Reference

**Course:** Google Cloud GENAI104  
**Lab:** Get Started with Agent Development Kit (ADK)  
**Duration:** 1.5 hours · 7 Credits  

---

## 👨‍💻 Author

**SURAM BHANU PRAKASH**  
🔗 [GitHub](https://github.com/Bhanuprakash2580/Hands-On-Build-Agent-Development-Kit-ADK-)  
💼 [LinkedIn](https://www.linkedin.com/in/your-linkedin-handle)

---

<p align="center">
  <i>Built with 🔥 using Google Cloud ADK · Gemini 2.5 Flash · Vertex AI</i>
</p>
