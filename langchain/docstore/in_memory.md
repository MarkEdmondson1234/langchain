# Script Purpose
This code defines a class `InMemoryDocstore` that provides a simple in-memory document store in the form of a dictionary. The `InMemoryDocstore` class includes a `search` method that takes a search string and returns either a string representing the summary of a document or a `Document` object representing the full text of the document. If the document does not exist, the `search` method returns an error message. The `InMemoryDocstore` class also includes an `add` method that takes a dictionary of document names and `Document` objects and adds them to the document store. If any of the document names already exist in the store, the `add` method raises a `ValueError`. 

## Functions
There are two functions defined in this code: `add` and `search`. The `add` function adds new documents to the document store, while the `search` function searches for documents in the store.

# Inputs and Outputs
The `add` function takes a dictionary of document names and `Document` objects as input and does not return any output. The `search` function takes a search string as input and returns either a string representing the summary of a document or a `Document` object representing the full text of the document. If the document does not exist, the `search` function returns an error message.

