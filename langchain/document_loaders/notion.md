from langchain.document_loaders.notion_directory import NotionDirectoryLoader

# create a NotionDirectoryLoader object with the file path
loader = NotionDirectoryLoader(path="/path/to/notion/directory")

# load documents from the Notion directory
docs = loader.load()

# print the number of documents loaded
print(len(docs))


"""
Sure, I can help with that!

# Title
NotionDirectoryLoader Class Summary

## Classes
- NotionDirectoryLoader: A class that loads Notion directory dumps.

## Functions/Methods
- __init__(self, path: str): Initializes the class with the file path.
- load(self) -> List[Document]: Loads documents from the file path and returns them as a list of Document objects.

## Code Examples of Use
Here's an example of how you can use the NotionDirectoryLoader class:


"""


