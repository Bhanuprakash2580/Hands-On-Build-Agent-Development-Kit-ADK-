# 🚀 Agent Development Kit (ADK) Project  
**Multi-Agent AI System using Gemini 2.5 Flash on Vertex AI**

---

## 📌 Overview

This project demonstrates building and running **AI agents** using the **Google Cloud Agent Development Kit (ADK)** with **Gemini 2.5 Flash** on Vertex AI.  

It includes:

- 🔎 Google Search-powered agent (RAG-based)  
- 🧠 Python agent with structured output  
- 🔁 Multi-agent system for fact-checking and correction  

---

## 📸 Screenshots & Demo

---

### 🏗️ Project Structure (VS Code)

Shows organized project folders and modular agent design.

![Project Structure](assets/project-structure.png)

---

### 🖥️ ADK Web UI Dashboard

Interactive interface to run and monitor agents.

![Web UI](assets/web-ui.png)

---

### 🔎 Google Search Agent (Real-Time RAG)

Demonstrates tool usage with live data retrieval and suggestions.

![Search Agent](assets/search-agent.png)

---

### 📊 Execution Trace View

Displays internal execution flow and debugging insights.

![Trace](assets/trace.png)

---

### 💻 CLI Chat Interface

Run agents directly from terminal for quick interaction.

![CLI](assets/cli.png)

---

### 🐍 Python Agent Execution Output

Programmatic execution with structured JSON output.

![Python Output](assets/python-output.png)

---

### 🔁 Multi-Agent System (LLM Auditor)

Fact-checking system using multiple agents:

- `critic_agent` → detects errors  
- `reviser_agent` → corrects output  

![Multi Agent](assets/multi-agent.png)

---

### 🔄 Agent Workflow / Graph Visualization

Visual representation of agent interaction and execution flow.

![Agent Graph](assets/agent-graph.png)

---

## 🏗️ Project Structure
adk_project/
├── my_google_search_agent/
├── app_agent/
├── llm_auditor/
└── requirements.txt


---

## ⚙️ Prerequisites

- Python 3.9+  
- Google Cloud account  
- Vertex AI enabled  

---

## 🔧 Setup Instructions

### 1️⃣ Clone Repo

```bash
git clone <your-repo-url>
cd adk_project

pip install --upgrade pip
pip install google-adk -r requirements.txt

export GOOGLE_GENAI_USE_VERTEXAI=TRUE
export GOOGLE_CLOUD_PROJECT=<your-project-id>
export GOOGLE_CLOUD_LOCATION=global
export MODEL=gemini-2.5-flash

adk web
Open: http://127.0.0.1:8000

adk run my_google_search_agent

python3 app_agent/agent.py

```

🤖 Agents
Agent	Description
Search Agent	Real-time Google Search (RAG)
App Agent	Structured Python output
LLM Auditor	Multi-agent fact-checking


🚀 Key Highlights

✅ Multi-agent architecture

✅ Tool integration (Google Search)

✅ Structured outputs (Pydantic)

✅ Debugging via execution trace

✅ Runs via UI, CLI, and Python

🏁 Conclusion

This project showcases:

Building scalable AI systems

Multi-agent collaboration

Real-time data integration

Production-style workflows


👨‍💻 Author

SURAM BHANU PRAKASH
GitHub: https://github.com/Hands-On-Build-](https://github.com/Bhanuprakash2580/Hands-On-Build-Agent-Development-Kit-ADK-


---

# 🔥 Important (Do This Before Upload)
screenshots

project-structure.png
<img width="2542" height="1345" alt="Screenshot 2026-03-18 155928" src="https://github.com/user-attachments/assets/54b0c2fc-1573-4f05-901e-21c166a746bf" />
web-ui.png
<img width="2559" height="1348" alt="Screenshot 2026-03-18 160014" src="https://github.com/user-attachments/assets/e8b382fd-98eb-495a-bc9b-2165bc41a024" />
cli-search-agent.png
<img width="2559" height="1356" alt="Screenshot 2026-03-18 160247" src="https://github.com/user-attachments/assets/ab088d7a-2383-4252-87f1-f5b577431710" />
python-agent-code.png
<img width="2559" height="1212" alt="Screenshot 2026-03-18 160430" src="https://github.com/user-attachments/assets/d94f9822-d79f-4705-9f56-3ebd32d8b31e" />
python-output.png
<img width="2559" height="1349" alt="Screenshot 2026-03-18 160502" src="https://github.com/user-attachments/assets/24d24744-2397-4592-9e20-2dd24357d14c" />
multi-agent-output.png
<img width="2559" height="1354" alt="Screenshot 2026-03-18 160614" src="https://github.com/user-attachments/assets/82847800-cb61-419f-83d2-a244ab7a43b5" />
agent-graph.png
<img width="850" height="1340" alt="Screenshot 2026-03-18 160731" src="https://github.com/user-attachments/assets/83d49668-4482-4025-803e-5b262fd70d4b" />
execution-trace.png
<img width="847" height="1365" alt="Screenshot 2026-03-18 160749" src="https://github.com/user-attachments/assets/835e0df8-c18b-4873-a0b7-d6e8e7d1740d" />
request-response.png
<img width="842" height="1354" alt="Screenshot 2026-03-18 160759" src="https://github.com/user-attachments/assets/5e5ef9ac-ca56-4a50-a2f8-98a076c46a63" />
