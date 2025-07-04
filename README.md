# 🧠 MCQ Generator with OpenAI, LangChain, and Streamlit

A smart **Multiple Choice Question (MCQ) Generator** built using **OpenAI**, **LangChain**, and **Streamlit**. This tool allows users to generate MCQs from a given topic or content using advanced prompt engineering techniques and chaining methods like `SimpleChain` and `SequentialChain`. It also supports structured output in **JSON format** and maintains a **timeline log** for every interaction.

---

## 🚀 Features

- 🤖 **OpenAI-Powered Question Generation**  
  Utilizes OpenAI LLMs to generate high-quality MCQs based on user input or document content.

- 🔗 **LangChain Integration**  
  Combines multiple prompt chains using `SequentialChain` for multi-step MCQ generation.

- 🖥️ **Streamlit Interface**  
  A user-friendly web interface for entering prompts, viewing results, and managing MCQ creation.

- 🧾 **JSON Output Format**  
  Stores generated questions and answers in a structured JSON format.

- 🕒 **Timeline Logs**  
  Maintains a log of all user queries and responses with timestamps for traceability and debugging.

---

## 📂 Project Structure
mcqgen/
│
├── StreamlitAPP.py # Main Streamlit app
├── chains.py # LangChain chains and prompt templates
├── utils.py # Utility functions (e.g., JSON export, logging)
├── logs/
│ └── timeline.jsonl # Logs of all generations with timestamps
├── responses/
│ └── latest_output.json # Stores last generated MCQs
├── README.md # Project documentation
└── requirements.txt # Python dependencies


---

## 🛠️ Tech Stack

- [OpenAI GPT Models](https://platform.openai.com/)
- [LangChain](https://www.langchain.com/)
- [Streamlit](https://streamlit.io/)
- [Python 3.10+](https://www.python.org/)
- JSON, Logging

---

## 🧪 How It Works

1. **User Input**: A topic or passage is entered into the Streamlit UI.
2. **LangChain Prompts**: Sequential chains are used to first extract key concepts, then generate MCQs from them.
3. **Output**: The MCQs are displayed in the UI, saved in a JSON format, and logged with a timestamp.
4. **Review**: An optional review/comment can be added for feedback or improvement.

---

## ▶️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/mcqgenerator.git
cd mcqgenerator
