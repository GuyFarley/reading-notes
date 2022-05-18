# Code 301 - Class 08 - APIs

## [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. **What does REST stand for?** Representational State Transfer

2. **REST APIs are designed around a *Resource*.** A resource is any kind of object, data, or service that a client can access

3. **What is an identifier of a resource? Give an example.** A URI uniquely identifies a resource. Example:

```
https://adventure-works.com/orders/1
```

4. **What are the most common HTTP verbs?** GET, POST, PUT, PATCH, and DELETE

5. **What should the URIs be based on?** Nouns (not verbs)

6. **Give an example of a good URI.**

```
https://adventure-works.com/orders
```

7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?** A 'chatty' API expose a large number of small resources, which might require a client to make several requests before receiving all the data it needs. This is a bad thing, and should be avoided in favor of an API that combines related info into a single resource that can be retrieved with a single request

8. **What status code does a successful GET request return?** 200 (OK)

9. **What status code does an unsuccessful GET request return?** 404 (Not Found)

10. **What status code does a successful POST request return?** 201 (Created)

11. **What status code does a successful DELETE request return?** 204 (No Content)

[Back to Home](../README.md)
