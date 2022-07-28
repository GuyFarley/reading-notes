# Code 401 - Class 34

## API Integration

### [Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)

**1. Explain the difference between a query string parameter and a path parameter.**

- A path parameter is a parameter that is placed after the base URL, to accept data that will point to a specific resource

- A query string parameter is placed after the `?` in the URL (after any path parameters) and consists of a key-value pair that sorts the data that gets returned

**2. What would our API URL with a path id parameter be given the following information:**

- **Domain: `http://our-site.com`**
- **`v3`**
- **model name: `stuff`**
- **id: `things`**
  - <http://our-site.com/v3/stuff/things>

**3. We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.**

- The "interface" for the API we created uses software such as Thunderclient or Postman to provide a place to input and receive the data that is being sent to/returned from our API. It's not a typical GUI, but rather a representation that allows us to see the data that gets sent back and forth

### [Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)

**1. Describe how you would use middleware to implement basic and bearer auth.**

- We would incorporate middleware that is dependent on the route being hit, and performs various functionality to authorize/authenticate a user.
  - Basic auth middleware would perform auth based on username and password only
  - Bearer auth middleware would require token authentication before allowing a user to access certain resources

**2. Describe the handshake necessary to implement OAuth.**

- Client info (including an ID and secret) are passed back and forth between a 3rd party (such as Google or GitHub). A token is obtained that is used by the server to authenticate the user for the resource they are trying to access.

**3. Describe how Role Based Access Control works to a non-technical friend.**

- Role based access is a process that requires a user to be authenticated, and then depending on their role in the organization, allows that user to access certain resources. For instance, and admin would have the ability to create, update, and delete records once logged in. But a sales rep may only have the ability to read and update.

[Back to Home](../README.md)
