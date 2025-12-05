# 📘 Q&A Chatbot using LangChain, FAISS & Ollama

This project implements a **PDF-based Question-Answering** Chatbot built using:

LangChain (LLM orchestration)

FAISS (vector database for semantic search)

Ollama (local LLM inference)

Embeddings-based document retrieval

The chatbot allows users to upload PDF files, process them into embeddings, store them locally, and then ask natural-language questions about the content.

## 🚀 Features

✔ Load and process PDF documents

✔ Extract text and create embeddings

✔ Store vectors in FAISS for fast retrieval

✔ Retrieve context based on user queries

✔ Generate answers using an Ollama LLM model

✔ Runs fully locally, no external API required

## 🧠 How It Works

Load PDF → Text extraction from pages

Chunk & Embed → Generate semantic embeddings

Store in FAISS → Vector index for similarity search

User Query → Embed + search nearest chunks

Ollama LLM → Generate final response based on retrieved context

## 📁 Project Structure
```
├── QAChatbot.ipynb           # Main notebook
├── requirements.txt          # Project dependencies
├── README.md                 # Project documentation
└── data/                     # PDF files
```

## 🛠 Installation

Install dependencies:

`pip install -r requirements.txt`


## Install and run Ollama:
https://ollama.com/download

Pull a model (example):

`ollama pull phi`

## ▶️ Running the Notebook

Start Jupyter:

`jupyter notebook`


Open QAChatbot.ipynb and run all cells.

## 📄 Requirements

### Key libraries:

langchain

langchain-community

langchain-core

langchain-ollama

faiss-cpu

python-dotenv

Full list is in requirements.txt.

## 📚 Example Workflow

Place your PDF into the data/ folder.

Run the notebook or script.

The system loads the PDF, creates embeddings, and builds a FAISS index.

Ask any question — the chatbot retrieves relevant chunks and generates an answer.

## 🧩 Customization

### You can modify:

PDF loader

Chunk size

Embedding model

Ollama model version

Retrieval strategy

## 🛡 Notes

No API keys are required unless you swap Ollama for an API-based LLM.

Embedding may take longer for large PDFs.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
