# Summary
This code defines a class called `MyScale` which provides a wrapper around the MyScale vector database. The class includes several methods to add or retrieve documents from the vector store, and perform similarity searches with or without relevance scores. The `drop` method is used to drop data, and the `metadata_column` property returns the metadata column.

## Functions
- `__init__(self, embedding_function: Embeddings, config: MyScaleSettings, **kwargs: Any)`: Initializes the schema and creates a connection to MyScale.
- `escape_str(self, string: str) -> str`: Escapes special characters in a string.
- `add_texts(self, texts: Iterable[str], ids: Optional[Iterable] = None, batch_size: int = 32, metadatas: Optional[List[dict]] = None) -> None`: Adds documents to the vector store.
- `from_texts(cls, embedding: Embeddings, texts: Iterable[str], text_ids: Optional[Iterable] = None, batch_size: int = 32, metadatas: Optional[List[dict]] = None, **kwargs: Any) -> MyScale`: Adds documents to the vector store and returns a new instance of MyScale.
- `__repr__(self) -> str`: Returns a string to show connection info and data schema.
- `_build_qstr(self, q_emb: List[float], topk: int, where_str: Optional[str] = None) -> str`: Builds a query string for similarity search.
- `similarity_search(self, query: str, k: int = 4, where_str: Optional[str] = None, **kwargs: Any) -> List[Document]`: Performs a similarity search with MyScale.
- `similarity_search_by_vector(self, embedding: List[float], k: int = 4, where_str: Optional[str] = None, **kwargs: Any) -> List[Document]`: Performs a similarity search with MyScale by vectors.
- `similarity_search_with_relevance_scores(self, query: str, k: int = 4, where_str: Optional[str] = None, **kwargs: Any) -> List[Tuple[Document, float]]`: Performs a similarity search with MyScale with relevance scores.
- `drop(self) -> None`: Drops data.
- `metadata_column(self) -> str`: Returns the metadata column.

# Inputs and outputs for each function
Please refer to the function descriptions above for information on inputs and outputs.

This code defines a class called `Pinecone` which provides a wrapper around the Pinecone vector database. The class includes two methods: `add_texts` and `similarity_search_with_score`. The `add_texts` method adds documents to the vector store and returns a list of ids. The `similarity_search_with_score` method performs a similarity search with Pinecone and returns a list of tuples, each containing a document and its similarity score. The class also includes an `__init__` method which initializes the schema and creates a connection to Pinecone, and several optional arguments. The `__init__` method also checks if the Pinecone client is installed and if the index is an instance of `pinecone.index.Index`.

This code defines a class called `Pinecone` which provides a wrapper around the Pinecone vector database. The class includes two methods: `add_texts` and `similarity_search_with_score`. The `add_texts` method adds documents to the vector store and returns a list of ids. The `similarity_search_with_score` method performs a similarity search with Pinecone and returns a list of tuples, each containing a document and its similarity score. The class also includes an `__init__` method which initializes the schema and creates a connection to Pinecone, and several optional arguments. The `__init__` method also checks if the Pinecone client is installed and if the index is an instance of `pinecone.index.Index`.

This code defines a class called `Pinecone` which provides a wrapper around the Pinecone vector database. The class includes two methods: `add_texts` and `similarity_search_with_score`. The `add_texts` method adds documents to the vector store and returns a list of ids. The `similarity_search_with_score` method performs a similarity search with Pinecone and returns a list of tuples, each containing a document and its similarity score. The class also includes an `__init__` method which initializes the schema and creates a connection to Pinecone, and several optional arguments. The `__init__` method also checks if the Pinecone client is installed and if the index is an instance of `pinecone.index.Index`. Additionally, the code includes a method called `from_texts` which constructs a Pinecone wrapper from raw documents by embedding them and adding them to a provided Pinecone index. Finally, the code includes a method called `from_existing_index` which loads a Pinecone vectorstore from an index name. The `for` loop in the `add_texts` method iterates over batches of texts, creates embeddings for each batch, and upserts them to Pinecone. The `from_existing_index` method loads a Pinecone vectorstore from an index name.

