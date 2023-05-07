from langchain.document_loaders.web_gitbook import GitbookLoader

# create a GitbookLoader object with the web page and whether to load all paths
loader = GitbookLoader(web_page="https://example.gitbook.io/docs", load_all_paths=True)

# load documents from the GitBook page or all paths in the navbar
docs = loader.load()

# print the number of documents loaded
print(len(docs))


"""
Sure, I can help with that!

# Title
GitbookLoader Class Summary

## Classes
- GitbookLoader: A class that loads GitBook data.

## Functions/Methods
- __init__(self, web_page: str, load_all_paths: bool = False, base_url: Optional[str] = None, content_selector: str = "main"): Initializes the class with the web page, whether to load all paths, base URL, and content selector.
- load(self) -> List[Document]: Fetches text from a single GitBook page or loads all (relative) paths in the navbar and returns them as a list of Document objects.
- _get_document(self, soup: Any, custom_url: Optional[str] = None) -> Optional[Document]: Fetches content from a page and returns a Document object.
- _get_paths(self, soup: Any) -> List[str]: Fetches all relative paths in the navbar.

## Code Examples of Use
Here's an example of how you can use the GitbookLoader class:


"""


