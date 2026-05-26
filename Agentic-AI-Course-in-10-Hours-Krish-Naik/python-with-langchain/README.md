# Python with LangChain Course

Welcome to the **Python with LangChain** repository. This project contains tutorials and examples for learning LangChain, ranging from model integrations and standard message structures to binding tools, tool execution loops, and creating autonomous agents.

---

## 📖 Documentation

For an in-depth developer guide covering the core concepts of this course, refer to the:
👉 **[LangChain Developer Guide](docs/langchain_guide.md)**

---

## 🗂️ Repository Notebooks Overview

The course is structured into the following step-by-step Jupyter notebooks:

1. **[1-langchain-intro.ipynb](langchain/1-langchain-intro.ipynb)**
   - Introduction to LangChain.
   - Defining custom tools using the `@tool` decorator.
   - Building and invoking basic agents using `create_agent` from `langchain.agents`.

2. **[2-model-integration.ipynb](langchain/2-model-integration.ipynb)**
   - Dynamic model integration using unified initialization with `init_chat_model()`.
   - Direct provider-specific imports and setup for **OpenAI**, **Google Gemini**, and **Groq** models.

3. **[3-tools.ipynb](langchain/3-tools.ipynb)**
   - Understanding LangChain schemas and executable tool functions.
   - Binding tools to a model with `model.bind_tools()`.
   - Inspecting model `tool_calls` output and executing manual tool calling loops.

4. **[4-messages.ipynb](langchain/4-messages.ipynb)**
   - Deep dive into LangChain's standard message objects (`SystemMessage`, `HumanMessage`, `AIMessage`, `ToolMessage`).
   - Constructing and managing conversational history.
   - Implementing a step-by-step tool calling message flow.

---

## ⚙️ Quick Start Setup

### 1. Install Dependencies
Make sure you have your virtual environment activated, then install packages listed in `[requirements.txt](requirements.txt)`:
```bash
pip install -r requirements.txt
```

### 2. Configure Environment Variables
Create a `[.env](.env)` file in the root directory (you can copy `[.env.sample](.env.sample)`) and fill in your API keys:
```env
OPENAI_API_KEY=your_openai_api_key_here
GOOGLE_API_KEY=your_google_api_key_here
GROQ_API_KEY=your_groq_api_key_here
```

---

## 🖥️ Running the Notebooks in VS Code

1. Open any of the notebook files in the `[langchain/](langchain/)` folder.
2. Click the **Select Kernel** button in the top-right corner of the notebook editor.
3. Click **Python Environments...** and select the interpreter pointing to the local virtual environment: `./.venv/Scripts/python.exe` (often labeled as `python-with-langchain (.venv)`).
4. Run the cells sequentially.
