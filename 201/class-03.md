# Code 201 - Class 03: HTML Lists, Control Flow with JS, and the CSS Box Model

## HTML Chapter 3: Chapter 3: “Lists”

Lists are commonly used in HTML because they come in quite handy for many things! There are three types of lists that HTML provides us:

- Ordered lists are numbered lists
- Unordered lists are bulleted
- Definition lists are provide definitions for each item in the list

## HTML Chapter 13: “Boxes”

CSS treats every HTML element as if it lives in its own box. And every box has 3 properties that can be modified to control how it appears on the page:

1. Border - Separates the edge of one box from another
2. Margin - Space around the outside of the border
3. Padding - Space between the border and the box's contents

Additional properties that can be used to change the appearance of a box include:

- `border-width`
- `border-style`
- `border-color`
- `border-width`
- `display`
- `visibility`
- `border-image`
- `box-shadow`
- `border-radius`

## JavaScript Chapter 2: “Basic JavaScript Instructions”, cont

**Arrays** are a very powerful feature of JavaScript that allows for great flexibility when writing your code. An **array** is a type of variable that can store a full list of values.

- Arrays are created in the same way any other variable is created
- Values assigned to an array are placed inside square brackets `[]` and separated by commas
- Example:

```
let colors;
colors = ['blue', 'gray', 'green'];
```

- You can also store a string, a number, and/or a Boolean all in the same array, since the values do not need to be all of the same data type
- The values in an array are automatically placed in a numbered list, and each item in the array is given a number called an **index**. ***These numbers start with 0, not 1!***
- In the code example above, the blue item would have an index of 0, the gray item would have an index of 1, and the green item would have an index of 2. So to access the 3rd item of this array, you would specify the number '2' inside square brackets after the array name:

```
colors [2]
```

Putting it all together, the following code example shows how you would create an array of 3 colors, access the 3rd item in that array, change its value, and write it into the HTML page:

```
let colors = ['blue', 'gray', 'green'];
colors[2] = 'orange';
let colorPick = document.getElementById('colors');
colorPick.textContent = colors[2];
```

## JavaScript Chapter 4: “Decisions and Loops”, cont

A **switch** statement is similar to an **if...else** statement in that it checks the value of a variable against possible values in the statement, and then makes decisions based on that evaluation. There are some key differences though...

- With a **switch** statement, there must be a `default` option that is executed if none of the cases match (whereas an `else` option is not required in an **if...else** statement)
- The code in a **switch** statement is only run until a match is found, then the `break` statement stops the rest of the statement from running

Loops are scripts that check a condition, and if it evaluates to true, a code block will run. There are 3 types of loops:

- **for loops** are best used when doing something to each item in a list, doing something a specific number of times, if building a counter, etc.
- **while loops** execute their statements as long as a specified condition evaluates to true. This type of loop will run an undetermined number of times.
- **do...while** loops are similar to while loops, except they will always run their code block at least once (even if the condition evaluates to false)

## Things I want to know more about

- How to change a box's appearance using the various values of the `display` property in CSS (`inline`, `block`, `inline-block`)
- Using loops in combination with arrays

[Back to Home](../README.md)
