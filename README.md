# Vector Search in Elasticsearch

This repository shows how to build a vector search solution using Elasticsearch. It includes generating embeddings with OpenAI, indexing data with dense vectors, and performing vector similarity queries.

---

## Features

- Load movie data from CSV  
- Generate text embeddings via OpenAI API  
- Create Elasticsearch index with dense_vector fields  
- Bulk index documents with embeddings  
- Perform k-NN vector searches based on semantic similarity  

---

## Setup

1. Clone the repo:

    ```bash
    git clone https://github.com/manish-ch0pra/VectorSearchInElasticsearch.git
    cd VectorSearchInElasticsearch
    ```

2. Run Elasticsearch locally (via Docker):

    ```bash
    docker run -d -p 9200:9200 -e "discovery.type=single-node" elasticsearch:8.13.0
    ```

3. Update your OpenAI API keys and endpoint in the script (from Azure AI Foundry).

4. Run the provided notebook to:
- Generate embeddings for your movie descriptions  
- Create the Elasticsearch index with vector mapping  
- Bulk upload the documents  
- Perform vector similarity search queries  

---