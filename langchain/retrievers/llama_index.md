This code defines two classes called `LlamaIndexRetriever` and `LlamaIndexGraphRetriever`, both of which are subclasses of `BaseRetriever` and `BaseModel`. 

- `LlamaIndexRetriever`: This class is used for question-answering with sources over an LlamaIndex data structure. It has two attributes including `index` and `query_kwargs`. The class also has two methods including `get_relevant_documents` and `aget_relevant_documents`. 

- `LlamaIndexGraphRetriever`: This class is used for question-answering with sources over an LlamaIndex graph data structure. It has two attributes including `graph` and `query_configs`. The class also has two methods including `get_relevant_documents` and `aget_relevant_documents`. 

Both classes have a `get_relevant_documents` method that inputs a string query and outputs a list of `Document` objects containing the page content and metadata from the response. The `aget_relevant_documents` method is not implemented for either class.

