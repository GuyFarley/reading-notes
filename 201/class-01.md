# Code 201 - Class 01: Introductory HTML and JavaScript

## Why this matters

*HTML*, *CSS*, and *JavaScript* all work together to create the experience of a web page. So it makes sense to understand the basics of each of these languages first: What they accomplish, their basic syntax, and how they work with each other. It's also important to look at the bigger picture of how a web page is designed, from identifying its target audience to deciding how they will interact with the site, before determining how the various languages should work together to accomplish your goals.

## HTML Chapter 1: "Structure"

In HTML, *elements* (or *tags*) are used to describe the structure of a page. In addition to the tags themselves (usually an opening and closing tag, wrapped around content) there are also attributes that can be included in the tags, to provide more information about the element's content.

>The structure that these elements create can be thought of as the "blueprint" of the final rendered page. As a metaphor, let's consider the manufacturing of a car. These HTML elements would indicate the various pieces that are used to build that car. They would tell you that the car has 4 wheels, 2 doors, a windshield, etc. They would also tell you roughly where those pieces were located in relation to the car itself. But they wouldn't tell you the color of the car, the size of the wheels, or the angle of the windshield.  

## HTML Chapter 8: "Extra Markup"

There's a fair amount of additional markup that can be used in HTML: Tags that don't necessarily fit into specific groups or sections. These include *DOCTYPE declarations* (which indicate the version of HTML being used), *comments*, *id* and *class* attributes (which can uniquely identify specific elements or types of elements), and the *meta* element (which contains additional information about your page, but is not viewable to the user).

Additionally, *escape characters* can be used to include special characters in your document, or to show characters that are otherwise reserved for HTML code. For example, rather than using an ampersand (&) which is a reserved character, you can instead write *&amp* or *&#38*.

>Going along with the car example, maybe this particular car is a DeLorean and needs to include a flux capacitor. Doesn't quite fit into a standard category of car components, does it? You might need a unique way to identify that flux capacitor, and maybe an *id* attribute would help to identify such a unique element.

## HTML Chapter 17: "HTML5 Layout"

With HTML5, some new elements have been created to help describe the purpose of the element. These "semantic" elements allow for code to be understood more clearly. For example: Before HTML5, all different sections on a page might have been grouped together into *div* elements, with class or id attributes then used to identify the role of those sections. But with HTML5, there are now specific elements that can be used in place of *div* that will indicate the role of each section (*header*, *article*, and *nav*, to name a few).

>On your DeLorean engineering drawings, which are really starting to take shape by now, you may want to distinguish the trunk from the rest of the interior (assuming DeLoreans have trunks). You would use the semantic element name "trunk" on your blueprint to indicate that the trunk is separate from the rest of the interior. Same idea here - these new HTML5 elements make it that much easier for someone to read the drawings and know exactly what they're looking at.

## HTML Chapter 18: "Process & Design"

Before ever putting fingers to keys, there's a lot of important thought that needs to go into how a website will function. You need to understand who your target audience is, what information they'll be looking for, and how you want them to respond to your content. This information should be used to very intentionally plan out your site's structure and design--not only to make your site as effective as possible, but to build your code (I imagine) in the cleanest, most efficient way possible.

To do this, you need to understand:

- Why people are visiting your site
- What they hope to achieve when they get there
- What information they will need

From a design perspective, you'll want the site to be easy to navigate, intuitive, and visually communicative (not to mention easy on the eyes). You'll need to use groupings of colors, styles, and font sizes to clearly show how the information is divided.

>This is a thought process I'm familiar with from my previous career in retail marketing, where I managed the design and production of in-store retail displays. Oftentimes these were full rollouts of displays within each store--and they started with the window displays (drawing the customer through the doors) and progressed through the store: Door clings, 3D displays inside the main entrance, and shelf displays at the point of sale. This required a lot of forethought to determine a message hierarchy, and how the customer would be compelled to buy the product as they made their way through the store to the product itself. These marketing displays started in much the same way our websites will: first, with an idea that was used to develop an initial design concept. Then becoming 3D renderings, engineering drawings, physical prototypes, and ultimately a final product.

## JS Introduction

JavaScript is used to make web pages more interactive, and they can do this in a few ways:

- Accessing the content of a page
- Modifying content on a page
- Programming rules for the browser to follow
- Reacting to events (like when a button is pressed or an amount of time has passed)

An example of this is a slideshow, where JavaScript reacts to specific events, accesses image files, and modifies the content of a page - all of which result in a running slide show that occurs within a single space on the web page. This is not only more fun to look at than an stationary image, but allows for one piece of the page to become much more dynamic.

>Taking it back to retail displays for a sec, JavaScript would be like a QR Code that is included on a printed shelf strip. While the shelf strip alone would fully function as a printed piece, the QR Code is what allows interactivity between the graphic and the shopper. Another example would be a digital video screen embedded into a blade sign or aisle violator. The graphic would function just fine on its own, as a stationary printed image, but the ability to push a button and view a quick video creates interactivity that helps drive the sale.

## JS Chapter 1: “The ABC of Programming”

***What is a script and how do I create one?***

JavaScript uses *scripts* to instruct a computer to perform tasks. These are simply directions that a computer will follow in order to achieve a desired goal. In Course 102, we learned that computers are stupid and need to be told exactly what to do and how to do it. In other words, you need to explain the directions the way you would explain them to a 3-year-old child.

The best way to write a script is to determine your end goal, break it down in to a series of tasks, and then figure out the steps that are needed to complete each of those tasks.

***How do computers fit in with the world around them?***

We use computers to create models of the world, using data we provide. Within these models:

- Objects represent physical things
- Methods perform tasks using the properties of those objects
- Events can be triggered when a user interacts with the computer

Browsers help computers display these models by:

 1. Receiving the HTML code for a page
 2. Creating a model of that page and storing it in memory
 3. Showing the final rendered page on your computer screen

Browsers also include interpreters (or scripting engines) that translates JavaScript code into instructions the browser can read and then perform

***How do I write a script for a web page?***

JavaScript is written in plain text, and the browser then uses a lot more code behind the scenes to display what you need it to display. In this way it simplifies a web developer's job - the developer only needs to know how to write the script that asks the browser to use that behind-the-scenes code.

In order to make a script run in the HTML, you place the script element where you want to JavaScript code to run. The browser follows the code line-by-line, so it will not run your script until it comes across the script element. In this way you can control when and where your interactivity will take place within a web page.

Scripts utilize objects (which we know represent a thing) and methods (which we know perform tasks), written in a standard format, often referring to specific members of the object and parameters that are passed to the method.

Example:

```
 document.write('Good afternoon!');
```

Like CSS code, it's always best to keep JavaScript code in its own file (with the .js extension). This will ensure your HTML code stays clean, and creates a modularity between the languages that allows for easier updates and overall flexibility.

## Things I want to know more about

- Deeper understanding of the different versions of HTML
- Using grouping and similarity when designing a website
- Designing navigation
- Designing a script using a flowchart
- The Progressive Enhancement approach to building a web page

[Back to Home](../README.md)
