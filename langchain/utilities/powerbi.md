# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes a `PowerBIWrapper` class that has several methods for querying the Power BI API. The `get_reports` method returns a list of reports in a workspace, the `get_report` method returns a specific report in a workspace, and the `get_report_embed_token` method returns an embed token for a specific report. The `validate_environment` method is used to validate that the required environment variables are set.

# Inputs and outputs for each function
The `get_reports` method takes a workspace ID as input and returns a list of dictionaries with metadata about each report, including the report ID and name.

The `get_report` method takes a workspace ID and report ID as input and returns a dictionary with metadata about the report, including the report name and URL.

The `get_report_embed_token` method takes a workspace ID, report ID, and user ID as input and returns an embed token for the report.

To use the script, you need to set the `POWERBI_BASE_URL` environment variable to the base URL of the Power BI API and provide valid credentials. The `validate_environment` method is used to validate that the required environment variables are set.

# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes a `PowerBIDataset` class that has several methods for querying the Power BI API. The `get_table_names` method returns a list of tables available, the `get_schemas` method returns the available schema's, and the `table_info` method returns information about all tables in the database. 

# Inputs and outputs for each function
The `get_table_names` method takes no input and returns a list of strings with the names of the tables available. 

The `get_schemas` method takes no input and returns a string with the available schema's.

The `table_info` method takes no input and returns a string with information about all tables in the database. 

To use the script, you need to set the `POWERBI_BASE_URL` environment variable to the base URL of the Power BI API and provide valid credentials.

# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes several methods for querying the Power BI API related to getting information about tables in a dataset. The `get_table_info` method returns information about specified tables, the `agetable_info` method returns information about specified tables asynchronously, the `_get_tables_todo` method returns the tables that still need to be queried, the `_get_schema_for_tables` method creates a string of the table schemas for the supplied tables, and the `run` method executes a DAX command and returns a JSON representing the results.

# Inputs and outputs for each function
The `get_table_info` method takes an optional list of table names as input and returns a string with information about the specified tables. 

The `agetable_info` method takes an optional list of table names as input and returns a string with information about the specified tables asynchronously. 

The `_get_tables_todo` method takes a list of table names as input and returns a list of strings with the names of the tables that still need to be queried. 

The `_get_schema_for_tables` method takes a list of table names as input and returns a string with the available schema's for the supplied tables. 

The `run` method takes a DAX command as input and returns a JSON representing the results.

To use the script, you need to set the `POWERBI_BASE_URL` environment variable to the base URL of the Power BI API and provide valid credentials.

# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes several methods for querying the Power BI API related to getting information about tables in a dataset. The `get_table_info` method returns information about specified tables, the `agetable_info` method returns information about specified tables asynchronously, the `_get_tables_todo` method returns the tables that still need to be queried, the `_get_schema_for_tables` method creates a string of the table schemas for the supplied tables, the `run` method executes a DAX command and returns a JSON representing the results, and the `arun` method executes a DAX command and returns a result asynchronously.

# Inputs and outputs for each function
The `get_table_info` method takes an optional list of table names as input and returns a string with information about the specified tables. 

The `agetable_info` method takes an optional list of table names as input and returns a string with information about the specified tables asynchronously. 

The `_get_tables_todo` method takes a list of table names as input and returns a list of strings with the names of the tables that still need to be queried. 

The `_get_schema_for_tables` method takes a list of table names as input and returns a string with the available schema's for the supplied tables. 

The `run` method takes a DAX command as input and returns a JSON representing the results.

The `arun` method takes a DAX command as input and returns a result asynchronously.

To use the script, you need to set the `POWERBI_BASE_URL` environment variable to the base URL of the Power BI API and provide valid credentials.

# Summary
This code defines a utility script that provides a wrapper around a Power BI endpoint. The purpose of the script is to enable querying the Power BI API and parsing the results.

## Functions
The script includes several methods for querying the Power BI API related to getting information about tables in a dataset. The `get_table_info` method returns information about specified tables, the `agetable_info` method returns information about specified tables asynchronously, the `_get_tables_todo` method returns the tables that still need to be queried, the `_get_schema_for_tables` method creates a string of the table schemas for the supplied tables, the `run` method executes a DAX command and returns a JSON representing the results, and the `arun` method executes a DAX command and returns a result asynchronously. The `json_to_md` function converts a JSON object to a markdown table.

# Inputs and outputs for each function
The `get_table_info` method takes an optional list of table names as input and returns a string with information about the specified tables. 

The `agetable_info` method takes an optional list of table names as input and returns a string with information about the specified tables asynchronously. 

The `_get_tables_todo` method takes a list of table names as input and returns a list of strings with the names of the tables that still need to be queried. 

The `_get_schema_for_tables` method takes a list of table names as input and returns a string with the available schema's for the supplied tables. 

The `run` method takes a DAX command as input and returns a JSON representing the results.

The `arun` method takes a DAX command as input and returns a result asynchronously.

The `json_to_md` function takes a list of dictionaries with JSON contents and an optional table name as input and returns a string with a markdown table.

