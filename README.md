# RAG Q&A Chat System

Interactive Retrieval-Augmented Generation (RAG) system with PDF uploads and chat history using Streamlit.

## Project Structure
- `streamlit_app.py` : Main Streamlit app
- `requirements.txt` : Python dependencies
- `.env.example` : Placeholder for API keys


## Installation

```bash
git clone https://github.com/yourusername/rag-qa-chat.git
cd rag-qa-chat
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate
pip install -r requirements.txt



## Running the App
streamlit run streamlit_app.py


Visit http://localhost:8501 in your browser.

## Features

Upload multiple PDF documents and query their content.

Session-based chat history per user.

History-aware question reformulation for context.

Context-aware, concise answers from LLM using Groq API.

Streamlit interface for interactive use.

Tools/Technologies

Python, Streamlit, LangChain, Groq API, HuggingFace Embeddings, Chroma, PyPDFLoader
