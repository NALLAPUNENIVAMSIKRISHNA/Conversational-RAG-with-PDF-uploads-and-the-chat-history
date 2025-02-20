# Conversational-RAG-with-PDF-uploads-and-the-chat-history

This project builds a question-answering app using PDFs, Langchain, ChromaDB, and Gemma. Users upload PDFs, ask questions, and maintain chat history.

Live Demo Video - https://drive.google.com/file/d/1_QjZfpFkHUq7Gw3yweFIDsGyCK2TVXqD/view?usp=sharing

## Features

*   PDF upload & Q&A
*   Persistent ChromaDB vector store (`is_persistent=True`)
*   Chat history maintained
*   Streamlit UI
*   Gemma LLM integration
*   Hugging Face embeddings

## Installation

3.  `python3 -m venv venv &&  `venv\Scripts\activate` 
4.  `pip install -r requirements.txt` (or individual packages: `streamlit langchain chromadb sentence-transformers python-dotenv langchain-groq langchain-huggingface`)
5.  Create `.env` file: `GROQ_API_KEY=YOUR_KEY`, `HF_TOKEN=YOUR_TOKEN` (of your own from hugging face and chat groq cloud websites)

## Usage

`streamlit run app.py`

## How it works

PDFs are processed, embeddings created, and stored in persistent ChromaDB. Langchain manages the conversational flow, using chat history for context. Gemma answers questions via the Streamlit UI.

## Requirements

Python 3.7+, Streamlit, Langchain, ChromaDB, Hugging Face `sentence-transformers`, `python-dotenv`, `langchain-groq`, `langchain-huggingface`
