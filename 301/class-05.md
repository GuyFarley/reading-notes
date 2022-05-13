# Code 301 - Class 05 - Putting it all together

## [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

### What is the single responsibility principle and how does it apply to components?

- [Wikipedia](https://en.wikipedia.org/wiki/Single-responsibility_principle) defines it as "a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part."
- This means that ideally, each component in React should only do one thing. And if it ends up growing, it should be "decomposed" into smaller subcomponents.

### What does it mean to build a ‘static’ version of your application?

- This means to build a version of the app that has no interactivity (yet)

### Once you have a static application, what do you need to add?

- State!

### What are the three questions you can ask to determine if something is state?

- From the [React doc](https://reactjs.org/docs/thinking-in-react.html):

  - Is it passed in from a parent via props? If so, it probably isn’t state.
  - Does it remain unchanged over time? If so, it probably isn’t state.
  - Can you compute it based on any other state or props in your component? If so, it isn’t state.  

### How can you identify where state needs to live?

- From the [React doc](https://reactjs.org/docs/thinking-in-react.html):

  - Identify every component that renders something based on that state.
  - Find a common owner component (a single component above all the components that need the state in the hierarchy).
  - Either the common owner or another component higher up in the hierarchy should own the state.
  - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

### What is a “higher-order function”?

- It is a function that operates on other functions (by taking them as arguments or returning them)

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

- It is returning a function from inside the `greaterThan()` function

### Explain how either map or reduce operates, with regards to higher-order functions

- `map` operates as a higher-order function that applies a function (a callback function) to all elements of an array and then builds a new array from the returned values

[Back to Home](../README.md)
