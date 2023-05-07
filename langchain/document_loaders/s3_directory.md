from langchain.document_loaders.s3_directory import S3DirectoryLoader

# create an S3DirectoryLoader object with the bucket name and prefix
loader = S3DirectoryLoader(bucket="my-bucket", prefix="my-prefix/")

# load documents from the S3 directory
docs = loader.load()

# print the number of documents loaded
print(len(docs))


"""
Sure, I can help with that!

# Title
S3DirectoryLoader Class Summary

## Classes
- S3DirectoryLoader: A class that loads documents from an S3 directory.

## Functions/Methods
- __init__(self, bucket: str, prefix: str = ""): Initializes the class with the S3 bucket and prefix.
- load(self) -> List[Document]: Loads documents from the S3 bucket and returns them as a list of Document objects.

## Code Examples of Use
Here's an example of how you can use the S3DirectoryLoader class:


"""


