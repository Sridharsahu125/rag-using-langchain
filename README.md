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
   git clone https://github.com/Sridharsahu125/rag-using-langchain.git
   cd rag-langchain


##Installation Requared Dependency :

pip install youtube-transcript-api langchain-community langchain-openai faiss-cpu tiktoken python-dotenv

##Set up your OpenAI API key:
export OPENAI_API_KEY="your-api-key-here"

Usage

Step 1: 
Indexing (Document Ingestion)
Fetch a YouTube video transcript using its ID.


Flatten the transcript into plain text.


Step 2: 
Text Splitting
Split the transcript into chunks using RecursiveCharacterTextSplitter.


Step 3: 
Embedding Generation and Storage
Generate embeddings for the text chunks using OpenAI's embeddings model.


Store the embeddings in a FAISS vector store.


Step 4:
Retrieval
Retrieve relevant document chunks based on a query using similarity search.


Step 5:
Augmentation and Generation
Augment the query with the retrieved context.


Generate a response using a language model (e.g., OpenAI's GPT).
