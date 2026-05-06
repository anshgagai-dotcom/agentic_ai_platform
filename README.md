# 🚀 Agentic AI Automation Platform

## 📌 Overview
This project is a **multi-agent AI system** that autonomously plans, executes, and verifies tasks using Large Language Models (LLMs).

It simulates a real-world **AI Business Analyst**, capable of breaking down complex queries and generating structured outputs.

---

## 🧠 Architecture

The system is built using a **3-layer agentic architecture**:

- **Planner Agent**
  - Breaks user query into actionable steps

- **Executor Agent**
  - Executes each step using tools

- **Verifier Agent**
  - Validates outputs and retries if incorrect

---

## 🔥 Key Highlight
This project implements a **verification loop** to reduce hallucinations in LLM outputs.

---

## ⚙️ Tech Stack

- LangChain
- OpenAI
- FastAPI
- Streamlit
- Python

---

## 🚀 Features

- Multi-agent workflow
- Tool-based execution
- Verification mechanism (retry logic)
- API + UI integration
- Modular code structure

---

## 📂 Project Structure
agentic_ai_platform/
│
├── agents/
│ ├── planner.py
│ ├── executor.py
│ ├── verifier.py
│
├── tools/
│ └── search_tool.py
│
├── utils/
│ └── prompts.py
│
├── app/
│ └── main.py
│
├── frontend/
│ └── streamlit_app.py
│
├── requirements.txt
└── README.md


---

## ▶️ How to Run

```bash
git clone https://github.com/yourusername/agentic_ai_platform.git
cd agentic_ai_platform

python -m venv venv
venv\Scripts\activate

pip install -r requirements.txt

uvicorn app.main:app --reload
streamlit run frontend/streamlit_app.py
