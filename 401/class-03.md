# Code 401 - Class 03 - Express REST API

## [Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

### Classes are a template for creating

- Objects

### Can a class declaration be hoisted?

- No. The class itself is hoisted but it's values are not initialized

### How would you describe a constructor and contextual “this” to a non-technical friend?

- A **constructor** is used to create an object based on the class it is in. The constructor uses the word **"this"** before each property, to indicate that it's creating a property for the specific object it is creating

## [Using Express Routing](https://expressjs.com/en/guide/routing.html)

### Within Express, what does routing refer to?

- It refers to how the endpoints of an application respond to requests from the client

### What is the difference between a route path and a route method?

- A **route path** is the endpoint at which a request can be made
- A **route method** is a method that corresponds to one of the HTTP methods (GET, POST, PUT, DELETE) and is attached to an instance (a singleton) of the **express** class

### When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

- **next** should be added as a parameter when it's necessary to pass control to another callback function. In order to use this parameter, you must include a **next()** statement in your code block

## [Express Routing](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4)

### What is an Express Router?

- It's a stripped-down express application that only contains what is needed to handle routes

### By what mean do we initialize express.Router() in an express server?

- we call an instance of router: `const router = express.Router();`

### What do we use route middleware for?

- We use it to do something before a request is processed (such as checking authentication or logging data)

[Back to Home](../README.md)
