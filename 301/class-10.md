# Code 301 - Class 10 - In memory storage

## [Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

1. **What is a ‘call’?** A function invocation

2. **How many ‘calls’ can happen at once?** One at a time

3. **What does LIFO mean?** Last In, First Out

4. **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

![Stack Drawing](/301/call%20stack.png)

5. **What causes a Stack Overflow?** When you have a function that calls itself without an exit point, the calls will stack up on each other until they reach the browser's maximum stack capacity. This will throw an error

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. **What is a ‘reference error’?** This will happen if you try to use a variable that hasn't been declared yet, or incorrectly declare a variable

2. **What is a ‘syntax error’?** This occurs when your code cannot be parsed in terms of syntax

3. **What is a ‘range error’?** A range error occurs when you try to give an object or array an invalid length, for example

4. **What is a ‘type error’?** Refers to an error regarding data types, for instance if you try to access a property in an undefined variable

5. **What is a breakpoint?** It is a point in the code that you can cause to "break" (or stop running) to help identify where an error might be occuring

6. **What does the word ‘debugger’ do in your code?** It will cause a breakpoint to occur, so you can see the history of the call stack

[Back to Home](../README.md)
