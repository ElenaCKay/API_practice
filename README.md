# APIs

APIs (Application Programming Interfaces) are sets of rules and protocols that allow different software applications to communicate and interact with each other. They define the methods and data formats that applications can use to request or exchange information. APIs provide a standardized way for developers to access certain functionalities or data from a service or platform without needing to understand the underlying implementation details.

APIs are used in various contexts, such as web development, mobile app development, and integration of different software systems. They enable developers to leverage existing functionalities, services, or data provided by other applications or platforms, without having to build everything from scratch. APIs can be used to retrieve data, submit data, perform operations, or even control hardware devices.

```commandline
+-------------------+                     +-------------------+
|   Client          |                     |   API Server      |
+-------------------+                     +-------------------+
        |                                          |
        |         HTTP Request                     |
        |----------------------------------------->|
        |                                          |
        |         HTTP Response                    |
        |<-----------------------------------------|
        |                                          |

```
In this diagram, the client initiates an HTTP request to the API server, specifying the desired action and any necessary parameters. The server processes the request and sends back an HTTP response containing the requested data or the result of the operation.

## Rest APIs

A REST API (Representational State Transfer API) is a type of API that follows a set of architectural principles and constraints. It is designed to be stateless, scalable, and interoperable. REST APIs are widely used in web development and adhere to the principles of the REST architectural style.

- Representational data flow - how is data transformed from one api to another both the client and the server can read the api. It can completely receive the resource Documentation of the resource contact. If the client doesn't not what to receive it might not be able to receive it. The client gets a head up as to what it will receive.
- URIs and naming - Like a url uniform resource indicator. You can use queries.
- Statelessness - Doesnt hold on to the previous request. Each request is individual. 
- Caching - Stores data that is used a lot inbetween the server and the client so it doesnt have to go back and forth a lot. Makes everything faster.

Some are open source and some are hidden behind a key and you need to register to get them. Some are paid for and some are private. 

Apps that use rest APIs:
Postman + insomnia

## HTTP

HTTP (Hypertext Transfer Protocol) is a protocol that defines how data is transferred over the web. It is the foundation of communication on the World Wide Web. HTTP defines the structure and semantics of requests made by clients (such as web browsers) and the responses returned by servers.

- HTTP stands for "Hypertext Transfer Protocol."
- It is primarily used for retrieving resources from web servers, such as HTML pages, images, videos, or other types of files.
- HTTPS (HTTP Secure) is an extension of HTTP that adds a layer of encryption using SSL/TLS protocols. It provides a secure connection between the client and the server, protecting the data exchanged from eavesdropping or tampering.

### HTTP Request structure:

```commandline
+--------------------------------------------------------+
|                         Request                        |
+--------------------------------------------------------+
|   Method   |           URI            |    HTTP Version   |
+--------------------------------------------------------+
|                          Headers                       |
+--------------------------------------------------------+
|                           Body                         |
+--------------------------------------------------------+

```

The method is the HTTP verb which indicated the action that should be performed:

- GET -> Retrieve or fetch data from a resource.
- POST -> Submit or send data to be processed or create a new resource.
- PUT -> Update or replace the entire representation of a resource.
- DELETE -> Delete or remove a specified resource.
- PATCH -> Make partial modifications or updates to a resource.