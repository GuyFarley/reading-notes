# Code 401 - Class 26

## Component Based UI

### [react hello world](https://reactjs.org/docs/hello-world.html)

**What are the building blocks of a React app?**

- Elements and Components

**What is the difference between an element and a React component?**

- A React *Element* describes what you want to see on the screen, and is the smallest building block of a React app. While a *Component* is a small, reusable piece of code that returns an Element to be rendered to the page

**What are some advantages of React’s component based architecture?**

- Components can be reused, plugged into other components, and easily refactored as needed

### [introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

**What is JSX and why do we use it?**

- JSX is a syntax extension to JavaScript, and it allows us to produce React elements

**Describe the process of embedding JavaScript expressions in JSX.**

- Any valid JavaScript expression can be embedded in JSX by placing it in curly braces. For example:

```
const name = 'Guy Farley';
const element = <h1>Hello, {name}</h1>;
```

**Is it safe to embed user input in JSX? Explain.**

### [rendering elements](https://reactjs.org/docs/rendering-elements.html)

**Explain what a React Component is to a non-technical friend.**

- In React, a Component is basically a JavaScript function that represents a piece of the user interface. It takes in some input, and then returns React elements that describe what should appear on the screen. Components allow developers to think about each piece of the UI in isolation, to more easily manage it

**Describe mutability and React Components, specifically, how is the UI updated?**

- React allows updating of the UI by changing the information being returned by the Components (via state)

**If changes are made to the UI, what does React update?**

- The DOM (only those portions that have been changed)

[Back to Home](../README.md)
