This code defines utility functions for parsing an OpenAPI spec. It includes an `HTTPVerb` enum for representing HTTP verbs, with methods for parsing HTTP verbs from strings. The code also imports several modules and classes from the `openapi_schema_pydantic` and `pydantic` libraries for working with OpenAPI specs.

This code defines an OpenAPI model called `OpenAPISpec` that removes misformatted parts of the spec. It includes several methods for getting specific components of the spec, such as paths, parameters, schemas, and request bodies. These methods also handle errors if the specified component is not found in the spec. There are also methods for getting referenced parameters, schemas, and request bodies, as well as their root references.

This code defines an OpenAPI model called `OpenAPISpec` that provides several methods for getting an OpenAPI spec from various sources, such as a dictionary, text, file path, or URL. It also includes methods for getting the base URL, valid HTTP methods for a specified path, and the operation object for a given path and HTTP method. Additionally, it includes a method for alerting if the OpenAPI spec is not supported and a method for parsing the OpenAPI spec object.

This code defines several methods for getting components of an OpenAPI spec for a given operation, such as parameters and request body. These methods also handle errors if the specified component is not found in the spec. Additionally, it includes a method for getting a cleaned operation id from an operation id by replacing all punctuation with underscores.

