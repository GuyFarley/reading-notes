# Code 201 - Class 06 - Problem Domain, Objects, and the DOM

## [Understanding the problem domain is the hardest part of programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

- Problem domains are sometimes the most difficult part of programming because they often do not give complete information about a project, or the info provided may be very unclear
- Programming is much easier if you can understand the problem domain!
- Understanding the problem to be solved is the most critical piece to the equation!
- As developers, we can make programming easier by doing one of two things:
  1. Making the problem domain easier
  2. Getting better at understanding the problem domain
- We can make the problem domain easier by taking one part of the problem and fully understanding it before looking at a bigger portion of the problem
- We can get better at understanding the problem domain by talking to those who actually know about the problem
- It will save a lot of time and energy to make sure you fully understand the problem before trying to write the code!

## [What’s the difference between primitive values and object references in JavaScript?](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)

- Primitive values and object references behave differently in JavaScript code, and this affects how JS programs will ultimately run
- **Primitive value** - A variable is set to a value directly
  - **Immutable data** - *Cannot* be changed
  - Example: you can access the first letter of a string stored in a variable, but you cannot change the first letter of that string in order to make it a different word
- **Object reference** - A variable does not contain the value directly, it instead contains a reference to the memory address where that object is stored on the computer
  - **Mutable data** - *Can* be changed
  - Example: you can access the first item in an array (because arrays are just special objects in JavaScript) and you can change that item whenever you like

```
let letters = ['s', 'l', 'i', 'p'] 
letters[1] = 'k'
console.log(letters) // ["s", "k", "i", "p"]
```

- **Side note:** You can define an array with `const` instead of `let`, and still be able to change elements within the array. This is because `const` only prevents you from reassigning values to a variable, not from changing (or *mutating*) existing values
- With object references, it is possible to create multiple references to the same memory address where data is stored - but this can sometimes be a problem in JavaScript programming
- To avoid issues with this, you can create a new object instead of a 2nd reference to an existing object by using `Object.assign` instead. Example:

```
let leadSinger = {
  name: 'Eddie Vedder',
  group: 'Pearl Jam'
}
let leadGuitar = Object.assign ({}, leadSinger, {name: 'Mike McCready'})
console.log(leadSinger, leadGuitar)
// {name: "Eddie Vedder", group: "Pearl Jam"}
// {name: "Mike McCready", group: "Pearl Jam"}
```

- When objects are compared using equality operators, the comparison will evaluate to false - This is because the objects are references (memory addresses) and not direct values. So even though the contents on the left and right of an equality operator will look the same, the memory addresses are different
  - To check whether the contents (not reference) of two objects match, you can:
    1. *Check through each key and value of the object to make sure they match (can be tricky)*
    2. *Covert the object to primitive value and then do the equality check*

- An example of the 2nd method:

```
const eddieA = { name: 'Eddie Vedder' }
const eddieB = { name: 'Eddie Vedder' }
eddieA === eddieB // false
JSON.stringify(eddieA) === JSON.stringify(eddieB) // true
```

- Chris Geelhoed notes in his article "What’s the difference between primitive values and object references in JavaScript?":
  > "Developing a strong grasp of primitive values, object references, and mutability is a critical step in progressing past the beginner stages of JavaScript programming.
  >
  >This knowledge will help you identify bugs, understand key differences in programming paradigms, and help you understand your code at a deeper level."

## JavaScript Chapter 3: “Object Literals” (pp.100-105)

- **Objects** group together sets of variables and functions
  - Inside an object, variables become **properties** and functions become **methods**
  - Each property and method in an object have a **key** (or a name) and a **value**
- There are several ways to create objects in JavaScript, but the most popular is **Literal Notation**
  - **Object** is the curly braces and their contents
  - Each **key** and its **value** are separated by a colon `:`
  - Each **property** and **method** are separated with a comma `,`
  - Example:

```
let hotel = {
  name: 'Best Western',
  rooms: 40,
  booked: 25,
  checkAvailability: function() {
    return this.rooms - this.booked; 
  } //subtracts value of 'booked' in this object from value of 'rooms' in this object
}
```

- You can access the properties/methods of an object using **dot notation**
  - Access a property or method by using the name of the object, followed by a period, followed by the name of the property/method. Example:

```
  let hotelName = hotel.name;
  let roomsFree = hotel.checkAvailability();
```

- Square bracket syntax can also be used to access properties/methods of an object:

```
let hotelName = hotel['name'];
let roomsFree = hotel['checkAvailability']();
```

## Chapter 5: “Document Object Model” (pp.183-242)

- The DOM tree is a model of a web page, and consists of four types of nodes:
  - **Document nodes** represents entire pages
  - **Element nodes** represent the elements of that page
  - **Attribute nodes** represent the attributes of those elements (if they exist). These are not "children" of the elements, but instead part of the elements
  - **Text nodes** represent the text within each element

- Accessing and updating the DOM tree requires two steps:
  1. Step 1: Access the elements
  2. Step 2: Work with those elements

### Accessing the Elements

- Common ways to access an individual element:
  - `getElementById()` - Uses the value of the element's `id` attribute
  - `querySelector()` - Uses a CSS selector to return the first matching element
- Common ways to access multiple elements (or nodelists):
  - `getElementByClassName()` - Selects all elements with a specific `class` attribute
  - `getElementsByTagName()` - Selects all elements with a specific tag name
  - `querySelectorAll()` - Uses a CSS selector to select all matching elements

### Working With the Elements

- `nodeValue` property lets you access or update the contents of a text node
- `innerHTML` property allows you to access the child elements of an element and their text content
- `textContent` property allows you to access just the text content

**DOM queries** are methods that find elements in the DOM tree:

```
getElementById('one'); // looks through the DOM tree for an element whose `id` attribute has a value of "one"
```

```
let itemOne = getElementById('one'); // the variable "itemOne" stores a reference to where the node is located in the DOM tree
```

- You can select an item from a Nodelist as well, by specifying the index number of the element you want:

```
let elements = document.getElementsByClassName('hot'); // creates the Nodelist containing elments with the class attribute whose value is "hot", stores in variable "elements"
if (elments.length >= 1) { // checks if there is at least one element in the Nodelist
  let firstItem = elements[0]; // assigns the first element from the Nodelist to the variable "firstItem"
}
```

- Adding or removing HTML content can be done one of two ways:
  1. The `innerHTML` property (faster, but less secure):
  - Store new content as a string in a variable
  - Select the element you want to replace the content of
  - Set the element's innerHTML property to be the value of the varaible you created (the new string)
  2. DOM manipulation (more secure, but slower):
  - Create element and text nodes, then attach them or remove them from the DOM tree
- We can view the DOM tree using the developer tools found within the browser!

[Back to Home](../README.md)
