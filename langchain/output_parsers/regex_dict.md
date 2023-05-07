# Summary
This code defines a class `RegexDictParser` that inherits from `BaseOutputParser` and includes a method for parsing text output into a dictionary using regular expressions.

## Functions
- `parse`: parses the output of an LLM call using regular expressions.

# Inputs and outputs for each function
## parse
Inputs:
- `text`: a string representing the input text to be parsed.

Outputs:
- Returns a dictionary representing the parsed output.

The `RegexDictParser` class includes a `regex_pattern` attribute that defines the regular expression pattern to be used for parsing the output. It also includes an `output_key_to_format` attribute that maps output keys to expected formats. The `parse` method uses the regular expression pattern and expected formats to extract values from the input text and return them as a dictionary. If there is no match for an output key or multiple matches are found, a `ValueError` is raised. If the value for an output key matches `no_update_value`, the key is skipped.

