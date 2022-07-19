# Code 401 - Class 27

## useState() Hook

### [Introducing Hooks](https://reactjs.org/docs/hooks-intro.html#motivation)

**What was the motivation for introducing Hooks?**

- Before hooks, there was not a way to "attach" reusable behavior to a component. A few methods were developed for dealing with this issue (such as render props and higher-order components) but they required a developer to restructure their components. This was not ideal, so hooks were created.

**What changes are important regarding implementing Hooks versus Component Classes?**

- Written as functions instead of classes
- Must receive props as arguments into the parameters
- No constructor needed
- No render method (just a return)

**Hooks allow you to reuse stateful logic without changing...**

- Your component hierarchy

### [hooks api](https://reactjs.org/docs/hooks-overview.html)

**Name two rules imposed by React Hook usage.**

1. Only call hooks at the top level
2. Only call hooks from React functions

**How would you identify a custom Hook and why might you create one?**

- Custom hooks start with `use`. For example: `useFriendStatus`.

### [the state hook](https://reactjs.org/docs/hooks-state.html)

**What is a Hook?**

- A hook allows you to use state and other React features without writing a class. It lets you "hook into" React features.

**When would I use the `useState` Hook?**

- When you want to add React state to function components. Instead of converting the function component to a class, you can now use a hook inside it.

**If you were to add React state to a function component by declaring a state variable:**

**What does calling `useState` do?**

- Declares the "state variable"

**What do we pass to `useState` as an argument?**

- The initial state ONLY

**What does `useState` return?**

- 2 values: the current state, and a function that updates it

[Back to Home](../README.md)
