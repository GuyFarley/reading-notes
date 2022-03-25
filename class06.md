# Class 06: Activate Web Pages with JavaScript

## What is JavaScript?

Well, we've covered two languages so far: HTML and CSS. Isn't that enough already? No way! **JavaScript** is what actually makes a web page interactive! If **HTML** is what you read, and **CSS** is what you see, then **JavaScript** is what you *do*.

In a more technical sense, JavaScript is a programming language with first-class functions (functions in JS are treated like any other variable). For example, in such a language, a function can be passed as an argument to other functions, can be returned by another function and can be assigned as a value to a variable (from [MDN's Glossary](https://developer.mozilla.org/en-US/docs/Glossary/First-class_Function)).

Of course, we know JavaScript as a scripting language for web pages--but it is used in a multitude of non-browser environments as well.

## So what does it do?

Ultimately, JavaScript's job is to listen to user input. Based on this input, output is fed back to the user. In this way, it makes websites interactive and dynamic! And of course, more effective at driving revenue.

As noted on [W3Schools](https://www.w3schools.com/js/tryit.asp?filename=tryjs_variables_undeclared) website, here's an example of how JavaScript interacts with HTML (where the JavaScript can be found inside the *script* tags):
```
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Variables</h2>

<p>In this example, x, y, and z are variables.</p>

<p id="demo"></p>

<script>
let x = 5;
let y = 6;
let z = x + y;
document.getElementById("demo").innerHTML =
"The value of z is: " + z;
</script>

</body>
</html>
```
I look forward to learning much more about JavaScript and will provide updates as I learn!

[Back to Home](README.md)