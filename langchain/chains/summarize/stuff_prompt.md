Title: Code for Generating Prompts for Language Models

Keywords: PromptTemplate, language models, summarization, document

Classes: 
- PromptTemplate: A class for generating prompts for language models.

Functions/Methods:
- load_summarize_chain: A function for loading a document summarization chain based on input parameters, including language model, chain type, and verbosity flag.
- _load_stuff_chain: A function for loading a StuffDocumentsChain instance for summarizing documents.
- _load_map_reduce_chain: A function for loading a MapReduceDocumentsChain instance for summarizing documents.
- _load_refine_chain: A function for loading a RefineDocumentsChain instance for summarizing documents.
- LoadingCallable: An interface for loading the combine documents chain.

Code Examples of Use: 
- To generate a prompt for summarizing a given text, use the PROMPT object from the PromptTemplate class:
```
prompt = PROMPT.generate_prompt({"text": "Lorem ipsum dolor sit amet."})
```
- To load a document summarization chain, use the load_summarize_chain function:
```
chain = load_summarize_chain(llm, chain_type="stuff", verbose=True)
```

