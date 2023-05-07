Title: Prompt Generation for Language Model Training

## Summary
This code defines several PromptTemplate classes used for generating prompts for language model training. The prompts include generating passages to answer questions, write counter arguments, and support/refute claims, among others.

## Keywords
prompt generation, language model training, question answering

## Classes
PromptTemplate - a class for generating prompts based on a given template and input variables.

## Functions/Methods
N/A

## Code Examples of Use
N/A

Title: Hypothetical Document Embeddings

## Summary
This code likely describes a research paper or article titled "Hypothetical Document Embeddings" published on arxiv.org. Unfortunately, without more information, it is difficult to provide a more detailed summary.

## Keywords
document embeddings, hypothetical data, natural language processing

## Classes
HypotheticalDocumentEmbedder - a class for generating hypothetical documents for a query and then embedding them.

## Functions/Methods
- embed_documents(texts: List[str]) -> List[List[float]]: Call the base embeddings.
- combine_embeddings(embeddings: List[List[float]]) -> List[float]: Combine embeddings into final embeddings.
- embed_query(text: str) -> List[float]: Generate a hypothetical document and embedded it.
- _call(inputs: Dict[str, Any], run_manager: Optional[CallbackManagerForChainRun] = None) -> Dict[str, str]: Call the internal LLM chain.
- from_llm(llm: BaseLanguageModel, base_embeddings: Embeddings, prompt_key: str, **kwargs: Any) -> HypotheticalDocumentEmbedder: Load and use LLMChain for a specific prompt key.

## Code Examples of Use
N/A

Title: Prompt Selector and Templates for Document Analysis

## Summary
This code defines several prompt templates for document analysis, including a prompt for answering questions and a prompt for generating a final answer from extracted parts of a long document and a question. It also includes a prompt selector that chooses the appropriate prompt based on the model being used.

## Keywords
document analysis, prompt templates, question answering

## Classes
ConditionalPromptSelector - a class for selecting a prompt based on a condition.
ChatPromptTemplate - a class for generating prompts for chat models.
HumanMessagePromptTemplate - a class for generating prompts for human messages.
SystemMessagePromptTemplate - a class for generating prompts for system messages.
PromptTemplate - a class for generating prompts based on a given template and input variables.

## Functions/Methods
N/A

## Code Examples of Use
N/A

This code defines several prompt templates for document analysis, including a prompt for answering questions and a prompt for generating a final answer from extracted parts of a long document and a question. It also includes a prompt selector that chooses the appropriate prompt based on the model being used. The code is organized into three sections, each with its own title, summary, keywords, classes, functions/methods, and code examples of use. The first section is titled "Prompt Generation for Language Model Training" and defines several PromptTemplate classes used for generating prompts for language model training. The second section is titled "Hypothetical Document Embeddings" and likely describes a research paper or article published on arxiv.org. The third section is titled "Prompt Selector and Templates for Document Analysis" and defines several prompt templates for document analysis, including a prompt for answering questions and a prompt for generating a final answer from extracted parts of a long document and a question. It also includes a prompt selector that chooses the appropriate prompt based on the model being used.

This code defines a prompt selector for document analysis, which includes a prompt for answering questions and a prompt for generating a final answer from extracted parts of a long document and a question. The code also includes a prompt selector that chooses the appropriate prompt based on the model being used. The code has a section for each of the three main topics: Prompt Generation for Language Model Training, Hypothetical Document Embeddings, and Prompt Selector and Templates for Document Analysis. Each section includes a title, summary, keywords, classes, functions/methods, and code examples of use. The specific code you provided defines a ConditionalPromptSelector with a default prompt and conditionals based on whether the model is a chat model or not.

