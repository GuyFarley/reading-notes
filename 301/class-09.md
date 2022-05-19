# Code 301 - Class 09 - Functional Programming

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. **What is functional programming?** It is a programming style (or "paradigm") that treats computation as evaluation of mathematical functions instead of changing-state and mutable data

2. **What is a pure function and how do we know if something is a pure function?** A function is "pure" if it returns the same result if given the same arguments and does not cause any observable side effects

3. **What are the benefits of a pure function?** A pure function is easier to test because the data is immutable.

4. **What is immutability?** Data is immutable if its state cannot change after it is created.

5. **What is Referential transparency?** If a function consistently yields the same result for the same input, it is considered "referentially transparent"

>"pure functions + immutable data = referential transparency"

## [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. **What is a module?** A separate Javascript file that holds functionality that can be used in various places throughout an app

2. **What does the word ‘require’ do?** It allows the Javascript file to access the required module

3. **How do we bring another module into the file the we are working in?** We need to "require" it. In other words we need to add the following to our Javascript file that we want to bring the module into:

```
require('./<module-name>');
```

4. **What do we have to do to make a module available?** Inside the module, we need to export the portion of the module that we want to be available outside the module:

```
module.export = <portion of module to be available outside module>;
```

Then we need to declare a variable in the Javascript file that is equal to the "require" statement:

```
let counter = require('./<module-name>');
```

[Back to Home](../README.md)
