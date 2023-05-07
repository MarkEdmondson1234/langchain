# Summary
This code defines classes, methods, and variables for implementing an agent that can hold a conversation and use tools to look up information. It includes the `StructuredChatAgent` class, which extends the `Agent` class and is used for responding to structured chat prompts, and the `ConvoOutputParser` class, which extends the `AgentOutputParser` class and is used for parsing the output of a conversational chat agent. It also includes several variables containing text templates and instructions for formatting the output of the agent.

## Functions
- `StructuredChatAgent`: class that extends the `Agent` class and is used for responding to structured chat prompts.
- `ConvoOutputParser`: class that extends the `AgentOutputParser` class and is used for parsing the output of a conversational chat agent.

# Inputs and outputs for each function
- `StructuredChatAgent`: no inputs or outputs described.
- `ConvoOutputParser`: inputs: `text`. Outputs: `AgentAction` or `AgentFinish`.

The code defines several variables containing text templates and instructions for formatting the output of the agent.

# Summary
This code defines a class called `ConversationalChatAgent` that extends the `Agent` class and is used for holding a conversation and using tools to look up information. It includes several methods and variables for creating prompts, validating tools, and constructing scratchpads. 

## Functions
- `ConversationalChatAgent`: class that extends the `Agent` class and is used for holding a conversation and using tools to look up information.

# Inputs and outputs for each function
- `ConversationalChatAgent`: inputs: `llm`, `tools`, `callback_manager`, `output_parser`, `system_message`, `human_message`, `input_variables`. Outputs: `Agent`.

The code defines several methods and variables for creating prompts, validating tools, and constructing scratchpads.

