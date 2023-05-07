This code defines three functions for analyzing text using textstat and spacy. The `import_wandb` function imports the `wandb` package and raises an error if it is not installed. The `load_json_to_dict` function loads a json file to a dictionary. The `analyze_text` function analyzes text by computing complexity metrics and generating visualizations using spacy. The function takes in a text string, a boolean for whether to compute complexity metrics, a boolean for whether to generate visualizations, an spacy language model, and an output directory for saving the visualization files. The function returns a dictionary containing the complexity metrics and visualization files serialized in a wandb.Html element. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`.

# heading
This code defines a function called `construct_html_from_prompt_and_generation` which constructs an html element from a prompt and a generation.

## functions
The code defines only one function.

# Inputs and outputs for each function
The `construct_html_from_prompt_and_generation` function takes in two parameters: a prompt string and a generation string. The function returns an html element containing the formatted prompt and generation strings, with the prompt in black and the generation in green. The function uses the `wandb` package to construct the html element.

This code defines a class called `WandbCallbackHandler` which is a callback handler that logs to Weights and Biases. The class has two methods, `on_llm_start` and `on_llm_new_token`, which are called when the LLM (Language Model) starts and generates a new token, respectively. The class takes in several parameters such as `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, `complexity_metrics`, and `stream_logs`. The class initializes the callback handler and logs the response using the run.log() method to Weights and Biases. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`.

This code defines a class called `WandbCallbackHandler` which is a callback handler that logs to Weights and Biases. The class has several methods, including `on_llm_new_token`, `on_llm_end`, `on_llm_error`, `on_chain_start`, `on_chain_end`, and `on_tool_start`, which are called when the LLM (Language Model) starts and generates a new token, when the chain starts and ends running, and when the tool starts running, respectively. The class takes in several parameters such as `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, `complexity_metrics`, and `stream_logs`. The class initializes the callback handler and logs the response using the run.log() method to Weights and Biases. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`.

This code defines a class called `WandbCallbackHandler` which is a callback handler that logs to Weights and Biases. The class has several methods, including `on_llm_new_token`, `on_llm_end`, `on_llm_error`, `on_chain_start`, `on_chain_end`, `on_tool_start`, `on_tool_end`, `on_tool_error`, `on_text`, `on_agent_finish`, `on_agent_action`, and `_create_session_analysis_df`, which are called when the LLM (Language Model) starts and generates a new token, when the chain starts and ends running, when the tool starts and ends running, when the agent is ending, and when the agent starts an action, respectively. The class takes in several parameters such as `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, `complexity_metrics`, and `stream_logs`. The class initializes the callback handler and logs the response using the run.log() method to Weights and Biases. The class also creates a dataframe with all the information from the session. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`.

This code defines a class called `WandbCallbackHandler` which is a callback handler that logs to Weights and Biases. The class has several methods, including `on_llm_new_token`, `on_llm_end`, `on_llm_error`, `on_chain_start`, `on_chain_end`, `on_tool_start`, `on_tool_end`, `on_tool_error`, `on_text`, `on_agent_finish`, `on_agent_action`, and `_create_session_analysis_df`, which are called when the LLM (Language Model) starts and generates a new token, when the chain starts and ends running, when the tool starts and ends running, when the agent is ending, and when the agent starts an action, respectively. The class takes in several parameters such as `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, `complexity_metrics`, and `stream_logs`. The class initializes the callback handler and logs the response using the run.log() method to Weights and Biases. The class also creates a dataframe with all the information from the session. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`. 

The `flush_tracker` method flushes the tracker and resets the session. It takes in several optional parameters such as `langchain_asset`, `reset`, `finish`, `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, and `complexity_metrics`. It creates a table of action records and a table of session analysis, logs them to Weights and Biases, and saves them as an artifact.

# Heading
This code defines a class called `WandbCallbackHandler` which is a callback handler that logs to Weights and Biases. The class takes in several parameters such as `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, `complexity_metrics`, and `stream_logs`. The class has several methods, including `on_llm_new_token`, `on_llm_end`, `on_llm_error`, `on_chain_start`, `on_chain_end`, `on_tool_start`, `on_tool_end`, `on_tool_error`, `on_text`, `on_agent_finish`, `on_agent_action`, and `_create_session_analysis_df`, which are called when the LLM (Language Model) starts and generates a new token, when the chain starts and ends running, when the tool starts and ends running, when the agent is ending, and when the agent starts an action, respectively. The class initializes the callback handler and logs the response using the run.log() method to Weights and Biases. The class also creates a dataframe with all the information from the session. The code imports several packages and modules, including `tempfile`, `pathlib`, `typing`, `langchain.callbacks`, `langchain.schema`, and several utility functions from `langchain.callbacks.utils`.

## Functions
- `flush_tracker`: Flushes the tracker and resets the session. It takes in several optional parameters such as `langchain_asset`, `reset`, `finish`, `job_type`, `project`, `entity`, `tags`, `group`, `name`, `notes`, `visualize`, and `complexity_metrics`. It creates a table of action records and a table of session analysis, logs them to Weights and Biases, and saves them as an artifact.

# Inputs and Outputs for Each Function
## flush_tracker
### Inputs
- `langchain_asset`: The langchain asset to save.
- `reset`: Whether to reset the session.
- `finish`: Whether to finish the run.
- `job_type`: The job type.
- `project`: The project.
- `entity`: The entity.
- `tags`: The tags.
- `group`: The group.
- `name`: The name.
- `notes`: The notes.
- `visualize`: Whether to visualize.
- `complexity_metrics`: Whether to compute complexity metrics.

### Outputs
- None.

