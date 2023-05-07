# heading
Tools for interacting with a Power BI dataset.

## functions
The code does not define any functions.

# Inputs and outputs for each function
N/A

The code provides tools for working with Power BI datasets, including a callback manager, a language model chain, and a base tool. It also includes several prompts for working with DAX queries and provides utilities for converting JSON to markdown.

This code defines a tool for querying a Power BI dataset using DAX queries. The tool takes in a DAX query as input and returns the query result from the dataset. If the query is incorrect, an error message will be returned. The code also defines a cache to store previous query results and includes methods for checking the cache and executing the query. The tool includes two methods for running the query, a synchronous method and an asynchronous method. The code also includes several response messages for common errors and issues that may arise when working with Power BI datasets.

# heading
Tools for interacting with a Power BI dataset.

## functions
The code defines two classes for interacting with Power BI datasets: InfoPowerBITool and ListPowerBITool.

# Inputs and outputs for each function
InfoPowerBITool:
- Input: A comma-separated list of tables in the dataset.
- Output: The schema and sample rows for the specified tables.

ListPowerBITool:
- Input: An empty string.
- Output: A comma-separated list of tables in the dataset.

Both functions use the PowerBIDataset class to interact with the dataset. The functions are defined as subclasses of the BaseTool class and include methods for running the tool synchronously and asynchronously. The code also includes several response messages for common errors and issues that may arise when working with Power BI datasets.

This code defines a tool for using an LLM to parse a question into a DAX query for a Power BI dataset. The tool takes in a fully formed question related to the dataset as input and returns the DAX query. The code also includes a cache to store previous queries and includes methods for checking the cache and executing the query. The tool includes two methods for running the query, a synchronous method and an asynchronous method. The code also includes several response messages for common errors and issues that may arise when working with Power BI datasets.

