# Summary
The code is a utility that calls Jira. It includes several prompts for creating and querying Jira issues. The code uses the Pydantic library to define data models for the Jira API.

## Functions
The code includes several prompts for creating and querying Jira issues, including `JIRA_CATCH_ALL_PROMPT`, `JIRA_GET_ALL_PROJECTS_PROMPT`, `JIRA_ISSUE_CREATE_PROMPT`, and `JIRA_JQL_PROMPT`.

# Inputs and outputs for each function
- The prompts take various input parameters, such as project keys, issue types, and JQL queries.
- The prompts return information about Jira issues, such as issue keys, summaries, and descriptions.

# Summary
The code is a utility that calls Jira. It includes several prompts for creating and querying Jira issues. The code uses the Pydantic library to define data models for the Jira API.

## Functions
The code includes several prompts for creating and querying Jira issues, including `JIRA_CATCH_ALL_PROMPT`, `JIRA_GET_ALL_PROJECTS_PROMPT`, `JIRA_ISSUE_CREATE_PROMPT`, and `JIRA_JQL_PROMPT`.

# Inputs and outputs for each function
- The prompts take various input parameters, such as project keys, issue types, and JQL queries.
- The prompts return information about Jira issues, such as issue keys, summaries, and descriptions.

# Summary
The code defines a class called `JiraAPIWrapper` which provides methods for searching, creating, and listing Jira issues and projects. The class uses the Pydantic library to define data models for the Jira API.

## Functions
The `JiraAPIWrapper` class includes several methods for interacting with Jira, including `search`, `project`, `create`, `other`, and `run`.

# Inputs and outputs for each function
- The `search` method takes a JQL query string as input and returns a string with information about the matching Jira issues.
- The `project` method takes no inputs and returns a string with information about all Jira projects.
- The `create` method takes a JSON string with issue fields as input and returns a string with the new issue's key.
- The `other` method takes a Python expression as input and returns the result of executing that expression.
- The `run` method takes a mode string (one of `jql`, `get_projects`, `create_issue`, or `other`) and a query string as input and returns the result of calling the corresponding method.

