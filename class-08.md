# table of contents
## code 301 reading notes
## Clas 08 reading notes
### Reading Class 008, 3 APR

APIs
Based on this article: https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-designLinks to an external site.
          
What does REST stand for?

REST stands for Representational State Transfer.

 

REST APIs are designed around a ____.

REST APIs are designed around a resource.

 

What is an identifier of a resource? Give an example.

An identifier of a resource is a URI that uniquely identifies that resource. Example: https://api.example.com/orders/1.

 

What are the most common HTTP verbs?

The most common HTTP verbs are GET, POST, PUT, PATCH, and DELETE.

 

What should the URIs be based on?

URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

 

Give an example of a good URI.

Example of a good URI: https://api.example.com/orders.

 

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

A 'chatty' web API involves frequent small requests and responses. It's usually considered a bad thing due to the increased load on the network.

 

What status code does a successful GET request return?

A successful GET request returns status code 200.

 

What status code does an unsuccessful GET request return? 

An unsuccessful GET request might return a status code like 404 (Not Found).

 

What status code does a successful POST request return?

A successful POST request typically returns status code 201.

 

What status code does a successful DELETE request return?

A successful DELETE request returns status code 204.

## Things I want to know more about.