# Readings: Express

### 1. What’s the difference between PUT and PATCH?

PUT - updates entire resource

PATCH - updates part of resource

### 2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

[Mocki](https://github.com/adalyte/mocki)
[Postman](https://www.postman.com/)
[Swagger](https://swagger.io/)

### 3. Compare and contrast Swagger and APIDocjs. Which HTTP status codes should be sent with each type of (un)successful API call?

'200': description: OK
'400': description: Bad request. User ID must be an integer and larger than 0.
'401': description: Authorization information is missing or invalid.
'404': description: A user with the specified ID was not found.
'5XX': description: Unexpected error.

source: https://swagger.io/docs/specification/describing-responses/

### 4. Compare and contrast SOAP and ReST

ReST stands for Representationl State Transfer. It is a set of architectural principles first decribed by Roy Fielding in 2000. It descrbes an API for communication between web applications. A ReSTful application meets these six guidelines:

```plaintext
1. A client-server architecture composed of clients, servers, and resources.
2. Stateless client-server communication, meaning no client content is stored on the server between requests. Information about the session’s state is instead held with the client.
3. Cacheable data to eliminate the need for some client-server interactions.
4. A uniform interface between components so that information is transferred in a standardized form instead of specific to an application’s needs. This is described by Roy Fielding, the originator of REST, as "the central feature that distinguishes the REST architectural style from other network-based styles."
5. A layered system constraint, where client-server interactions can be mediated by hierarchical layers.
6. Code on demand, allowing servers to extend the functionality of a client by transferring executable code (though also reducing visibility, making this an optional guideline).
```

SOAP, or Simple Object Access Protocol, is an official standardized protocol that defines an API for communication bewteen web applications. It predates ReST, and it's standardized approach is less flexible and slower.

source: https://www.redhat.com/en/topics/integration/whats-the-difference-between-soap-rest

### Document the following Vocabulary Terms

#### Web Server

Software and hardware that accepts and responds to HTTP requests

#### Express

Node.js web application framework for building web applications

#### Routing

Routing is how a web API matches a URI to an action.

#### WRRC

The Web Request/ Response Cycle
