# Code 401 - Class 36

## Application State with Redux

### [Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

**1. What is the first principle of Redux?**

- To represent the whole state of your application in a single JavaScript object

**2. What is a store and what do we use our reducers for within that store?**

- A store in Redux is where all state is kept. The Reducer function is the single, pure function that takes the previous state of the app and the action being dispatched, and returns the next state of the app

**3. Name three Redux store methods given to us by createStore and describe their use.**

- `getState()` - Retreives the current state of the Redux store
- `dispatch()` - Dispatches actions to change the state of the app
- `subscribe()` - Lets you register a callback that will be called any time an action is dispatched. This allows the UI to be updated to reflect the current state

**4. Explain to a non-technical recruiter what `combineReducers()` does and why it is useful.**

It is very common that multiple reducers need to be used within an app to manage state. This can require extensive code to be written so the different reducers can handle their respective parts of the state tree, and then combine their results to update the UI accordingly.

Redux offers the `combineReducers()` function that prevents a developer from needing to write all the code by hand, and automatically creates the top-level reducer function.

[Back to Home](../README.md)
