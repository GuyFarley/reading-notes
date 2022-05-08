# Code 301 - Class 01 - Introduction to React and Components

## Why this matters

React is a component-based library that we'll be working with quite a bit in 301, so it's important to begin to understand what components are. It's also important for us to understand how data is passed into these React components, which is how props (or properties) are used. The readings below explain the basic concepts behind this functionality.

## [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

### What is a “component”?

From the tutorialspoint article "Component-Based Architecture" (linked above):

- A **component** is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exports it as a higher-level interface
- It is a software object that encapsulates functionality
- It is a unit of composition with a contractually specified interface and explicit context dependencies
- **Components** represent well-defined communication interfaces containing methods, events, and properties. A component provides a higher level of abstraction and divides the problem into sub-problems, each associated with **component partitions**
- *Component reusability = the ability to reuse functionality and behaviors in a self-deployable binary unit.* This allows for:
  - Reduced time in market, and reduced development cost
  - Increased reliability
- 3 different views of a component:
  - **Object-oriented** - Viewed as a set of one more more cooperating classes. Defined attributes and operations, and defined interfaces that enable classes to communicate
  - **Conventional** - Viewed as a functional element or module of a program
  - **Process-related** - Build from existing components in a library. As software architecture is formulated, components are selected and used to populate that architecture
  
### What are the characteristics of a component?

From the tutorialspoint article "Component-Based Architecture" (linked above):

- Reusable
- Replaceable
- Not context specific
- Extensible - Can be extended from existing components to provide new behavior
- Encapsulated
- Independent - Designed to have minimal dependencies on other components

### What are the advantages of using component-based architecture?

From the tutorialspoint article "Component-Based Architecture" (linked above):

- Ease of deployment
- Reduced Cost
- Ease of development
- Reusable
- Modification of technical complexity
- Reliability
- System maintenance and evolution
- Independency and flexible connectivity of components

## [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

### What is “props” short for?

- **Props** stands for *properties*. Props are arguments passed into React components (from w3schools.com)

### How are props used in React?

- They are used for passing data from one component to another.

### What is the flow of props?

- Uni-directional (one way from parent to child)
- Props data is read-only, and child components should not change the data coming from their parent component
- Using Props in React:

1. Define an attribute and its value (or data)

```
<ChildComponent text={"I'm the 1st child"} />
```

2. Pass it to child component(s) by using Props

```
const ChildComponent = (props) => {
  return <p> I'm the 1st child!</p>;
};
```

3. Render the Props Data

```
const ChildComponent = (props) => {
  return <p>{props.text}</p>;
};
```

## Things I want to know more about

- Practical examples of how props are used in React
- What are best practices for building components?
- Are there components already included within the React library, or do we write them all ourselves?

[Back to Home](../README.md)
