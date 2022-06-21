# Code 401 - Class 07 - Bearer Authorization

## [Intro to JWT](https://jwt.io/introduction/)

### What is a JSON Web Token (JWT)?

- A compact, self-contained method for transmitting data securely between parties as a JSON object

### When should we use JSON Web Tokens?

- **Authorization** - Once user is logged in, each request they make to a server will include the JWT and will allow them access to any routes, services, resources that are permitted with that JWT

- **Information Exchange** - "Signed" JWT's can ensure authentication of a user, and that the information hasn't been tampered with upon transmittal

### Claims are expected in which structural component of a JWT?

- The **Payload**

## [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

### If I get a JWT and I can decode the payload, how can we call that secure?

- JWT's can be signed, encrypted, or both. Even if someone could read its contents, if they don't know they private key they cannot change the contents. If they were somehow able to, the receiver would reject the content since the signature doesn't match the one they originally sent.

### If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature

- The calculated hash of payload + secret

### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter

- The content and secret are encrypted and appended as a *signature*. If the content were to be changed at some point, the calculated signature would be different and would no longer match what was originally sent

## [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

### Why use JWT?

- To securely transfer information between any two bodies

### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend

- Because it is so compact, it allows for super fast transmission - which makes it highly usable. And since it is self-contained, it avoids the need to make multiple requests to a server (which saves time and money) - all info about the user is already contained in the token!

### What are the three components (the structure) of a JWT signature?

1. **Header** - JSON object that contains 2 properties: alg (algorithm) and typ (type of token)
2. **Payload** - JSON object that contains the claims (sub, name, admin)
3. **Signature** - base64 header + base64 payload + secret

[Back to Home](../README.md)
