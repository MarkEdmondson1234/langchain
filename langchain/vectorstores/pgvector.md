This code defines a wrapper around a Postgres/PGVector database. It includes classes for managing collections and embeddings, as well as a query result class and a distance strategy enum. The `CollectionStore` class manages collections and their metadata, while the `EmbeddingStore` class manages embeddings and their metadata. The `QueryResult` class represents the result of a query, including the embedding and distance. The `DistanceStrategy` enum defines different distance metrics for use in similarity search. 

# Inputs and outputs for each function
`CollectionStore.get_by_name`:
- `session`: a SQLAlchemy session object
- `name`: a string representing the name of the collection to retrieve
Returns an instance of the `CollectionStore` class or `None`.

`CollectionStore.get_or_create`:
- `session`: a SQLAlchemy session object
- `name`: a string representing the name of the collection to retrieve or create
- `cmetadata`: an optional dictionary representing metadata for the collection
Returns a tuple containing an instance of the `CollectionStore` class and a boolean indicating whether the collection was created.

`EmbeddingStore`:
- `collection_id`: a UUID representing the ID of the collection to which the embedding belongs
- `embedding`: a vector of floats representing the embedding
- `document`: an optional string representing the document associated with the embedding
- `cmetadata`: an optional dictionary representing metadata for the embedding
- `custom_id`: an optional string representing a user-defined ID for the embedding
No return value.

`DistanceStrategy`:
Defines different distance metrics for use in similarity search.

The code also defines a number of constants and imports various modules.

This code defines a VectorStore implementation using Postgres and pgvector. It includes functions for connecting to the database, creating tables and collections, and adding texts to the store. The `PGVector` class takes several inputs, including a connection string, an embedding function, a collection name, and a distance strategy. The code also defines several helper classes and functions, including `CollectionStore`, `EmbeddingStore`, `QueryResult`, and `DistanceStrategy`.

This code defines a VectorStore implementation using Postgres and pgvector. It includes classes for managing collections and embeddings, as well as a query result class and a distance strategy enum. The `PGVector` class takes several inputs, including a connection string, an embedding function, a collection name, and a distance strategy. The code also defines several helper classes and functions, including `CollectionStore`, `EmbeddingStore`, `QueryResult`, and `DistanceStrategy`. 

The `add_texts` function takes an iterable of strings to add to the vectorstore, along with optional metadata and vectorstore-specific parameters. It returns a list of IDs from adding the texts into the vectorstore.

The `similarity_search` function runs similarity search with PGVector with distance, taking a query text to search for, the number of results to return, and an optional filter by metadata. It returns a list of documents most similar to the query.

The `similarity_search_with_score` function returns docs most similar to the query, along with a score for each. It takes the same inputs as `similarity_search`.

The `similarity_search_with_score_by_vector` function is similar to `similarity_search_with_score`, but takes an embedding vector instead of a query text. It also takes an optional filter by metadata.

This code defines a VectorStore implementation using Postgres and pgvector. It includes classes for managing collections and embeddings, as well as a query result class and a distance strategy enum. The `PGVector` class takes several inputs, including a connection string, an embedding function, a collection name, and a distance strategy. The code also defines several helper classes and functions, including `CollectionStore`, `EmbeddingStore`, `QueryResult`, and `DistanceStrategy`. 

The `add_texts` function takes an iterable of strings to add to the vectorstore, along with optional metadata and vectorstore-specific parameters. It returns a list of IDs from adding the texts into the vectorstore.

The `similarity_search` function runs similarity search with PGVector with distance, taking a query text to search for, the number of results to return, and an optional filter by metadata. It returns a list of documents most similar to the query.

The `similarity_search_with_score` function returns docs most similar to the query, along with a score for each. It takes the same inputs as `similarity_search`.

The `similarity_search_with_score_by_vector` function is similar to `similarity_search_with_score`, but takes an embedding vector instead of a query text. It also takes an optional filter by metadata.

The `similarity_search_by_vector` function returns a list of documents most similar to an embedding vector, taking an embedding vector, the number of results to return, and an optional filter by metadata. It returns a list of Documents most similar to the query vector.

The `from_texts` and `from_documents` functions return a VectorStore initialized from texts and embeddings or documents and embeddings, respectively. They take several inputs, including the texts or documents to be added to the store, the embeddings to use, and optional parameters. They return a PGVector object.

# VectorStore Implementation using Postgres and pgvector

This code defines a VectorStore implementation using Postgres and pgvector. It includes classes for managing collections and embeddings, as well as a query result class and a distance strategy enum. 

## Functions

The code defines several helper classes and functions, including `CollectionStore`, `EmbeddingStore`, `QueryResult`, and `DistanceStrategy`. 

- `add_texts`: Takes an iterable of strings to add to the vectorstore, along with optional metadata and vectorstore-specific parameters. It returns a list of IDs from adding the texts into the vectorstore.

- `similarity_search`: Runs similarity search with PGVector with distance, taking a query text to search for, the number of results to return, and an optional filter by metadata. It returns a list of documents most similar to the query.

- `similarity_search_with_score`: Returns docs most similar to the query, along with a score for each. It takes the same inputs as `similarity_search`.

- `similarity_search_with_score_by_vector`: Similar to `similarity_search_with_score`, but takes an embedding vector instead of a query text. It also takes an optional filter by metadata.

- `similarity_search_by_vector`: Returns a list of documents most similar to an embedding vector, taking an embedding vector, the number of results to return, and an optional filter by metadata. It returns a list of Documents most similar to the query vector.

- `from_texts` and `from_documents`: Return a VectorStore initialized from texts and embeddings or documents and embeddings, respectively. They take several inputs, including the texts or documents to be added to the store, the embeddings to use, and optional parameters. They return a PGVector object.

# Inputs and outputs for each function

- `add_texts`:
    - Inputs: iterable of strings, optional metadata, vectorstore-specific parameters
    - Outputs: list of IDs
    
- `similarity_search`:
    - Inputs: query text, number of results to return, optional filter by metadata
    - Outputs: list of documents most similar to the query
    
- `similarity_search_with_score`:
    - Inputs: same as `similarity_search`
    - Outputs: list of documents most similar to the query, along with a score for each
    
- `similarity_search_with_score_by_vector`:
    - Inputs: embedding vector, number of results to return, optional filter by metadata
    - Outputs: list of documents most similar to the query vector, along with a score for each
    
- `similarity_search_by_vector`:
    - Inputs: embedding vector, number of results to return, optional filter by metadata
    - Outputs: list of documents most similar to the query vector
    
- `from_texts` and `from_documents`:
    - Inputs: texts or documents to be added to the store, embeddings to use, optional parameters
    - Outputs: PGVector object
    
- `connection_string_from_db_params`:
    - Inputs: driver, host, port, database, user, password
    - Outputs: connection string

