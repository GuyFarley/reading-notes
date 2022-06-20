# Code 401 - Class 06 - Authentication

## [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

### Explain to a non-technical friend how you would safely hash and store a password

- Passwords are passed through cryptographic *hashing* algorithms, which store the passwords in a different format than plain text. This prevents the passwords from being easily cracked if stolen

### What is Bcrypt?

- A hash algorithm that makes use of **Key Stretching**, which is a method used to increase the time and resources needed to test each possible key

### Why might you use something like Bcrypt?

- This method is solid enough to protect users' passwords and data stored in most web applications

## [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

### What is Basic Authentication?

- From [Wikipedia](https://en.wikipedia.org/wiki/Basic_access_authentication):

> Basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

### What properties are necessary in the header of a Basic Auth request?

- The request must contain a header field in the form of `Authorization: Basic <credentials>`, where credentials is the Base64 encoding of ID and password joined by a single colon `:`.

### How are username:password in Basic Auth encoded?

- Using a variant of *Base64*, which (according to [Wikipedia](https://en.wikipedia.org/wiki/Base64)) is:

> ...a group of binary-to-text encoding schemes that represent binary data (more specifically, a sequence of 8-bit bytes) in sequences of 24 bits that can be represented by four 6-bit Base64 digits.

## [OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

### Define the authentication process to a non-technical recruiter

- Authentication is simply the process used to verify that an entity (person or website) is who it claims to be when requesting information online.

### How should your error messaging respond (both HTTP and HTML)? Why?

- Error messages should respond generically (not specifically), otherwise the messages can be used by bad actors to obtain information you did not intend to provide them (user ID and password enumeration)

### Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle

[Back to Home](../README.md)
