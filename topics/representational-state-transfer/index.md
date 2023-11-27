# Representational State Transfer (REST)

Representational State Transfer (REST) is an architectural style for building web services. REST and REST-like (a.k.a. RESTful) services are built on top of the HTTP protocol, and they use standard HTTP methods like GET, POST, PUT, and DELETE to interact with resources. REST is widely used for creating web services.

REST is based on the following principles…

Client-Server Architecture: The client and the server are separate components that communicate with each other through a standardized interface.

Stateless: Every request from the client to the server must contain all the necessary information required to complete the request. The server does not maintain any state about the client.

Cacheable: Responses from the server must be cacheable or non-cacheable, depending on the requirement.

Uniform Interface: A uniform interface should be used to interact with the resources. This interface should be simple, easy to understand, and consistent across all resources.

Layered System: The architecture should be designed in a layered manner, with each layer having a specific role to play. This allows for scalability, flexibility, and better separation of concerns.

RESTful web services typically use the following HTTP methods: GET to read a resource, PUT to write a a resource, PATCH to update a resource, DELETE to destroy a resource, and POST to send more-complex information.

REST uses HTTP status codes. For example, code 200 means a request was successful, and code 404 means a requested resource was not found.
