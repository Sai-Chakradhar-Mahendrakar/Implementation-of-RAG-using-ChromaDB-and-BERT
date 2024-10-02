# ChromaDB and BERT Integration with Retrieval-Augmented Generation (RAG)

This repository demonstrates the integration of [BERT](https://huggingface.co/bert-base-uncased) embeddings with ChromaDB for document storage and querying. It also showcases a Retrieval-Augmented Generation (RAG) system for retrieving relevant documents based on queries.

## Features
- **BERT Embeddings**: Uses pre-trained BERT model to generate embeddings for document storage.
- **ChromaDB**: A database used to store document embeddings and metadata.
- **Query System**: Query through the stored documents and retrieve relevant information using BERT embeddings.
- **RAG System**: Example of a RAG model that retrieves documents and generates responses using context.

## RAG System Overview

Below is a diagram representing the Retrieval-Augmented Generation (RAG) system, where relevant documents are retrieved from ChromaDB based on a user query, and a generative model is used to formulate responses.

![RAG System](path_to_your_image.png)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name ```
2. Install the required packages:
   ```bash
   pip install chromadb
   ```
## Usage

1. Add documents to ChromaDB:
   ```bash
   documents = [
      {"dept": "HR", "content": "HR is responsible for recruiting new employees."},
      # Add more documents as needed
    ]
   add_documents_to_chromadb(documents, db_path="docs/")
   ```
2. Query documents from a specific department:
   ``` bash
   search_results = search_department_in_chromadb("docs/", department="IT", query="network", n_results=2)
   print(search_results)
   ```
## Contributing
Feel free to submit a pull request or open an issue to contribute to this project.
