# Class 07: Programming with JavaScript

## What is your malfunction! Hopefully not your function...

But before we talk about *functions*, let's talk about the *control flow* (or, the order in which the computer executes statements in a script). Most JavaScript will include many control structures such as *conditionals*, *loops*, and *functions*. These ontrols can drive complex flows of processing with very few lines of code! Here's the point: **When reading a script, you must not only read from start to finish but also note how the program structure affects the order of execution.**

Ok back to functions. They are blocks of code designed to perform a task, and are only executed when something in the script "invokes" them. Functions are how we, as coders, create new commands for a program. They are very handy because they allow you to reuse code. In other words: Once code is defined once, it can be used over and over.

## Function Invocation

As mentioned, the code inside the function will execute when something invokes the function. This can happen in three different ways:
- When an event occurs (user clicks a button)
- If invoked from JavaScript code
- Automatically (self invoked)

Functions can also be used as variables (in formulas, assignments, and calculations). [W3Schools](https://www.w3schools.com/js/js_functions.asp) provides the following example, where instead of using a variable to store the return value of a function:
```
let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
```
You can use the function directly, as a variable value:
```
let text = "The temperature is " + toCelsius(77) + " Celsius";
```
## Refactoring
One of the greatest benefits of functions is something called refactoring - or, the ability to change the implementation while keeping the same functionality. Functions give us a place to do this. Code inside the code block can be changed, efficiencies can be found over time, etc. 

[Back to Home](README.md)