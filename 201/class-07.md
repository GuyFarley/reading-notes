# Code 201 - Class 07 - HTML Tables; JS Constructor Functions

## [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

- **Domain modeling**: the process of a conceptual model within your code to solve a specific problem
- **object oriented** model: stores data in properties and contains behaviors inside methods
Example:

1. Constructor function is defined using a function expression: the variable `EpicFailVideo` is declared, then assigned a function with 2 parameters called `epicRating` and `hasAnimals`

```
let EpicFailVideo = function(epicRating, hasAnimals){}
```

2. Function is called, and data inside the parameters is stored inside `this.epicRating` and `this.hasAnmials` properties

```
let EpicFailVideo = function(epicRating, hasAnimals){
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}
```

3. Two objects are **instantiated** with the `new` keyword and their properties are **initialized** by calling the `EpicFailVideo` constructor function

```
let parkourFail = new EpicFailVideo(7, false);
let corgiFail = new EpicFailVideo(4, true);
```

4. The objects are stored inside the `parkourFail` and `corgiFail` variables

## HTML Chapter 6: “Tables” (pp.126-145)

- Tables can be used in HTML to display information in grid format. This can be done using the `<table>` element
  - `<tr>` = table row
  - `<td>` = cell within each row
  - `<th>` = cell within the header
- You can also split a table into a header, body, and footer using the `<thead>`, `<tbody>`, and `<tfoot>` tags, respectively

## JavaScript Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

- Objects can be created with **Constructer Notation** as well: creates a new blank object that properties and methods can be added into
- Examples:

```
let hotel = new Object();
```

OR

```
let hotel = {}
```

- Once you've created the blank object, you can add to it using **dot notation** or square bracket syntax
- Examples:

```
hotel.name = 'Holiday Inn';
```

OR

```
hotel['name'] = 'Holiday Inn';
```

- You can also delete a property from an object using the `delete` keyword: `delete hotel.name;`

### Constructor Notation

- If you need to create multiple objects that represent similar things, you can use **constructor notation** to build them:

1. Use a function as a template
2. Add statements to the function that add properties or methods
3. The `this` keyword is used to indicate that each new property or method belongs to the object that "this" function creates

```
function Hotel(name, rooms, booked){
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  this.checkAvailability = function(){
    return this.rooms - this.booked;
  };
}
```

4. Create **instances** of the new object using the **constructor function**

- The `new` keyword, followed by a call to the function creates a new object, with the properties of each new object passed as arguments to that function:

```
let quayHotel = new Hotel('Quay', 40, 25);
let parkHotel = new Hotel('Park', 65, 88);
```

**Arrays** are a special type of object, where the key for each value is its index number

- ***Arrays can store objects and objects can hold arrays***

### Built-In Objects

- The DOM is actually just one of three sets of built-in objects:

1. **Browser Object Model**: Creates a model of the browser tab or window
2. **Document Object Model**: Creates a model of the current web page
3. **Global JavaScript Objects**: A group of individual objects that relate to different parts of the JavaScript language

[Back to Home](../README.md)
