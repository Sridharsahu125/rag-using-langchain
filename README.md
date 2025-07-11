# RAG Implementation using LangChain

This project demonstrates a Retrieval-Augmented Generation (RAG) pipeline using LangChain to process and query YouTube video transcripts. The implementation includes document ingestion, text splitting, embedding generation, vector storage, retrieval, and generation of responses based on the retrieved context.

## Features

- **Document Ingestion**: Fetches and processes YouTube video transcripts.
- **Text Splitting**: Uses `RecursiveCharacterTextSplitter` to split transcripts into manageable chunks.
- **Embedding Generation**: Leverages OpenAI's `text-embedding-3-small` model to generate embeddings.
- **Vector Storage**: Stores embeddings in a FAISS vector store for efficient retrieval.
- **Retrieval-Augmented Generation**: Retrieves relevant document chunks and generates responses using a language model.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/rag-langchain.git
   cd rag-langchain


