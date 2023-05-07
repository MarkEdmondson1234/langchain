# A script for loading blobs from a file system
This script defines three classes: `BlobLoader`, `Blob`, and `FileSystemBlobLoader`. The `BlobLoader` class is an abstract base class that defines the interface for loading blobs. The `Blob` class represents a binary large object and has two attributes: `key` and `content`. The `FileSystemBlobLoader` class is a concrete implementation of the `BlobLoader` class that loads blobs from a file system. The script also imports the `FileSystemBlobLoader` and `Blob` modules and defines a list of public objects with the `__all__` variable.

