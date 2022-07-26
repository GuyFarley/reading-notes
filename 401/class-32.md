# Code 401 - Class 32

## Context API - Behaviors

### [Hooks and Context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

**With regard to the React Context API, what does a “provider” do?**

- It allows consuming components to subscribe to context changes

**With regard to the React Context API, how would we implement a “consumer” role?**

- Wrap a `<Consumer>` component around the elements that require the context from the provider

**Specifically with Context, how are we “wrapping” components to achieve our goals?**

- Opening `<Consumer>` tag before the elements and closing `<Consumer />` tag afterwards. Example:

```
    <CountContext.Consumer>
      {context => {
        if (context === undefined) {
          throw new Error('CountConsumer must be used within a CountProvider')
        }
        return children(context)
      }}
    </CountContext.Consumer>
```

### [Awesome React Context links](https://github.com/diegohaz/awesome-react-context)

**Consume content from (at least) two more of the Awesome React Context links. After some familiarity with React Context, once again share your takeaways from each:**

- **Takeaway 1:** (from the video [What's New in React 16.3.0](https://www.youtube.com/watch?v=WhWqy-vxKS8)): Context is an object that contains:

```
{
  Consumer: Object,
  Provider: Object,
  currentValue: "Hello",
  defaultValue: "Hello",
}
```

- **Takeaway 2:**
- The `<Provider>` component can render its children, and whatever you pass to the `value` prop will be available to the context `<Consumer>`
- We need to wrap the Consumers with the appropriate `<Provider>` component, in order to pass them the context they need

[Back to Home](../README.md)
