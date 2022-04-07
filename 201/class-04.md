# Code 201 - Class 04 - HTML Links, CSS Layout, JS Functions

## HTML Chapter 4: "Links"

- You can create links to other pages from your page by using the `<a>` element:

```
<a href="https://www.google.com">Google</a>
```

- URL's are fine for linking to other sites, but when linking to other pages on your own site, it's always best to use **relative URL's**

## HTML Chapter 15: “Layout”

- CSS treats each HTML element as if it lives in its own box
- These boxes can be **block-level** or **inline**
  - **Block-level** elements start on a new line
  - **Inline** elements flow in between surrounding text
- Containing elements (or parent elements) are block-level elements that contain other block-level elements inside them (for instance, all elements of a footer would be contained within the parent element `<footer>` or `<div>`)
- There are many positioning schemes that CSS provides, which help you control the layout of a page:
  - **Normal flow**: Elements appear one after the other, vertically
  - **Relative positioning**: Elements can be shifted up, down, left, or right (as compared to where they would have been placed)
  - **Absolute positioning**: Positioning an element in relation to its containing element
  - **Fixed positioning**: Similar to absolute positioning, but positions an element in relation to the browser window instead
  - **Floating elements**: Positions an element to the far left or far right of its containing box

## JavaScript Chapter 3: “Functions, Methods, and Objects”

- Function **keyword** declares the function
- Function **name** identifies the function (followed by parentheses)
- The function's **code block** contains the statements that perform the function's task
- Functions store the code that is needed to perform a task, and the function can be called multiple times. This is way more efficient that re-writing the code each time it is needed
- Functions are **called** (or **invoked**) with just one line of code that includes the function's name, followed by parentheses:

```
sayHello();
```

- Information can be provided to the function in the form of **parameters**. These exist inside the parentheses after the function name, and act as variables inside the code block
- When calling this type of function, you specify the values it will use in the parentheses that follow the function name (when called). These values become **arguments** when passed to the actual function, and those arguments become values of the variables inside the code block
- Functions can return a single value or multiple values (as when using an array)
- Example of a simple function:

```
function myFunction() {
  let carName = "Subaru";
  document.getElementById("demo1").innerHTML =
  typeof carName + " " + carName;
}
```

## Article: “6 Reasons for Pair Programming”

- Pair programming is when two developers work together at a single workstation (remotely or in person) to write code
- According to this [Code Fellows article](https://www.codefellows.org/blog/6-reasons-for-pair-programming/), pair programming provides:

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

## Things I want to know more about

- Returning multiple values from a function using an array
  - What are some good examples of how to use this in the real world?
- The subtle differences between **parameters** and **arguments**

[Back to Home](../README.md)
