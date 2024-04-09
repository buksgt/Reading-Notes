# table of contents
## code 301 reading notes
## Class XX reading notes
### Reading Class 00XX, X APR

READING: https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

1. In your own words, describe what each group of status code represents:

100's (Informational Responses): These codes indicate that the server has received and is processing the request, but no response is available yet. It's like a preliminary response before the final response.

200's (Success Responses): This group signifies that the request was successfully received, understood, and processed. In simple terms, things went as planned.

300's (Redirection Messages): These codes tell the client that they need to perform additional actions to complete the request. This usually involves redirection to a different URL.

400's (Client Error Responses): This group indicates that there were problems with the request made by the client. It could be a bad request, unauthorized access, or forbidden actions, among others.

500's (Server Error Responses): These codes signify that the server failed to fulfill an apparently valid request. These are the problems on the server side.

2.  What is a status code 202?

This is a success status response code that indicates the request has been accepted for processing, but the processing has not been completed. It's often used for asynchronous processes.

3. What is a status code 308?

This is a redirection status code, specifically indicating "Permanent Redirect". It means that the resource requested has been definitively moved to the URL given by the Location headers, and future requests should use this new URL.

4. What code would you use if an update didn’t return data to a client?

The appropriate status code would l be 204 No Content.

5. What code would you use if a resource used to exist but no longer does?

Use 410 Gone. This code indicates that the resource requested is no longer available and will not be available again.

6. What is the ‘Forbidden’ status code?

This is 403 Forbidden. It means that the server understood the request but refuses to authorize it. 

 

VIDEO: https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw

 

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

It enhances security by keeping sensitive data like the database connection string out of the source code. This minimizes the risk of accidentally exposing it, especially when the code is shared or stored publicly. It increases flexibility by allowing different settings for various environments (like development, testing, production) without altering the codebase.

2. What is middleware?

Middleware in web development is a function that processes the request and response objects in a web application. It can execute code, modify the request and response, and pass control to the next middleware function.

3. What does app.use(express.json()) do?

It is an Express middleware function that parses incoming JSON requests and makes the parsed data available under the req.body property.

4. What does the /:id mean in a route?

/:id in a route is a placeholder for a dynamic value that represents a specific parameter, such as an ID. It allows the route to handle requests for specific resources based on the ID provided in the URL.

5. What is the difference between PUT and PATCH?

PUT is used for updating or replacing an entire resource. Fields not included in a PUT request are typically reset to their default values or omitted.

PATCH is used for partial updates to a resource. Only the fields specified in the request are updated, leaving others unchanged.

6. How do you make a default value in a schema?

When defining a schema, you can assign default values to specific fields, ensuring that if no value is provided for a field when a new record is created, it automatically gets filled with this predefined default.

7. What does a 500 error status code mean?

A 500 error indicates a general server error when the server encounters an unexpected condition that prevents it from fulfilling the request.

8. What is the difference between a status 200 and a status 201?

A status 200 indicates that a request has been successfully processed. A status 201 is used specifically when a new resource has been created in response to a request, often seen with POST requests.

# Things I want to know more about.