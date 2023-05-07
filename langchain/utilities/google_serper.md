# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes several methods for querying the Power BI API related to getting information about tables in a dataset. The `get_table_info` method returns information about specified tables, the `agetable_info` method returns information about specified tables asynchronously, the `_get_tables_todo` method returns the tables that still need to be queried, the `_get_schema_for_tables` method creates a string of the table schemas for the supplied tables, the `run` method executes a DAX command and returns a JSON representing the results, and the `arun` method executes a DAX command and returns a result asynchronously. The `json_to_md` function converts a JSON object to a markdown table.

The code also includes a utility script that calls Google Search using the Serper.dev API.

# Inputs and outputs for each function
For the Power BI API utility script:
- The `get_table_info` method takes an optional list of table names as input and returns a string with information about the specified tables.
- The `agetable_info` method takes an optional list of table names as input and returns a string with information about the specified tables asynchronously.
- The `_get_tables_todo` method takes a list of table names as input and returns a list of strings with the names of the tables that still need to be queried.
- The `_get_schema_for_tables` method takes a list of table names as input and returns a string with the available schema's for the supplied tables.
- The `run` method takes a DAX command as input and returns a JSON representing the results.
- The `arun` method takes a DAX command as input and returns a result asynchronously.
- The `json_to_md` function takes a list of dictionaries with JSON contents and an optional table name as input and returns a string with a markdown table.

For the Google Search utility script:
- The script calls Google Search using the Serper.dev API and returns the search results.

Please note that the inputs and outputs for each function are further described in the code.

# Summary
This code defines a utility script that provides a wrapper around the Serper.dev Google Search API. The purpose of the script is to enable querying the Google Search API and parsing the results.

## Functions
The script includes several methods for querying the Google Search API related to getting search results. The `results` method runs a query through GoogleSearch and returns the results as a dictionary. The `run` method runs a query through GoogleSearch and parses the results. The `aresults` method runs a query through GoogleSearch asynchronously and returns the results as a dictionary. The `arun` method runs a query through GoogleSearch asynchronously and parses the results. The `_parse_results` method is a helper method that parses the results returned by the GoogleSearch API.

# Inputs and outputs for each function
- The `results` method takes a query string as input and returns a dictionary with the search results.
- The `run` method takes a query string as input and returns a string with the parsed search results.
- The `aresults` method takes a query string as input and returns a dictionary with the search results asynchronously.
- The `arun` method takes a query string as input and returns a string with the parsed search results asynchronously.

Please note that the inputs and outputs for each function are further described in the code.

# Summary
This code defines a utility script that provides a wrapper around the Serper.dev Google Search API. The purpose of the script is to enable querying the Google Search API and parsing the results.

## Functions
The script includes several methods for querying the Google Search API related to getting search results. The `results` method runs a query through GoogleSearch and returns the results as a dictionary. The `run` method runs a query through GoogleSearch and parses the results. The `aresults` method runs a query through GoogleSearch asynchronously and returns the results as a dictionary. The `arun` method runs a query through GoogleSearch asynchronously and parses the results. The `_parse_results` method is a helper method that parses the results returned by the GoogleSearch API.

# Inputs and outputs for each function
- The `results` method takes a query string as input and returns a dictionary with the search results.
- The `run` method takes a query string as input and returns a string with the parsed search results.
- The `aresults` method takes a query string as input and returns a dictionary with the search results asynchronously.
- The `arun` method takes a query string as input and returns a string with the parsed search results asynchronously.

Please note that the inputs and outputs for each function are further described in the code.

