RAG Q&A System
A Retrieval-Augmented Generation system capable of answering user questions by indexing and retrieving information from PDF documents. The system supports multi-session interactions and maintains conversation history for context-aware responses.

Overview:-
This project demonstrates a practical implementation of document-based question answering using a combination of:
Document loaders
Text chunking
Embedding models
Vector similarity search
LLM-based response generation
The UI is built in Streamlit to support PDF uploads, interactive chat, and persistent session handling.

Features:-
Multi-session conversational interface
PDF ingestion and preprocessing
Text chunking with overlap
Embedding generation using HuggingFace models
Vector database using Chroma
Context-aware question refinement
Answer generation using Groq or other LLMs
Session history stored in memory for continuity

System Architecture :-
User uploads one or more PDFs
Text is extracted and chunked
Embeddings are generated for each chunk
Chroma vector store indexes the embeddings
User question is reformulated using history
Relevant chunks are retrieved
LLM generates a grounded answer
Response and history are displayed in the UI

Tech Stack:-
Python
LangChain
HuggingFace Embeddings
ChromaDB
Groq API / LLM of choice
Streamlit
PyPDFLoader

Project Structure:-
RAG-QA-System/
│
├── app.py
├── rag_pipeline.py
├── embeddings/
├── vectorstore/
├── utils/
│   └── text_processing.py
│
├── requirements.txt
└── README.md

Installation:-
pip install -r requirements.txt
streamlit run app.py

Future Enhancements:-
Add support for multiple file formats
Implement long-term memory
Add evaluation metrics
Deploy on cloud
