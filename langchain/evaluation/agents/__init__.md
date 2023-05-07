# heading
Chains for evaluating ReAct style agents.

## functions
The code defines a class called `TrajectoryEvalChain` for evaluating ReAct style agents. The class inherits from `Chain` and includes methods for parsing output, getting the agent trajectory, and running the evaluation chain.

# Inputs and outputs for each function
The `from_llm` method creates a new instance of the class using a specified `ChatOpenAI` instance, a sequence of `BaseTool` instances, and an optional `TrajectoryOutputParser`. The `input_keys` and `output_keys` properties specify the expected input and output keys for the evaluation chain. The `_call` method runs the evaluation chain with the specified inputs and returns a dictionary containing the score and reasoning (if `return_reasoning` is True).

The code imports the `TrajectoryEvalChain` class from the `langchain.evaluation.agents.trajectory_eval_chain` module and adds it to the `__all__` list.

