# Text-Summarizer-AI-Project
Using LLaMA (via Ollama), FastAPI &amp; Streamlit


## Features
- FastAPI backend
- Streamlit frontend
- Local LLaMA inference using Ollama

## Setup Instructions
1. Clone the repository
2. Install dependencies:
   pip install -r requirements.txt
3. Start backend:
   uvicorn backend.main:app --reload
4. Start frontend:
   streamlit run frontend/app.py



🧠 Text Summarizer AI

Local LLaMA Inference with FastAPI & Streamlit

A full-stack AI application that performs text summarization using a locally hosted LLaMA model via Ollama, featuring a FastAPI backend and a Streamlit frontend. This project runs entirely offline, ensuring data privacy, low latency, and zero API costs.

📌 Project Overview
🎯 Goal

Build a modern, modular AI application that:

Runs LLMs locally without cloud dependencies

Provides a clean API layer for inference

Offers a simple, interactive web UI for users

Follows real-world engineering best practices

🚀 Features

⚡ FastAPI backend for high-performance API handling

🎨 Streamlit frontend for real-time user interaction

🧠 Local LLaMA inference using Ollama

🔒 Privacy-first (no external API calls)

💸 Cost-efficient (no usage fees)

🧩 Modular architecture (easy to extend)

🛠️ Technology Stack
Component	Technology
LLM Runtime	Ollama (LLaMA)
Backend API	FastAPI
Frontend UI	Streamlit
Language	Python
Version Control	Git & GitHub
📂 Project Structure
text-summarizer-ai/
│
├── backend/
│   ├── main.py          # FastAPI application
│   ├── summarizer.py    # LLaMA / Ollama interaction logic
│   └── __init__.py
│
├── frontend/
│   └── app.py           # Streamlit UI
│
├── requirements.txt     # Python dependencies
├── README.md            # Project documentation
└── .gitignore

⚙️ Prerequisites

Before running the project, ensure you have:

Python 3.9+

Ollama installed

LLaMA model pulled locally

Git

Install Ollama

👉 https://ollama.com

Pull a model (example):

ollama pull llama2


Verify Ollama is running:

ollama list

🧪 Setup Instructions
1️⃣ Clone the repository
git clone <your-repo-url>
cd text-summarizer-ai

2️⃣ Create & activate a virtual environment (recommended)
python -m venv venv


macOS / Linux

source venv/bin/activate


Windows

venv\Scripts\activate

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Start the FastAPI backend
uvicorn backend.main:app --reload


Backend will run at:

http://127.0.0.1:8000


Optional API docs:

http://127.0.0.1:8000/docs

5️⃣ Start the Streamlit frontend
streamlit run frontend/app.py


Frontend will open in your browser automatically.

🔁 How It Works (Architecture Flow)

User inputs text in Streamlit UI

Streamlit sends a request to FastAPI

FastAPI formats the prompt

Request is sent to local LLaMA via Ollama

Model generates summary

Summary is returned to UI in real time

📈 Example Use Cases

Summarizing long articles or documents

Private data processing without cloud exposure

Offline AI demos

LLM experimentation and prototyping

🔮 Future Enhancements

Docker containerization

Authentication & rate limiting

Multiple model selection

Streaming token responses

Logging & monitoring

CI/CD pipeline

🧠 Key Takeaways

Demonstrates LLM integration without cloud APIs

Showcases API design + frontend development

Highlights privacy-focused AI architecture

Easily extendable to chatbots, Q&A systems, or agents

🧑‍💻 Author

Khaleef Haughton
Built for learning, showcasing AI + backend engineering, and real-world system design.

📜 License

This project is open-source and available for educational and personal use.
