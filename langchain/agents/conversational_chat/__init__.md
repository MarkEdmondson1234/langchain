# Summary
This code defines classes and methods for implementing an agent that can respond to structured chat prompts. It includes the `StructuredChatAgent` class, which extends the `Agent` class and is used for responding to structured chat prompts. The `create_prompt` method creates a prompt template that includes instructions for using the agent's tools and formatting the input. The `from_llm_and_tools` method constructs an agent from a language model and a list of tools.

## Functions
- `StructuredChatAgent`: class that extends the `Agent` class and is used for responding to structured chat prompts.
- `create_prompt`: method that creates a prompt template that includes instructions for using the agent's tools and formatting the input.
- `from_llm_and_tools`: method that constructs an agent from a language model and a list of tools.

# Inputs and outputs for each function
- `StructuredChatAgent`: no inputs or outputs described.
- `create_prompt`: inputs: `tools`, `prefix`, `suffix`, `format_instructions`, `input_variables`. Outputs: `BasePromptTemplate`.
- `from_llm_and_tools`: inputs: `llm`, `tools`, `callback_manager`, `output_parser`, `prefix`, `suffix`, `format_instructions`, `input_variables`. Outputs: `Agent`.

