# 🕸️ Module 3: LangGraph Advanced Workflows

Welcome to the third module of the **Agentic AI Masterclass**! This module is focused on **State Management, Cyclical Workflows, Human-in-the-loop, and Multi-Agent Collaboration** using **LangGraph**. LangGraph is the premier framework for building advanced agentic systems because it lets you model workflows as graph nodes (actions) and edges (decisions), allowing models to loop, self-correct, and maintain a shared state.

---

## 🗺️ Topics Covered

In this module, you will learn how to:
1. Transition from linear, one-shot sequential chains to complex **cyclical state graphs**.
2. Manage conversations, memory, and custom schemas inside a shared state object.
3. Establish **Human-in-the-loop (HITL)** gates. Learn how to pause graph execution when an agent wants to perform a sensitive task (e.g., executing a database write or generating an invoice), solicit human input or approval, and resume execution.
4. Use state-travel debugging tools to trace how inputs mutate the graph's state step-by-step.
5. Build **Multimodal Agent nodes** that parse images, charts, and diagrams as native node inputs.
6. Design **Multi-Agent Systems** utilizing the *Supervisor* pattern. Build teams of specialized worker agents (e.g., Researcher, Coder, Writer) that run isolated tasks and collaborate to deliver a final, unified report.

---

## 📂 Notebook Directory

* **`1-BasicChatbot/chatbot.ipynb`**: Introduction to stateful LangGraph graphs, compiling, and running cyclical conversational systems.
* **`2-HumanAssistance/humanintheloop.ipynb`**: Setting checkpoints and interrupts to pause execution, solicit user feedback/approval, and resume execution cleanly.
* **`3-Debugging/debugging.ipynb`**: Accessing graph history, executing state-time-travel to inspect past states, and debugging state variables.
* **`4-Multimodal/1-multimodalopenai.ipynb`**: Processing multiple visual modalities (image diagrams, file assets) inside graph reasoning nodes.
* **`Agents/multiaiagent.ipynb`**: Constructing multi-agent collaboration structures with supervisor delegation, parallel execution, and state reconciliation.

---

## 🚀 How to Run

1. Ensure your virtual environment is active:
   ```bash
   .venv\Scripts\Activate.ps1   # Windows
   # source .venv/bin/activate  # macOS/Linux
   ```
2. Install the specific requirements for this module:
   ```bash
   pip install -r requirements.txt
   ```
3. Make sure your `.env` contains `OPENAI_API_KEY`, `GROQ_API_KEY`, and `TAVILY_API_KEY`.
4. Run Jupyter Notebook and start with the basic stateful chatbot:
   ```bash
   jupyter notebook
   ```
