# APIs

## [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

APIs should be platform independant, any client should be able to call the API.

The API should be able to evolve without breaking client functionality.

REST stands for Representational State Transfer. REST over HTTP uses open standards and doesn't bind the implimentation of the API or client to any specific implementation.

- Rest APIs are designed around resources, any kind of object, data, or service that can be accessed by the client.
- Resource has an identifier, a URI that uniquely identifies that resource.
- Clients exchange representations of resources. i.e. JSON.
- REST APIs use a uniform interface, common operations are GET, POST, PUT, PATCH, and DELETE.
- Use stateless request model. One request shouldn't require transient data from another.

Focus on the business intities the API exposes.

Resource URIs should be based on nouns (The resources) not adjectives (the operations).

`/orders` = good

`/create-order` = bad

A client should not be exposed to internal implimentation. The API should work on the data, not the client.

Adopt a consistent nameing convention for URIs.

- `/customers` = a collection of customers
- `/customers/{ID}` = a single customer
- `/orders` = a collection of orders
- `/customers/{ID}/orders` = a collection of a single customers orders

Try to keep it simple though, so that future changes don't break your system. Try to avoid URIs more complex than `/collection/item/collection`.

Avoid chatty APIs that expose a lot of small resources. Strike a balance between sending more data with less calls, but not so much that the client ends up with data it won't use.

Avoid creating dependancies between API and the underlying data sources. API should be an abstraction of the data, not a direct representation.


### API Design Questions

1. **What does REST stand for? -** Representational State Transfer
2. **REST APIs are designed around a __. -** Resources like objects, data, or services.
3. **What is an identifier of a resource? Give an example. -** a URI, such as `/clients/2`
4. **What are the most common HTTP verbs? -** GET, POST, PUT, PATCH, and DELETE.
5. **What should the URIs be based on? -** Nouns (the resource)
6. **Give an example of a good URI. -** `/clients/2/orders`
7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? -** It's when you expose a lot of small resources and thus require many calls to the API. It can be bad because it can take up a lot of bandwidth and resources.
8. **What status code does a successful `GET` request return? -** 200 (OK)
9. **What status code does an unsuccessful `GET` request return? -** 404 (Not Found) or 204 (No Content)
10. **What status code does a successful `POST` request return? -** 201 (Created)
11. **What status code does a successful `DELETE` request return? -** 204 (No Content)

## Bookmark and Review

- [RegExr](https://regexr.com/) - Pay particular attention to the cheatsheet
- [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
- [Regex 101](https://regex101.com/)

## Things I Want To Learn More About

[Generating documentation from API Contracts](https://learn.microsoft.com/en-us/aspnet/core/tutorials/web-api-help-pages-using-swagger?view=aspnetcore-8.0)