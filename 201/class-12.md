# Code 201 - Docs for the HTML `<canvas>` Element & Chart.js

## Why this matters

- Graphics and charts can add visual interest and help to communicate data and ideas much more effectively than simple text. The tools described below provide some great methods for easily creating these visuals on your web page!

## [EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

- **Chart.js** is a JavaScript plugin that can be used to draw graphs onto a page using HTML's `<canvas>` element
  - `<canvas>` element is added to HTML page
  - A `<script>` is included at the foot of the body element to retrieve the context of the canvas
  - You can include labels, datasets, and options inside the `<script>` tag to control how the charts will render on the page

## Canvas API

- As noted above, you first create the **canvas environment** in the HTML
- A `draw()` function is included to create the blank template
- Canvas can only support two shapes: **rectangles** and **paths** (or lists of points connected by lines). There are many path drawing functions that can help us to create complex shapes
- You can draw a simple rectangle with code like the following:

```
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}
```

- In this example, `fillRect()` draws a black square 100 pixels on each side
- `clearRect()` then erases a 60x60 pixel square from the center
- `strokeRect()` then creates a rectangular outline 50x50 pixels inside the cleared square
- Drawing a path would be a similar process, with the following steps:
  1. Create the path
  2. Use **drawing commands** to draw into the path
  3. **Stroke** or **fill** the path to render it
- Various other functions can be used with `<canvas>` to do the following:
  - **Move the pen** - Moves the pen to specific coordinates on the page
  - Draw **lines**
  - Draw **arcs**
  - Create **bezier curves** and **quadratic curves**
  - And a combination of these to create all sorts of images

- There are also `<canvas>` options to help add different colors, line styles, gradients, patterns, and shadows. These properties include:
  - `fillStyle = color`
  - `strokeStyle = color`
  - `globalAlpha = transparencyValue`
  - `lineWidth = value`
  - `lineCap = type`
  - and many others...
- Finally, text can be rendered using the `fillText()` and `strokeText()` methods, and can be styled using the following properties:
  - `font = value`
  - `textAlign = value`
  - `textBaseline = value`
  - `direction = value`

## Things I want to know more about

- **Chart.js** and all its possible uses

[Back to Home](../README.md)
