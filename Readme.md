# 🧠 DSAlyzer — AI-Powered DSA Problem Solver

**DSAlyzer** is an interactive AI-powered web application that helps users solve Data Structures and Algorithms (DSA) problems. Built with [AutoGen](https://github.com/microsoft/autogen), [Streamlit](https://streamlit.io/), and [Groq API](https://console.groq.com/), DSAlyzer uses multi-agent collaboration to plan, solve, and explain DSA queries with real-time Python code execution — all without Docker.

---

## 🚀 Features

- 🧠 **AI-Powered DSA Problem Solver** -- Ask DSA questions in plain English and get code + explanation.
- 🔁 **Multi-Agent Collaboration** -- Solver + Executor agents coordinate to generate and verify Python code.
- ⚡ **Groq API Support** -- Ultra-fast responses powered by LLaMA 3 on Groq infrastructure.
- 🧪 **Live Code Execution**-- Code is executed locally via Python subprocess and results shown in the chat.
- 💡 **Clean UI with Streamlit** -- Simple and responsive interface for a seamless experience.
- 📂 **Code Persistence** -- Executed code can be saved to local `.py` files by the agents.
- 🐳 **Docker Support** -- To isolate code enviornment

---

## 🏗️ Tech Stack

- `Python 3.10+`
- [AutoGen (Microsoft)](https://github.com/microsoft/autogen)
- [Streamlit](https://streamlit.io/)
- [Groq API](https://console.groq.com/)
- `asyncio`, `dotenv`, `platform`, and more

---

🧰 **Project Structure**
```
DSAlyzer_withoutDocker/
│
├── .env                          # 🔐 Environment variables (Groq API key)
├── .gitignore                   # 🚫 Git ignored files
├── app.py                       # 🖥️ Streamlit frontend
├── main.py                      # 🛠️ CLI entry point (optional)
├── requirements.txt             # 📦 Python dependencies
│
├── agents/                      # 🤖 AI Agent definitions
│   ├── code_executor_agent.py   # Executes code using LocalCommandLineExecutor
│   ├── problem_solver.py        # Problem-solving agent logic
│
├── config/                      # ⚙️ Configuration settings
│   ├── constant.py              # Model constants and metadata
│   ├── settings.py              # Model Definition
│   ├── docker_utils.py          # Docker helpers 
│   ├── docker_executor.py       # Docker code executor
│
└── team.py                      # 👥 RoundRobinGroupChat team config
---
[**Live Demo**](https://dsanalyzer.onrender.com/)
[**Video Demo**](https://drive.google.com/file/d/1D0-xudIazWKbCx5BJy76s0m47XPiUenp/view?usp=sharing)

