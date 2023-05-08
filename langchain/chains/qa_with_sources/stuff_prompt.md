This code is a Python script that defines a string variable called "template" for generating question-answering prompts. It imports a module called "PromptTemplate" from a package called "langchain". The prompt template includes a question, content, and sources, and is used to generate a final answer with references. Keywords for this code could include "prompt generation", "question-answering", and "string formatting".

This code block is not related to the previous conversation. Could you please provide me with a code snippet to summarize?

This code defines a string variable that includes a speech by the President of the United States calling on Congress to fund ARPA-H, an agency for health research. The speech also includes a call for unity and a reflection on the history and character of the United States. The code also includes a final answer that the President did not mention Michael Jackson. Keywords for this code could include "health research", "political speech", and "unity".

This code defines two classes called "PromptTemplate" and "EXAMPLE_PROMPT" for generating question-answering prompts. The "PromptTemplate" class takes a string template as input and generates a prompt with input variables. The "EXAMPLE_PROMPT" class is a specific example of a prompt template that includes a page content and source. The code also includes a question template that can be used with the "PromptTemplate" class. Keywords for this code could include "prompt generation", "question-answering", and "string formatting". 

## keywords
prompt generation, question-answering, string formatting

## classes
- PromptTemplate: generates a prompt with input variables based on a string template
- EXAMPLE_PROMPT: a specific example of a prompt template that includes page content and source

## functions/methods
N/A

## code examples of use
```python
template = """QUESTION: {question}
=========
{summaries}
=========
FINAL ANSWER:"""
PROMPT = PromptTemplate(template=template, input_variables=["summaries", "question"])

EXAMPLE_PROMPT = PromptTemplate(
    template="Content: {page_content}\nSource: {source}",
    input_variables=["page_content", "source"],
)
```

