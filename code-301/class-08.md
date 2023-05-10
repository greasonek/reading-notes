# Reading Notes Class 08

## API Design Best Practices

> A well-designed app should support **platform independence** and **service evolution**

- *platform independence* - any client should be able to call the API which requires standard protocols and mechanism whereby the client and web service can agree on format of the data to exchange 

- *service evolution* - API should be able to evolve and add functionality independently from client apps, as API evolves existing client app should continue to function without needing modification

- REST = independent of underlying protocol and not necessarily tied to HTTP (but most use it as the app protocol);

- consistent naming conventions in URIs; use of plural nouns to reference collections

- organize collections and items in a hierarchy (ex, /customers is path to customer collection, /customers/5 is path to customer with ID of 5 (/customers/{id}))
  
  - *avoid resources for URIs more complex than collection/item/collection*

- POST - creates a resource - assigns URI to new resource and returns to client, frequently applied to collections

- PUT - creates resource OR updates a resource; client specifies URI for a resource, if it already exists then is replaced otherwise a new resource is created; frequently applied to individual items

- PATCH - performs partial update to existing resource

1. What does REST stand for?

- Representational State Transfer - an architectural style for building distributed systems based on hypermedia

2. REST APIs are designed around a resource (any object, data or service that can be accessed by the client)

3. What is an identifier of a resource? Give an example.

- A URI that uniquely identifies the source, it contains a scheme name, authority, path, query and fragment; ex)  "scheme" :// "authority" / "path" [?query][#fragment]; A URI for a particualr order on amazon would be something like https://www.amazon.com/gp/css/order-history?ie=UTF8

4. What are the most common HTTP verbs?

- GET, POST, PUT, PATCH, DELETE

5. What should the URIs be based on?

- nouns (the resource) *not the verb (operations on the resource)*

6. Give an example of a good URI.

- http://amazon.com/orders

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

- "chatty" web APIs expose a large number of small resources, the more requests on the web server the bigger the load - not a good thing

8. What status code does a successful GET request return?

- status 200 (OK)

9. What status code does an unsuccessful GET request return?

- status 404 (Not Found)

10. What status code does a successful POST request return?

- status 201 (Created)

11. What status code does a successful DELETE request return?

- status 204 (No Content)
