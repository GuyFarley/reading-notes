# Code 401 - Class 29

## Advanced State with Reducers

### [useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

**Name an alternative to the `useState` Hook.**

- `useReducer()`

**Why might the `useReducer` Hook be preferable to the `useState` Hook?**

- In cases where you have complex state logic that involves sub-values, or when the next state depends on the previous one

**What are two ways to set the initial state?**

1. Pass the initial state as a second argument. For example:

```
const [state, dispatch] = useReducer(
    reducer,
    {count: initialCount}
  );
```

2. Create the initial state "lazily" by passing in an `init` function as the 3rd argument. The initial state will be set to `init(initialArg)`

### [Ultimate Guide to useReducer](https://blog.logrocket.com/react-usereducer-hook-ultimate-guide/)

**In terms of state, what does `useReducer` expect to receive as a parameter?**

- It expects a `reducer` function as its first parameter and the initial state as the 2nd parameter

**What does `useReducer` return?**

- An array that holds the current state value, along with a `dispatch` function

**Explain `dispatch` to a non-technical recruiter.**

When data needs to be updated and re-rendered to the screen, one of the best ways to do this is through a `useReducer` hook. The `useReducer` hook accepts a `reducer` function and the initial state of the data. It then returns back the current state value, along with a `dispatch` function. The `dispatch` function itself holds the type of action that needs to be executed when it is later called.

[Back to Home](../README.md)
