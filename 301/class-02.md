# Code 301 - Class 02 - State and Props

## Why this matters

As we begin building components in React, it will be very helpful to understand when methods or events occur within the component's lifecycle. This will help us to be intentional as we build, to avoid bugs or inefficient code. It will also be helpful for us to understand the different kind of data components use (props vs. state) so we can also be intentional about when/where that data should be provided to the component.

## [React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- Components can be **classes** or **functions**
- The methods used on these components are called **lifecycle events** and can be called during the component's lifecycle
- The three phases of the component lifecycle are:
  - **Mounting** - An instance of a component is created and inserted into the DOM during this phase
  - **Updating** - A component is rerendered whenever it is updated or its **state** changes
  - **Unmounting** - Occurs when a component is being removed from the DOM. The only lifecycle event during this phase is `componentWillUnmount`, which allows you to clean up the DOM, network requests, and subscriptions

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- *The render happens first*
- `render()` is the only method that is required in a class component - when called, it examines `this.props` and `this.state`
- `render()` should NOT modify the component **state** and should NOT directly interact with the browser

### What is the very first thing to happen in the lifecycle of React?

- *The constructor*
  - If the component is a subclass, `super(props)` needs to be called or else the props will be undefined
  - Can be used to assign state using `this.state` or to bind event handle methods

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- *constructor*
- *render*
- *React updates*
- *componentDidMount*
- *componentWillUnmount*

### What does componentDidMount do?

- *This method allows you to initialize the DOM, load anything using a network request, and/or set up subscriptions*

- React's default behavior is to re-render a component after every state change, but this can be prevented by setting `shouldComponentUpdate()` to `false`.

## [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

### What types of things can you pass in the props?

- Things you want to initialize your component to, or how you want your component to initially render (initial count of a counter, for example)

### What is the big difference between props and state?

- Props are handled outside of a component and passed into it, while state exists (and is handled) inside of that component

### When do we re-render our application?

- Whenever state changes

### What are some examples of things that we could store in state?

- A counter - State will be used to keep track of when the counter is changed inside the component
- A form that needs to be updated by the user - State will be used to store these changes

[Back to Home](../README.md)
