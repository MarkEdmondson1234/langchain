# Summary
This code defines two classes, `ListOutputParser` and `CommaSeparatedListOutputParser`, both of which inherit from `BaseOutputParser` and include methods for parsing text output. 

## Functions
- `parse`: parses the output of an LLM call.
- `get_format_instructions`: returns format instructions for the parser.

# Inputs and outputs for each function
## parse
Inputs:
- `text`: a string representing the input text to be parsed.

Outputs:
- Returns a list of strings representing the parsed output.

## get_format_instructions
Inputs:
- None

Outputs:
- Returns a string representing the format instructions for the parser.

The `ListOutputParser` class defines an abstract method `parse` that must be implemented by any subclass. The `CommaSeparatedListOutputParser` class is a subclass of `ListOutputParser` and includes a specific implementation of the `parse` method that parses comma-separated lists. The `get_format_instructions` method returns format instructions for the parser.

