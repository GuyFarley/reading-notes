# Code 401 - Class 31

## Context API

### [Context API](https://reactjs.org/docs/context.html)

**What can React Context provide your app?**

- A method of passing data down through the component tree without having to manually pass down props

**Why might we use Context?**

- Whenever we have data that can be considered "global" for a component tree. Example: current authenticated user

**Why should we use it sparingly?**

- Because it ultimately makes component reuse more difficult. It should only be used when data needs to be accessible by many components at different nesting levels

### [Awesome React Context links](https://github.com/diegohaz/awesome-react-context)

**Consume content from (at least) two of the Awesome React Context links. Share your take-away from each:**

- **Takeaway 1:** (from the video [Heres how React's New Context API Works](https://www.youtube.com/watch?v=XLJN4JfniH4))

  - Context becomes really important when data needs to be passed down through multiple levels (through components that don't even use it, in most cases). Even at just 3-4 component levels, this becomes extremely cumbersome! Historically, many developers will rely on something like Redux to store data - but in most cases React's Context API is a better option

- **Takeaway 2:** (from the article [Migrating to React's New Context API
](https://kentcdodds.com/blog/migrating-to-reacts-new-context-api))

  - React's Context API is an improvement over previous context handling within React in a few ways. It provides explicit components that must be used in order to provide and consume context. Instead of using properties to make things work, you can now use simple components.

[Back to Home](../README.md)
