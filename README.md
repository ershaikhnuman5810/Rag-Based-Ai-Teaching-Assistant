# 🤖 RAG-Based AI Teaching Assistant

An AI-powered Teaching Assistant built using Retrieval-Augmented Generation (RAG) that helps students understand course materials by answering questions based on relevant educational content.

The system retrieves relevant information from course materials stored in JSON files and uses Large Language Models (LLMs) to generate context-based answers locally.

## 🚀 Features

- 📚 **Course-Based Question Answering:** Answers questions using relevant course materials.
- 🔍 **Semantic Search:** Retrieves relevant text chunks using BGE-M3 embeddings.
- 🧠 **Retrieval-Augmented Generation:** Combines retrieved information with an LLM to generate answers.
- 💻 **Local AI Processing:** Uses Ollama to run language models locally.
- 🎯 **Context-Aware Answers:** Generates answers based on retrieved course content.
- 🎥 **Video Reference Support:** Can include relevant video titles and timestamps when available in the source material.
- 📂 **JSON-Based Knowledge Base:** Supports course materials stored in JSON files.
- 🛠️ **Jupyter Notebook:** Provides an interactive environment for running the RAG pipeline.

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Jupyter Notebook | Development and execution |
| Ollama | Local model execution |
| BGE-M3 | Text embedding generation |
| Llama 3.2 | Answer generation |
| JSON | Course material storage |
| NumPy | Numerical operations |
| Pandas | Data processing |
| Scikit-learn | Cosine similarity |
| Joblib | Embedding storage |
| Requests | API communication |

## ⚙️ How It Works

1. **Load Course Materials:** Reads educational content from JSON files.
2. **Create Embeddings:** Converts course text into vector representations using BGE-M3.
3. **Store Embeddings:** Saves embeddings for reuse.
4. **Receive a Question:** Accepts a student's question.
5. **Retrieve Relevant Content:** Uses cosine similarity to find the most relevant text chunks.
6. **Generate an Answer:** Sends the question and retrieved context to Llama 3.2 through Ollama.
7. **Display the Result:** Returns an answer based on the retrieved course material.

## 📋 Prerequisites

Before running the project, ensure you have:

- Python 3.10 or a compatible version
- Jupyter Notebook
- Ollama installed and running
- Required Python packages installed
- Sufficient RAM and storage for the selected local AI models

## 📥 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/ershaikhnuman5810/Rag-Based-AI-Teaching-Assistant.git
2. Navigate to the Project Directory

cd Rag-Based-AI-Teaching-Assistant

3. Install Ollama Models

Install Ollama from its official website:

https://ollama.com/

Download the required models:

ollama pull bge-m3 ollama pull llama3.2

Verify the installed models:

ollama list

4. install Python Dependencies

If the repository contains a requirements. txt file, run:

pip install -r requirements.txt

Otherwise, install the packages required by your notebook:

pip install pandas numpy scikit-learn joblib requests jupyter

5. Start Jupyter Notebook

jupyter notebook

Open the notebook:

RAG-BASED AI TEACHING ASSISTANT.ipynb

Run the notebook cells in the correct order
Example Questions

You can ask questions such as:

What is HTML?

What is Flexbox in CSS?

What are semantic HTML tags?

How do HTML forms work?

Which course video explains the video tag?

At what timestamp is a particular topic discussed?

Answers depend on the information available in the course materials.
