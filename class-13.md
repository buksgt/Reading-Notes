# table of contents
## code 301 reading notes
## Class 13 reading notes
### Reading Class 13, 10 APR

### Reading:

1. **Which HTTP method would you use to update a record through an API?**
   
   **PUT or PATCH**: To update a record through an API, you would typically use the HTTP methods PUT or PATCH. PUT is used when you're updating the entire resource, while PATCH is for partial updates.

2. **GET, PUT, PATCH, and DELETE**: In RESTful APIs, these methods often require an ID parameter to specify which resource you want to retrieve (GET), update (PUT/PATCH), or delete (DELETE). POST typically does not require an ID since it's used for creating new resources.

### Video:

1. **What’s the relationship between REST and CRUD?**
   
   **REST**, or Representational State Transfer, is an architectural style for creating networked applications, and it often uses HTTP methods to communicate. CRUD, which stands for Create, Read, Update, and Delete, are the four basic operations of persistent storage. In RESTful APIs, these CRUD operations are implemented using HTTP methods. The common mapping is: Create (CRUD) to POST (HTTP), Read to GET, Update to PUT/PATCH, and Delete to DELETE. This mapping provides a standard way to interact with resources (like database entries) over a network.

2. **If you had to describe the process of creating a RESTful API in 5 steps, what would they be?**
   
   - **Define the Data Model**: Outline the structure of the data, determining the resources (like users, products) and their attributes.
   - **Determine Resource Endpoints**: Establish the URLs (endpoints) for accessing each resource. These should be structured logically and predictably.
   - **Assign HTTP Methods to CRUD Operations**: Map CRUD functionalities to the appropriate HTTP methods for each endpoint (GET for read, POST for create, PUT/PATCH for update, DELETE for delete).
   - **Design Representation Formats**: Decide how the data will be represented (commonly in JSON or XML), including the structure of request and response bodies.
   - **Implement Statelessness and Error Handling**: Ensure the API is stateless, with each client request containing all necessary information, and implement comprehensive error handling for clear communication of issues like invalid requests or server errors.

# Things I want to know more about.