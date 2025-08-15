**API**
- a set of rules or protocols that enables software applications to communicate with each other to exchange data, features and functionality.
- API communication in terms of a request and response between a client and server.
- application submitting the request is the client, and the server provides the response.
- API is the bridge establishing the connection between client and the server.

> have different type of method as shown below
>> GET → Retrieve data
>> POST → Create new data
>> PUT → Update entire data
>> PATCH → Update part of the data
>> DELETE → Remove data


**COMPONENTS OF API**
- Endpoints  : URLs that provide access to specific resources  or functionalities. 
- Methods/HTTP Verbs  : Actions that can be performed  (e.g., GET, POST, PUT, DELETE). 
- Requests  : Data sent by the client to the server. 
- Responses  : Data sent back by the server to the client. 
- Headers  : Metadata about the request or response (e.g.,  authentication tokens, content type). 
End to End API Testing, Curated by Lamhot Siagian 
- Payload/Body  : Data being sent with the request (typically in JSON or XML format).


**PROTOCOL**
- HTTP - hypertext transfer protocol
- HTTPS - hypertext transfer protocol secured (often used)


**HTTPS RESPONSE CODE**  
> Status code  
>> 100 Continue - The server has received the request headers and the client should continue to send the request body.

>> 200 OK - The request was successful, and the server returned the requested data.  
>> 201 Created - The request was successful, and a new resource was created.  
>> 204 No Content - The request was successful but there is no content to return.

>> 301 Moved Permanently - The resource has been permanently moved to a new URL.  
>> 302 Found - The resource is temporarily located at a different URL.

>> 400 Bad Request - The server could not understand the request due to invalid syntax.  
>> 401 Unauthorized - Authentication is required or credentials are invalid.  
>> 403 Forbidden - The client is authenticated but does not have permission to access the resource.  
>> 404 Not Found - The requested resource could not be found on the server.  
>> 405 Method Not Allowed - The HTTP method is not allowed for the resource.  
>> 409 Conflict - There is a conflict with the current state of the resource.

>> 500 Internal Server Error - The server encountered an unexpected error.  
>> 502 Bad Gateway - The server received an invalid response from an upstream server.  
>> 503 Service Unavailable - The server is currently unable to handle the request.


**POSTMAN**
- tools for testing API
- can use any protocal (need to configure)
- manually check endpoint or sending request (GET, POST, PUT, PATCH, DELETE)

> collection - a list of multiple request connecting to the same API
>> avoid configuration in our request ex: url (address), therefore make the address as a variable and save it into the correct collection
>> variables - initial values is this will be available to others if you share the collection
>> variables - current value is this is private to you and this is the value that Postman uses
> query parameter - usually add parameters for requesting specific data/response based on parameter have been set

Links: https://www.youtube.com/watch?v=VywxIQ2ZXw4