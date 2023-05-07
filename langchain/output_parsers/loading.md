# Summary
This code defines a function `load_output_parser` that loads an output parser based on the configuration provided. The function imports the `RegexParser` class from the `langchain.output_parsers.regex` module. 

## Functions
- `load_output_parser`: loads an output parser based on the configuration provided. It takes a dictionary `config` as input and returns a dictionary with the output parser loaded.

# Inputs and outputs for each function
## load_output_parser
Inputs:
- `config`: a dictionary containing the configuration for the output parser. 

Outputs:
- Returns a dictionary with the output parser loaded.

The `load_output_parser` function imports the `RegexParser` class from the `langchain.output_parsers.regex` module. It then checks if the `config` dictionary contains an `output_parsers` key. If it does, it checks if the value is not `None`. If it is not `None`, it extracts the `_type` key from the `_config` dictionary and checks if it is equal to `"regex_parser"`. If it is, it creates an instance of the `RegexParser` class with the remaining keys in `_config` and sets the `config["output_parsers"]` key to the created instance. If the `_type` key is not equal to `"regex_parser"`, it raises a `ValueError` with a message indicating that the output parser type is not supported. Finally, the function returns the `config` dictionary with the output parser loaded.

