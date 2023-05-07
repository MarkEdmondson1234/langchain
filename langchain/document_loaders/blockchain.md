from langchain.document_loaders.blockchain import BlockchainType

# use the ETH_MAINNET blockchain type
blockchain_type = BlockchainType.ETH_MAINNET


"""
Sure, I can help you with that!

# Title
BlockchainType Class Summary

## Classes
- BlockchainType: An enumeration class that defines the supported blockchain types.

## Functions/Methods
None

## Code Examples of Use
Here's an example of how you can use the BlockchainType enumeration:


"""


This code defines a class called BlockchainDocumentLoader that loads elements from a blockchain smart contract into Langchain documents. The supported blockchains are Ethereum mainnet, Ethereum Goerli testnet, Polygon mainnet, and Polygon Mumbai testnet. If no BlockchainType is specified, the default is Ethereum mainnet. The Loader uses the Alchemy API to interact with the blockchain, and the ALCHEMY_API_KEY environment variable must be set to use this loader. The API returns 100 NFTs per request and can be paginated using the startToken parameter. If get_all_tokens is set to True, the loader will get all tokens on the contract. The max_execution_time (sec) can be set to limit the execution time of the loader. The class has a load() method that returns a list of Document objects. The method makes API calls to get the NFTs from the contract and creates Document objects with the returned data. The class has no other methods or functions.

This code defines a method called _get_next_tokenId() that adds one to the tokenId and ensures the correct tokenId format is used. The method takes a tokenId string as input and returns a string with the next tokenId. The method first detects the value type of the tokenId using the _detect_value_type() method. Then, it converts the tokenId to an integer and adds one to it. Finally, it formats the result as a string with the correct tokenId format and returns it. The _detect_value_type() method is a static method that detects the value type of the tokenId and returns a string with the value type. The method takes a tokenId string as input and returns a string with the value type. The code has no classes or code examples of use.

