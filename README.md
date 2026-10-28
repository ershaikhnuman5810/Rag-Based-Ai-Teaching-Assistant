RAG-Based AI Teaching Assistant
A Retrieval-Augmented Generation (RAG) project that helps students ask questions about web development course materials and receive answers grounded in relevant course content.
Features
Answers questions about course topics using retrieved text chunks.
Uses BGE-M3 embeddings to represent course content and questions.
Uses Ollama with Llama 3.2 to generate answers locally.
Works with course material stored in JSON chunk files.
Can include relevant video titles and timestamps when that information exists in the retrieved material.
Tech Stack
Python
Jupyter Notebook
Ollama
Llama 3.2
BGE-M3
JSON
How It Works
Load course text chunks from JSON files.
Create embeddings for the course chunks with BGE-M3.
Retrieve chunks relevant to a student's question.
Send the question and retrieved context to Llama 3.2 through Ollama.
Display the generated answer.
Prerequisites
Python installed on your computer.
Ollama installed and running.
The required Ollama models downloaded:
ollama pull bge-m3
ollama pull llama3.2
The Python packages used by your code installed in the same environment as your notebook or application.
Setup
Clone this repository:
git clone https://github.com/YOUR-USERNAME/rag-based-ai-teaching-assistant.git
cd rag-based-ai-teaching-assistant
Start Ollama and confirm the models are available:
ollama list
Install the Python dependencies listed in requirements.txt (once you have created that file):
pip install -r requirements.txt
Open and run the Jupyter Notebook, or run app.py if you have created the application script.
Note: Update the repository URL and commands to match your GitHub username and actual file names. The exact Python dependencies should match the imports in your code.
Example Questions
What is HTML?
What is Flexbox in CSS?
Which course video explains the video tag?
At what timestamp is a topic discussed?
Project Structure
rag-based-ai-teaching-assistant/
├── app.py                  # Optional main Python application
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
├── .gitignore              # Files Git should ignore
├── notebooks/              # Optional Jupyter notebooks
└── data/                   # Course JSON chunks (only if sharing is permitted)
