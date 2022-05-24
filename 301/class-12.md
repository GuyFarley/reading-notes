# Code 301 - Class 12 - CRUD

## [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. **In your own words, describe what each group of status code represents:**

- **100’s** = Informational status codes regarding the server's reception of the request and its ability to comply (or not comply) for the full response
- **200’s** = Success codes, letting the client know that the request was accepted (though may not yet be processed)
- **300’s** = Redirection codes, letting the client know the request must be sent to a different location
- **400’s** = Client error codes, regarding invalid requests from a client to a server
- **500’s** = Server error codes, regarding errors on the server side

2. **What is a status code 202?** Confirms a request has met all validation requirements when sent from the client

3. **What is a status code 308?** Lets a client know the resource is no longer at that URL and the request must be sent to a different URL

4. **What code would you use if an update didn’t return data to a client?** 204 No Content

5. **What code would you use if a resource used to exist but no longer does?** 410 Gone

6. **What is the ‘Forbidden’ status code?** This lets the client know that although it is authorized to the backend, it still doesn't have permission to access the requested resource

## [Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. **Why do we need to pull our MongoDB database string out of our server and put it into our .env?** So our MongoDB address doesn't get uploaded to GitHub along with the rest of the files

2. **What is middleware?** Code that runs after your server gets a request, but before it gest passed to your route

3. **What does `app.use(express.json())` do?** Let's our server accept JSON format for data being sent

4. **What does the `/:id` mean in a route?** It means `:id` is a parameter, and we can access whatever is passed into this parameter using `request.params.id`

5. **What is the difference between `PUT` and `PATCH?`** `PUT` will update an entire resource, while `PATCH` will update only a portion of the resource

6. **How do you make a default value in a schema?** Use the property `default:` and provide a default value

7. **What does a `500` error status code mean?** This means there was an error on the server side, and had nothing to do with any errors on the client side

8. **What is the difference between a status `200` and a status `201`?** A 200 status code means a server request was received and is currently being processed, while a 201 status code means the request was successful and a resource was created

[Back to Home](../README.md)
