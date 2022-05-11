# Code 301 - Class 03 - Passing Functions as Props

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

### What does .map() return?

- `.map()` returns a modified array that is the same length as the array passed into it (and does not mutate the original array)

### If I want to loop through an array and display each value in JSX, how do I do that in React?

- You can use `.map()` to loop through the array and then return an `<li>` element for each item. Then you can assign the resulting array of elements to a variable and include that variable inside a `<ul>` element

### Each list item needs a unique ____

- Key

### What is the purpose of a key?

- A key is a special string attribute that needs to be included when creating a list of elements. It helps React identify which items have been changed, added, or removed

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

### What is the spread operator?

- The spread operator `(...)` expands an iterable object into the list of arguments, when used in a function call

### List 4 things that the spread operator can do

- Spread an array into separate arguments
- Add an item to a list
- Combine objects
- Copy an array

### Give an example of using the spread operator to combine two arrays

```
const myArray = [1,2,3,4]
const yourArray = [2,3,4,5]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 1 2 3 4 2 3 4 5
```

### Give an example of using the spread operator to add a new item to an array

```
const someNames = ['Guy','Tom','Jess']
const moreNames = ['Joe','Lisa', ...someNames]
console.log(moreNames) = // ['Joe', 'Lisa', 'Guy', 'Tom', 'Jess']
```

### Give an example of using the spread operator to combine two objects into one

```
const objectOne = {hello: 'world'}
const objectTwo = {whats: 'up'}
const objectThree = {...objectOne, ...objectTwo}
console.log(objectThree) // Object { hello: 'world', whats: 'up'}
```

## [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

### In the video, what is the first step that the developer does to pass functions between components?

- Creates the function wherever the state is that needs to change within the function

### In your own words, what does the increment function do?

- It takes in an array of objects and checks each object to see if the 'name' property matches the name being passed in. If so, it increments the 'count' property of that object by 1, and passes the object back into a modified array of objects. Then it changes the state of the original array so the values are that of the new array

### How can you pass a method from a parent component into a child component?

- Within the `render()` method of the child component, you can add a property to the child component that equals `{this.method}` (with 'method' being the method you are passing into it)

### How does the child component invoke a method that was passed to it from a parent component?

- The method can be called by including `this.props.method(this.props.property)` where 'method' is the method on the parent component that needs to be invoked, and 'property' is the property to be referenced

## Things I want to know more about

I definitely need some practice with the process the developer was going through on the video, where he passed functions between components. This really turned my brain inside out so I need to work through it many times to understand what's happening

[Back to Home](../README.md)
