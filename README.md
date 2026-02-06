# LangChain Prompt Engineering & Chat UI Lab

This repository contains a collection of Python implementations for **Prompt Engineering**, **Contextual Chatbots**, and **Automated Research Summarization** using the LangChain framework. It demonstrates how to manage complex LLM workflows, maintain chat history, and deploy interactive AI tools.

## 🌟 Key Features

### 1. Advanced Prompt Management
* **Dynamic Templates**: Generation and persistence of complex prompt templates to JSON format for reusability.
* **Chat Configurations**: Pre-defined domain-specific expert roles (e.g., Cricket Expert) using `ChatPromptTemplate`.
* **Multi-Lingual Greeting**: Demonstration of simple variable injection for automated tasks.

### 2. Conversational AI & History
* **Stateful Chatbots**: Interactive CLI-based chatbots that maintain context using `HumanMessage` and `AIMessage`.
* **History Persistence**: Loading and managing external chat history files using `MessagesPlaceholder` to provide customer support context.

### 3. Research Tool (Streamlit UI)
* **Summarization Engine**: A web interface that allows users to select research papers and customize the explanation style (Beginner, Technical, etc.) and length.
* [cite_start]**Logic-Guided Summaries**: Enforces mathematical details, analogies, and accuracy checks via structured templates[cite: 1].

---

## 🛠️ Project Structure

| File | Description |
| :--- | :--- |
| `prompt_ui.py` | Streamlit application for the Research Tool. |
| `chatbot.py` | CLI chatbot with persistent session history. |
| `prompt_generator.py`| Script to create and save JSON-based prompt templates. |
| `messages_placeholder.py` | Logic for loading chat history from external text files. |
| `template.json` | [cite_start]A serialized prompt configuration for standardized research analysis[cite: 1]. |

---

## ⚙️ Installation & Setup

### Prerequisites
* Python 3.9+
* OpenAI or Groq API Key

### 1. Install Dependencies
```bash
pip install langchain langchain-openai langchain-groq streamlit python-dotenv
