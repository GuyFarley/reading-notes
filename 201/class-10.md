# Code 201 - Class 09 - Forms and Events

## Why this matters

- It's important to understand how JavaScript processes code (one line at a time) in order to effectively debug your code
- Debugging is an important skill that involves narrowing down where the problem might be, then looking for clues

## JavaScript Ch. 10 - “Error Handling & Debugging”

- There are several tools or concepts that will help a programmer to more easily identify bugs and where they are occuring:
  - When data is required from another function, that function is **stacked** on top of the current task
  - **Hoisting** is the concept that variables and functions are created before they are executed. This happens in the PREPARE phase of a script, at which point they are **hoisted** to the top of the execution context
  - **Exception-handling** code can be included in your JavaScript to help inform you when there's a problem, rather than relying on the interpreter to tell you
  - **Error objects** are built-in objects created by JS when an error occurs, and they include:
    - *name* (type of error)
    - *message* (description)
    - *fileNumber* (name of the JS file)
    - *lineNumber* (line number of error)
- The **console** can help you greatly when debugging. It is helpful to log data to the console (via `console.log()` at specific points in your code, so that you can visually see in the console when lines of code are being executed correctly
- **Breakpoints** can be used to pause the execution of a script on any line, allowing you to see the values stored at each breakoint
- Once you've added these **breakpoints**, you can step through them to find out where errors might be occuring

## Things I want to know more about

- Adding breakpoints and stepping through code line by line
- **Try, Catch, Finally** statements

[Back to Home](../README.md)
