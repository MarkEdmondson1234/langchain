# VectorStore Implementation using Redis

This code defines a VectorStore implementation using Redis. It includes classes for managing collections and embeddings, as well as a query result class and a distance strategy enum.

## Functions

The code defines several helper classes and functions, including `CollectionStore`, `EmbeddingStore`, `QueryResult`, and `DistanceStrategy`.

- `_check_redis_module_exist`: Check if the correct Redis modules are installed.
- `_check_index_exists`: Check if Redis index exists.
- `_redis_key`: Redis key schema for a given prefix.
- `_redis_prefix`: Redis key prefix for a given index.
- `_default_relevance_score`: Default relevance score function.

# Inputs and outputs for each function

- `_check_redis_module_exist`:
    - Inputs: Redis client, required modules
    - Outputs: None

- `_check_index_exists`:
    - Inputs: Redis client, index name
    - Outputs: boolean indicating whether index exists

- `_redis_key`:
    - Inputs: prefix
    - Outputs: Redis key schema

- `_redis_prefix`:
    - Inputs: index name
    - Outputs: Redis key prefix

- `_default_relevance_score`:
    - Inputs: float value
    - Outputs: float value

This code defines a VectorStore implementation using Redis. The `Redis(VectorStore)` class is a wrapper around Redis vector database and includes functions for managing collections and embeddings, as well as a query result class and a distance strategy enum. The code defines several helper classes and functions, including `_check_redis_module_exist`, `_check_index_exists`, `_redis_key`, `_redis_prefix`, and `_default_relevance_score`. 

- `_check_redis_module_exist`: checks if the correct Redis modules are installed.
- `_check_index_exists`: checks if Redis index exists.
- `_redis_key`: defines Redis key schema for a given prefix.
- `_redis_prefix`: defines Redis key prefix for a given index.
- `_default_relevance_score`: defines default relevance score function.

The `Redis(VectorStore)` class has an `__init__` function that initializes necessary components including `redis_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `relevance_score_fn`. It also has a `_create_index` function that creates a Redis index with a given `dim` value. The `add_texts` function adds more texts to the vectorstore and returns a list of IDs. 

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, embeddings, keys, batch size, and optional parameters
    - Outputs: list of IDs

The code defines a VectorStore implementation using Redis. The `Redis(VectorStore)` class is a wrapper around Redis vector database and includes functions for managing collections and embeddings, as well as a query result class and a distance strategy enum. The code defines several helper classes and functions, including `_check_redis_module_exist`, `_check_index_exists`, `_redis_key`, `_redis_prefix`, and `_default_relevance_score`. 

- `_check_redis_module_exist`: checks if the correct Redis modules are installed.
- `_check_index_exists`: checks if Redis index exists.
- `_redis_key`: defines Redis key schema for a given prefix.
- `_redis_prefix`: defines Redis key prefix for a given index.
- `_default_relevance_score`: defines default relevance score function.

The `Redis(VectorStore)` class has an `__init__` function that initializes necessary components including `redis_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `relevance_score_fn`. It also has a `_create_index` function that creates a Redis index with a given `dim` value. The `add_texts` function adds more texts to the vectorstore and returns a list of IDs. 

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, embeddings, keys, batch size, and optional parameters
    - Outputs: list of IDs

The `similarity_search` function returns the most similar indexed documents to the query text. 

- `similarity_search`:
    - Inputs: query text, number of documents to return, and optional parameters
    - Outputs: list of documents that are most similar to the query text

The `similarity_search_limit_score` function returns the most similar indexed documents to the query text within the score_threshold range.

- `similarity_search_limit_score`:
    - Inputs: query text, number of documents to return, minimum matching score required for a document to be considered a match, and optional parameters
    - Outputs: list of documents that are most similar to the query text, including the match score for each document. If there are no documents that satisfy the score_threshold value, an empty list is returned.

The code defines a VectorStore implementation using Redis. The `Redis(VectorStore)` class is a wrapper around Redis vector database and includes functions for managing collections and embeddings, as well as a query result class and a distance strategy enum. The code defines several helper classes and functions, including `_check_redis_module_exist`, `_check_index_exists`, `_redis_key`, `_redis_prefix`, and `_default_relevance_score`. 

- `_check_redis_module_exist`: checks if the correct Redis modules are installed.
- `_check_index_exists`: checks if Redis index exists.
- `_redis_key`: defines Redis key schema for a given prefix.
- `_redis_prefix`: defines Redis key prefix for a given index.
- `_default_relevance_score`: defines default relevance score function.

