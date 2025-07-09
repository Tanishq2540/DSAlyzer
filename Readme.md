# 🧠 DSAlyzer — AI-Powered DSA Problem Solver

**DSAlyzer** is an interactive AI-powered web application that helps users solve Data Structures and Algorithms (DSA) problems. Built with [AutoGen](https://github.com/microsoft/autogen), [Streamlit](https://streamlit.io/), and [Groq API](https://console.groq.com/), DSAlyzer uses multi-agent collaboration to plan, solve, and explain DSA queries with real-time Python code execution — all without Docker.

---

## 🚀 Features

- 🧠 **AI-Powered DSA Problem Solver** — Ask DSA questions in plain English and get code + explanation.
- 🔁 **Multi-Agent Collaboration** — Solver + Executor agents coordinate to generate and verify Python code.
- ⚡ **Groq API Support** — Ultra-fast responses powered by LLaMA 3 on Groq infrastructure.
- 🧪 **Live Code Execution** — Code is executed locally via Python subprocess and results shown in the chat.
- 💡 **Clean UI with Streamlit** — Simple and responsive interface for a seamless experience.
- 📂 **Code Persistence** — Executed code can be saved to local `.py` files by the agents.

---

## 🏗️ Tech Stack

- `Python 3.10+`
- [AutoGen (Microsoft)](https://github.com/microsoft/autogen)
- [Streamlit](https://streamlit.io/)
- [Groq API](https://console.groq.com/)
- `asyncio`, `dotenv`, `platform`, and more

---

🧰 **Project Structure**
graphql
Copy
Edit
DSAlyzer_withoutDocker/
├── agents/
│   └── code_executor_agent.py    # Agent to execute Python code locally
├── config/
│   ├── constant.py               # Model ID and constants
│   └── .env                      # Your Groq API key
├── app.py                        # Streamlit frontend
├── main.py                       # CLI entry point (optional)
├── team.py                       # Team config with RoundRobin group chat
├── requirements.txt              # Dependencies
└── README.md                     # This file

**Live Demo**
https://dsanalyzer.onrender.com/
