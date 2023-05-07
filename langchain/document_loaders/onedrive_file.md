from langchain.document_loaders.onedrive import OneDriveFileLoader
from O365 import Account

# create an O365 account object
account = Account()

# authenticate with the account
credentials = ("username", "password")
account.authenticate(credentials)

# get the OneDrive drive object
drive = account.drive()

# get a file from the drive
file = drive.get_item("file_id")

# create a OneDriveFileLoader object with the file
loader = OneDriveFileLoader(file)

# load documents from the file
docs = loader.load()

# print the number of documents loaded
print(len(docs))


"""
Sure, I can help with that!

# Title
OneDriveFileLoader Class Summary

## Classes
- OneDriveFileLoader: A class that loads documents from a OneDrive file.

## Functions/Methods
- __init__(self, file: File): Initializes the class with a OneDrive file.
- load(self) -> List[Document]: Loads documents from the OneDrive file and returns them as a list of Document objects.

## Code Examples of Use
Here's an example of how you can use the OneDriveFileLoader class:


"""


