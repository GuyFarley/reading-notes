# Code 401 - Class 28

## Component Lifecycle / `useEffect` Hook

### [effects hook](https://reactjs.org/docs/hooks-effect.html)

**What purpose does useEffect serve in a function component compared to its counterpart(s) in class components?**

- In a function component, `useEffect()` allows additional code to run after React has updated the DOM. This is similar to `componentDidMount()` and `componentDidUpdate` in class components

**When using the useEffect Hook:**

- **What does useEffect do?**
  - It tells React the component needs to do something after the render

- **Why is useEffect called inside a component?**
  - This lets us access the props right from the effect

- **Does useEffect run after every render?**
  - Yes. This prevents us from needing to duplicate code, as we would need to do in a class component when using `componentDidMount()` and `componentDidUpdate`

**Explain the importance of properly implementing effects with Cleanup**

- When an effect has the potential to produce a memory leak (such as when subscribed to an external data source), we need to "clean up" after the effect to prevent this. We can do this by returning a function from inside the `useEffect()` hook that cleans up after the component unmounts

[Back to Home](../README.md)
