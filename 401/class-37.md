# Code 401 - Class 37

## Redux - Combined Reducers

### [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

**1. Why create multiple reducers?**

- For ease of maintainability

**2. How would you combine multiple reducers?**

- Bring in `combineReducers` from `redux`. Then write your multiple reducer functions to manage state. Then set a new variable (can be called `reducers`) to equal `combineReducers()`, passing in the state properties you want to change, along with the specific reducer functions that will handle each of them.

**3. How will you manage state as an immutable object? why?**

### [Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

**1. `combineReducers` is a utility function to simplify the most common use case when writing *Redux Reducers* .**

- Redux reducers

**2. Explain how `combineReducers` assembles the new state tree.**

- `combineReducers` calls each slice reducer with its current slice of state, along with the current action, giving the slice reducer a chance to respond and update its portion of state if needed.

**3. How would you define initial state in an app using `combineReducers`?**

- There are 2 ways to do this:
  - The `createStore` function can take `preloadedState` as a 2nd argument
  - The root reducer can return the initial state value when the state argument is `undefined`

### [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

**1. Why will you want to split your reducing functions as your app becomes more complex?**

- To make it easier to manage independent portions of state

**2. The *`combineReducers`* helper function turns an object whose values are different reducing functions into a single reducing function you can pass to *`createStore`*.**

**3. What is a popular convention when naming reducers?**

- To name reducers after the state slices they manage, allowing you to use ES6 shorthand notation. For example:

```
combineReducers({ counter, todos }) 
```

is equivalent to writing:

```
combineReducers({ counter: counter, todos: todos })
```

[Back to Home](../README.md)
