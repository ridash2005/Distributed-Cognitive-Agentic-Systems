# 🛠️ Module 1: LangChain Fundamentals

Welcome to the first module of the **Agentic AI Masterclass**! This module is focused on the core building blocks of LLM integration and chaining. Understanding how to programmatically control LLMs, pass messages, enforce strict output structures, and connect custom tools is foundational to building agentic systems.

---

## 🗺️ Topics Covered

In this module, you will learn how to:
1. Connect to standard LLM endpoints using **LangChain Expression Language (LCEL)**.
2. Bind **custom Python functions as tools** for the LLM to call.
3. Handle **Message History** dynamically (Systems, Human, AI, and Tool message schemas).
4. Enforce **Structured Outputs** matching exact Pydantic JSON schemas.
5. Create **Custom Middleware** to intercept the agent's lifecycle (logging, prompt adjustments, token counting).
6. Build a **Centralized LLM Gateway** to effortlessly switch between model providers (OpenAI, Anthropic, Gemini, Groq).
7. Construct **Prompt and Output Guardrails** to enforce safety and prevent hallucination.

---

## 📂 Notebook Directory

* **`updatedlangchain/1-langchainintro.ipynb`**: Your gateway to LangChain. Learn basic expression chains and model invocations.
* **`updatedlangchain/2-modelintegration.ipynb`**: Deep dive into binding prompts, formatting templates, and model parameters.
* **`updatedlangchain/3-tools.ipynb`**: Learn how to convert standard Python functions into schemas the model can understand and invoke.
* **`updatedlangchain/4-messages.ipynb`**: Mastering chat states and managing message histories programmatically.
* **`updatedlangchain/5-structuredoutput.ipynb`**: Forcing the model to return formatted objects (e.g., JSON schemas) rather than raw natural text.
* **`updatedlangchain/6-middleware.ipynb`**: Implementing interceptors, logging, and custom logic layers around LLM executions.
* **`updatedlangchain/langchain_guardrails_crash_course.ipynb`**: Guarding LLM chains against prompt injection and toxic completions.
* **`llm_gateway_tutorial.ipynb`**: Setting up a unified abstraction gateway to seamlessly interact with multiple APIs.

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
3. Create your `.env` file at the root of the project with your API keys (e.g., `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`).
4. Launch your Jupyter notebook environment:
   ```bash
   jupyter notebook
   ```
   Open the notebooks in order starting from `1-langchainintro.ipynb`.
