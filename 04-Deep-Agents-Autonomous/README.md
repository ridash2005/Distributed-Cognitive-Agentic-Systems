# 🤖 Module 4: Deep Autonomous Agents

Welcome to the fourth and final module of the **Agentic AI Masterclass**! This module is focused on **Deep Autonomous Agents**. These systems represent the absolute cutting-edge of agentic engineering, utilizing planning middleware, sandboxed filesystems, and sub-agent delegation to tackle long-horizon, multi-step, complex engineering and research tasks autonomously.

---

## 🗺️ Topics Covered

In this module, you will learn the three architectural pillars of state-of-the-art autonomous agents (such as Claude Code, Manus, and Deep Research):
1. **Planning (`write_todos` / `read_todos`)**: Forcing the agent to outline its goals, track completed tasks, and dynamically re-prioritize its workflow as new facts are discovered.
2. **Context Sandboxing (Filesystem Backends)**: Providing the agent with access to a virtual disk backend (`ls`, `read_file`, `write_file`, `edit_file`, `glob`, `grep`) to organize context, parse extensive documents, write code, and persist information outside the raw LLM prompt window.
3. **Sub-Agent Delegation (`task()`)**: Spawning isolated helper agents with dedicated, microscopic instructions to run independent pipelines, offloading massive token payloads and keeping the main agent's context window extremely clean and reliable.

You will learn how to implement these capabilities cleanly using LangChain's open-source **`deepagents`** harness built on top of LangGraph.

---

## 📂 Notebook & Code Directory

* **`01-basicsdeepagent.ipynb`**: Learn how to spin up a Deep Agent, configure custom tools (such as Tavily search), bind a model (such as OpenAI or Groq Qwen), write planning custom systems prompts, and trigger autonomous long-running execution loops.

---

## 🚀 How to Run

1. Ensure your virtual environment is active:
   ```bash
   .venv\Scripts\Activate.ps1   # Windows
   # source .venv/bin/activate  # macOS/Linux
   ```
2. Install the necessary packages for this module:
   ```bash
   pip install deepagents tavily-python python-dotenv
   ```
3. Make sure your `.env` contains:
   * `OPENAI_API_KEY`
   * `GROQ_API_KEY`
   * `TAVILY_API_KEY`
4. Launch your Jupyter environment and open `01-basicsdeepagent.ipynb`:
   ```bash
   jupyter notebook
   ```
