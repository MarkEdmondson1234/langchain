# heading
Bing Search API toolkit.

## functions
The code defines two tools for working with the Bing Search API: `BingSearchRun` and `BingSearchResults`. `BingSearchRun` allows you to query the Bing Search API and returns the search results as a string. `BingSearchResults` also queries the API but returns the search results as a JSON array. Both tools require setting environment variables for the Bing Search API and take in a search query string as input.

# Inputs and outputs for each function
Both `BingSearchRun` and `BingSearchResults` take in a search query string as input and require setting environment variables for the Bing Search API. `BingSearchRun` returns the search results as a string, while `BingSearchResults` returns the search results as a JSON array.

The code to summarise is below:
```python
"""Bing Search API toolkit."""

from langchain.tools.bing_search.tool import BingSearchResults, BingSearchRun

__all__ = ["BingSearchRun", "BingSearchResults"]
```

