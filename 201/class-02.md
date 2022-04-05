# Code 201 - Class 02: HTML Text, CSS Introduction, and Basic JavaScript Instructions

## Why this matters

The content below is a continuation of our discussion about how **HTML**, **CSS**, and **JavaScript** are used to create the visual elements on a web page, as well as the interactive functionality. The JavaScript section is especially important, as it begins to explore how our instructions are pieced together to be understood by the browser, as well as how the code then makes decisions based on condition evaluation.

## HTML Chapter 2: "Text"

Text is by far the most common content displayed on web pages, and there are several elements that are used to mark up text to ensure it displays correctly. There are two different kinds of elements that can be used for text: **structural markup** and **semantic markup**.

As noted in Jon Duckett's book, "HTML & CSS - design and build websites", **structural markup** includes the elements you can use to describe both headings and paragraphs, while **semantic markup** provides extra information (such as where emphasis is placed in a sentence).

Examples of **structural markup** include:

- `<h1>`
- `<p>`
- `<b>`
- `<i>`
- `<sup>`
- `<sub>`
- `<br />`
- `<hr />`

Examples of **semantic markup** include:

- `<strong>`
- `<em>`
- `<blockquote>`
- `<q>`
- `<abbr>`
- `<cite>`
- `<dfn>`
- `<address>`

## HTML Chapter 10: “Introducing CSS”

CSS, or Cascading Style Sheets, work with HTML to provide the visual style to a page's structure. Using the CSS language, we can create style rules and then associate them with the elements on an HTML document.

Each of these CSS rules consists of two parts: a **selector** and a **declaration**.

- The **selector** indicates which HTML element the rule will apply to
- The **declaration** indicates how that element should be styled. Declarations themselves are also made up of two parts:
  - The **property** of a declaration notes the specific aspect of the element you want to change
  - The **value** specifies the setting you want to use for that property

 An example of a CSS rule would be:

```
p {
  font-family: Arial;
  color: blue;
}
```

While CSS rules may appear within an HTML document, this is not ideal. It is *especially* not ideal to use inline CSS (where the CSS is written into the HTML element itself). Best practice is to keep all CSS in a separate document, that is then referenced in the `<head>` of the HTML page.

## JavaScript Chapter 2: “Basic JavaScript Instructions”

A **script** in JavaScript is a set of very specific instructions for the computer to follow. Each instruction, or **statement**, within the script is like a step in a recipe. So, much like you would follow a recipe step-by-step to bake a banana bread, a computer will follow a script step-by-step in order to accomplish a goal.

**Variables** are like containers that exist to hold data. The data being held within the variable is its **value**. Variables are declared within the script in order to temporarily store information that is used in that script.

An **array** is a special type of variable that can store an entire list of values (not just one!) or a set of values that are related to each other.

**Expressions** and **operators** are used to evaluate into a single value that can then be assigned to a variable. **Expressions** rely on **operators** to calculate those values in some way--for instance, by adding two values together to create a new value, or to concatenate two strings together to create a new string value.

## JavaScript Chapter 4: “Decisions and Loops”

Oftentimes we will need our code to make decisions about what to do next. **Conditional statements** allow our code to do this. By including a conditional statement in our script, we are asking the code to:

1. Evaluate a condition
2. Execute a statement depending on that evaluation

Example:

```
if (score > 60) {
  document.write("Congrats, you passed the test!");
} else {
  document.write("Sorry, you failed!");
}
```

In the example above, the `if` statement evaluates the condition, and if the condition is **true**, the statements in the first code block are executed.
However, if the condition is **false** upon being evaluated, the statements in the second code block are executed instead.

## Things I want to know more about

- Using flowcharts to plan out how the code should make decisions before writing the actual code
- The `.textContent` method used on page 153

[Back to Home](../README.md)
