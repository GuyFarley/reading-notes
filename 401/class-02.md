# Code 401 - Class 02 - Express, NPM, TDD, CI/CD

## [An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

### Explain middleware, answer as though I were a non-technical recruiter

- Middleware is software that is designed to work with a whole host of web development data, to help solve problems. As it relates to Node and Express, middleware can be added to the request "pipeline" to handle data moving between the front end and back end.

### Express the most popular

- Node web framework

### Express is “unopinionated.” What does that mean?

- This means it is a framework that has fewer restrictions regarding which components can be pieced together to achieve a goal, or the best way to piece them together.

### What is a module and why is modularity useful to us as developers?

- A module is just a separate JS file that can be imported into other code as needed. Modularity is useful because it allows us to organize our code in manageable pieces.

## [What is NPM?](https://docs.npmjs.com/about-npm)

### What version of npm are you running on your machine?

- 8.5.0

### What command would you type to install a library/package called ‘jshint’ into your node project?

- `npm i jshint`

## [What is TDD?](https://www.agilealliance.org/glossary/tdd/)

### Explain why tests are important. Please explain as though I were your non technical elder

- Tests are important to ensure quality control of code being shipped, and to reduce the amount of time and work needed to fix errors retroactively. Testing has been shown to greatly reduce defect rates while only requiring a minimal increase in initial development time and energy

### What are three expected benefits of testing

1. Significant reduction in defect rates
2. Much less effort needed in final phases of a development project
3. Improved quality of code design, and increased ability to combine code with future programs

### Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests

- Individual Pitfalls:
  - Forgetting to run tests as often as needed
  - Writing tests that are too large
  - Writing trivial tests, or tests for trivial code

- Team Pitfalls:
  - Partial adoption (only a part of the team regularly tests code)
  - Poor maintenance of the test suite

## [CI/CD](https://www.youtube.com/watch?v=xSv_m3KhUO8)

### What are three benefits of Continuous Integration?

- Ensures new code can be integrated safely into the current version of your software
- Helps catch bugs
- Reduces merge conflicts

### What is the difference between Continuos Delivery and Continuous Deployment?

- Continuous Delivery = Developing software in such a way that it could be released at any time during development. Develop features with modular code, in more manageable increments

- Continuous Deployment = Allows you to actually deploy new features into production with little or no delay

### Explain how GitHub fits into this process assuming the listener comes from a non-technical background

- GitHub acts like a "clearing house" that helps keep track of changes to your code, and communicates with other systems about those changes
- "Webhooks" allow GitHub to send messages to external systems about activity in a project being shared to GitHub

[Back to Home](../README.md)