The `Redis(VectorStore)` class has an `__init__` function that initializes necessary components including `redis_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `relevance_score_fn`. It also has a `_create_index` function that creates a Redis index with a given `dim` value. The `add_texts` function adds more texts to the vectorstore and returns a list of IDs. 

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, embeddings, keys, batch size, and optional parameters
    - Outputs: list of IDs

The `similarity_search` function returns the most similar indexed documents to the query text. 

- `similarity_search`:
    - Inputs: query text, number of documents to return, and optional parameters
    - Outputs: list of documents that are most similar to the query text

The `similarity_search_limit_score` function returns the most similar indexed documents to the query text within the score_threshold range.

- `similarity_search_limit_score`:
    - Inputs: query text, number of documents to return, minimum matching score required for a document to be considered a match, and optional parameters
    - Outputs: list of documents that are most similar to the query text, including the match score for each document. If there are no documents that satisfy the score_threshold value, an empty list is returned.

This code defines a VectorStore implementation using Redis. The `Redis(VectorStore)` class is a wrapper around Redis vector database and includes functions for managing collections and embeddings, as well as a query result class and a distance strategy enum. The code defines several helper classes and functions, including `_check_redis_module_exist`, `_check_index_exists`, `_redis_key`, `_redis_prefix`, and `_default_relevance_score`. 

- `_check_redis_module_exist`: checks if the correct Redis modules are installed.
- `_check_index_exists`: checks if Redis index exists.
- `_redis_key`: defines Redis key schema for a given prefix.
- `_redis_prefix`: defines Redis key prefix for a given index.
- `_default_relevance_score`: defines default relevance score function.

The `Redis(VectorStore)` class has an `__init__` function that initializes necessary components including `redis_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `relevance_score_fn`. It also has a `_create_index` function that creates a Redis index with a given `dim` value. The `add_texts` function adds more texts to the vectorstore and returns a list of IDs. 

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, embeddings, keys, batch size, and optional parameters
    - Outputs: list of IDs

The `similarity_search` function returns the most similar indexed documents to the query text. 

- `similarity_search`:
    - Inputs: query text, number of documents to return, and optional parameters
    - Outputs: list of documents that are most similar to the query text

The `similarity_search_limit_score` function returns the most similar indexed documents to the query text within the score_threshold range.

- `similarity_search_limit_score`:
    - Inputs: query text, number of documents to return, minimum matching score required for a document to be considered a match, and optional parameters
    - Outputs: list of documents that are most similar to the query text, including the match score for each document. If there are no documents that satisfy the score_threshold value, an empty list is returned.

The code defines a VectorStore implementation using Redis. The `Redis(VectorStore)` class is a wrapper around Redis vector database and includes functions for managing collections and embeddings, as well as a query result class and a distance strategy enum. The code defines several helper classes and functions, including `_check_redis_module_exist`, `_check_index_exists`, `_redis_key`, `_redis_prefix`, and `_default_relevance_score`. 

- `_check_redis_module_exist`: checks if the correct Redis modules are installed.
- `_check_index_exists`: checks if Redis index exists.
- `_redis_key`: defines Redis key schema for a given prefix.
- `_redis_prefix`: defines Redis key prefix for a given index.
- `_default_relevance_score`: defines default relevance score function.

The `Redis(VectorStore)` class has an `__init__` function that initializes necessary components including `redis_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `relevance_score_fn`. It also has a `_create_index` function that creates a Redis index with a given `dim` value. The `add_texts` function adds more texts to the vectorstore and returns a list of IDs. 

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, embeddings, keys, batch size, and optional parameters
    - Outputs: list of IDs

The `similarity_search` function returns the most similar indexed documents to the query text. 

- `similarity_search`:
    - Inputs: query text, number of documents to return, and optional parameters
    - Outputs: list of documents that are most similar to the query text

The `similarity_search_limit_score` function returns the most similar indexed documents to the query text within the score_threshold range.

- `similarity_search_limit_score`:
    - Inputs: query text, number of documents to return, minimum matching score required for a document to be considered a match, and optional parameters
    - Outputs: list of documents that are most similar to the query text, including the match score for each document. If there are no documents that satisfy the score_threshold value, an empty list is returned.

The `RedisVectorStoreRetriever` class is a Pydantic object that retrieves relevant documents from the Redis vector store. It has the following functions:

- `get_relevant_documents`: returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit".
    - Inputs: query text
    - Outputs: list of documents that are most relevant to the query text
- `add_documents`: adds documents to the vectorstore
    - Inputs: list of documents
    - Outputs: list of IDs
- `aadd_documents`: adds documents to the vectorstore asynchronously
    - Inputs: list of documents
    - Outputs: list of IDs
- `agete_relevant_documents`: retrieves relevant documents from the Redis vector store asynchronously
    - Inputs: query text
    - Outputs: list of documents that are most relevant to the query text

