# Code 201 - Class 09 - Forms and Events

## HTML Chapter 7: “Forms” (p.144-175)

- Information can be collected from site visitors using a **form** which lives inside a `<form>` element in the HTML
- User fills in the **form** and presses a button to submit information to the server. This informatio is sent in **key/value pairs**
- Every `<form>` element requires an `action` attribute, whose value is the URL for the page on the server that will receive the information being sent
- The `<input>` element within the `<form>` element is used to create different kinds of **form controls**
- Types of `<input>` attributes include
  - `"text"`
  - `"password"`
  - `"radio"`
  - `"checkbox"`
  - `"text"`
  - `"file"`
  - `"image"`

## HTML Chapter 14: “Lists, Tables & Forms” (pp.330-357)

- CSS includes many properties that can be used to style HTML elements like lists, tables, and forms
- These include:
  - `list-style-type`
  - `list-style-image`
  - `list-style-position`
  - `list-style`
  - `empty-cells`
  - `border-spacing`
  - `border-collapse`
  - `list-style-type`
- These properties can make forms easier to read and use, which will increase user interaction
- Form controls can be vertically aligned within the form to make the form easier to use, as well

## JavaScript Chapter 6: “Events” (pp.243-292)

- JavaScript is able to respond to events that happen when a user interacts with the browser

1. Interactions create **events** (event is **"fired"** or **"raised"**)
2. Events **trigger** code. We control this as programmers:
>
> - We select the element node(s) we want the script to respond to
> - We indicate which event on the node(s) will trigger the response, and **bind** the event to that node
> - We state the code we want to run when the event is triggered
>
3. Code responds to users (interactivity!)

### Binding an event to an element

- **DOM event handler**:

```
el.onblur = checkUsername;
```

- **Event listener**:

```
elUsername.addEventListener('blur', checkUsername, false);
```

- You can pass arguments into event handlers or event listeners, but since you cannot have parentheses after the function names, the code gets a little funky:

```
let elUsername = document.getElementById('username');
let elMsg = document.getElementById('feedback');

function checkUsername(minLength) {
  if (elUsername.value.length < minLength) {
    elMsg.textContent = 'Username must be ' + minLength + 'characters or more';
  } else {
    elMsg.innerHTML = '';
  }
}

elUsername.addEventListener('blur', function() {
  checkUsername(5);
}, false);
```

[Back to Home](../README.md)
