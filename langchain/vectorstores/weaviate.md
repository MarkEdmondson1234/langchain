The code defines a wrapper around Weaviate vector database. It includes several helper functions such as `_default_schema`, `_create_weaviate_client`, and `_default_score_normalizer`. The `VectorStore` class has an `__init__` function that initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`. It also has a `_create_index` function that creates a Weaviate index with a given `dim` value. The `add_documents` function adds more documents to the vectorstore and returns a list of IDs. The `get_relevant_documents` function returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit". The `maximal_marginal_relevance` function calculates maximal marginal relevance.

The code defines a wrapper around Weaviate vector database and includes several helper functions such as `_default_schema`, `_create_weaviate_client`, and `_default_score_normalizer`. The `VectorStore` class has an `__init__` function that initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`. It also has a `_create_index` function that creates a Weaviate index with a given `dim` value. The `add_documents` function adds more documents to the vectorstore and returns a list of IDs. The `get_relevant_documents` function returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit". The `maximal_marginal_relevance` function calculates maximal marginal relevance.

# Functions
- `_default_schema`: returns a dictionary that defines the schema for a given index name.
- `_create_weaviate_client`: creates and returns a Weaviate client.
- `_default_score_normalizer`: defines default score normalization function.
- `__init__`: initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`.
- `_create_index`: creates a Weaviate index with a given `dim` value.
- `add_documents`: adds more documents to the vectorstore and returns a list of IDs.
- `get_relevant_documents`: returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit".
- `maximal_marginal_relevance`: calculates maximal marginal relevance.

# Inputs and outputs for each function
- `_default_schema`:
    - Inputs: index name
    - Outputs: dictionary that defines the schema for a given index name
- `_create_weaviate_client`:
    - Inputs: client, weaviate_url, weaviate_api_key
    - Outputs: Weaviate client
- `_default_score_normalizer`:
    - Inputs: val
    - Outputs: float
- `__init__`:
    - Inputs: client, index_name, text_key, embedding, attributes, relevance_score_fn
    - Outputs: None
- `_create_index`:
    - Inputs: dim
    - Outputs: None
- `add_documents`:
    - Inputs: texts, metadatas, kwargs
    - Outputs: list of IDs
- `get_relevant_documents`:
    - Inputs: query
    - Outputs: list of documents that are most relevant to the query text
- `maximal_marginal_relevance`:
    - Inputs: query_embedding, embedding_list, lambda_mult, k
    - Outputs: list of indices

The code defines a wrapper around Weaviate vector database and includes several helper functions such as `_default_schema`, `_create_weaviate_client`, and `_default_score_normalizer`. The `VectorStore` class has an `__init__` function that initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`. It also has a `_create_index` function that creates a Weaviate index with a given `dim` value. The `add_documents` function adds more documents to the vectorstore and returns a list of IDs. The `get_relevant_documents` function returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit". The `maximal_marginal_relevance` function calculates maximal marginal relevance.

# Functions
- `_default_schema`: returns a dictionary that defines the schema for a given index name.
- `_create_weaviate_client`: creates and returns a Weaviate client.
- `_default_score_normalizer`: defines default score normalization function.
- `__init__`: initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`.
- `_create_index`: creates a Weaviate index with a given `dim` value.
- `add_documents`: adds more documents to the vectorstore and returns a list of IDs.
- `get_relevant_documents`: returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit".
- `maximal_marginal_relevance`: calculates maximal marginal relevance.

# Inputs and outputs for each function
- `_default_schema`:
    - Inputs: index name
    - Outputs: dictionary that defines the schema for a given index name
- `_create_weaviate_client`:
    - Inputs: client, weaviate_url, weaviate_api_key
    - Outputs: Weaviate client
- `_default_score_normalizer`:
    - Inputs: val
    - Outputs: float
- `__init__`:
    - Inputs: client, index_name, text_key, embedding, attributes, relevance_score_fn
    - Outputs: None
- `_create_index`:
    - Inputs: dim
    - Outputs: None
- `add_documents`:
    - Inputs: texts, metadatas, kwargs
    - Outputs: list of IDs
- `get_relevant_documents`:
    - Inputs: query
    - Outputs: list of documents that are most

The code defines a Weaviate wrapper that includes several helper functions such as `_default_schema`, `_create_weaviate_client`, and `_default_score_normalizer`. The `Weaviate` class has an `__init__` function that initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`. It also has a `_create_index` function that creates a Weaviate index with a given `dim` value. The `add_documents` function adds more documents to the Weaviate and returns a list of IDs. The `get_relevant_documents` function returns the most relevant documents to the query text based on the search type, which can be either "similarity" or "similarity_limit". The `maximal_marginal_relevance` function calculates maximal marginal relevance. The `similarity_search_with_score` function returns the most similar documents to the query text along with their similarity scores. The `_similarity_search_with_relevance_scores` function returns the most similar documents to the query text along with their relevance scores, normalized on a scale from 0 to 1. The `from_texts` class method constructs a Weaviate wrapper from raw documents.

The code defines a user-friendly interface that allows users to embed documents, create a new index for the embeddings in the Weaviate instance, and add the documents to the newly created Weaviate index. The `from_texts` class method constructs a Weaviate wrapper from raw documents. It uses several helper functions such as `_default_schema`, `_create_weaviate_client`, and `_default_score_normalizer`. The `Weaviate` class has an `__init__` function that initializes necessary components including `weaviate_url`, `index_name`, `embedding_function`, `content_key`, `metadata_key`, `vector_key`, and `score_normalizer_fn`. The `add_documents` function adds more documents to the Weaviate and returns a list of IDs. 

# Inputs and outputs for each function
- `from_texts`:
    - Inputs: `texts`, `embedding`, `metadatas`, `**kwargs`
    - Outputs: `Weaviate` instance

