RAG with Groq

A Retrieval-Augmented Generation (RAG) pipeline that retrieves relevant document chunks from a vector store and uses Groq's LLM API to generate answers based on that context.

Features


Document embedding and storage in a vector database
Semantic search using cosine similarity
Answer generation using Groq's LLM API
Configurable similarity threshold and top-k retrieval
Project Structure
├── RAG.ipynb          # Main notebook with retriever and generator classes
├── DATA/               # Folder for source documents (not included in repo)
├── .env                # API keys (not included in repo)
├── .gitignore
└── README.md
How It Works
Documents are split into chunks and converted into embeddings
Embeddings are stored in a vector database
A user query is embedded and compared against stored embeddings using cosine similarity
The most relevant chunks are retrieved based on a similarity threshold
Retrieved chunks are passed to Groq's LLM as context to generate a final answer
