# Fake Embeddings
This code defines a class `FakeEmbeddings` that is a subclass of `Embeddings` and `BaseModel`. The class includes methods for embedding documents and queries using a randomly generated embedding of a specified size. 

## Functions
- `_get_embedding`: returns a list of floats representing a randomly generated embedding of a specified size.
- `embed_documents`: takes a list of strings and returns a list of lists of floats representing the embeddings of each document.
- `embed_query`: takes a string and returns a list of floats representing the embedding of the query.

# Inputs and outputs for each function
- `_get_embedding`: no inputs, returns a list of floats.
- `embed_documents`: takes a list of strings as input, returns a list of lists of floats.
- `embed_query`: takes a string as input, returns a list of floats.

