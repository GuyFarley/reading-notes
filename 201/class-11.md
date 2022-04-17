# Code 201 - Class 11 - Assorted Topics

## Why this matters

- The audio/visual aspects of web pages (aside from just text and photos on a page) have become integral to most sites by now. These are valuable tools for communicating to the site's visitors more effectively and providing a more engaging experience. The info in these readings will help us to more easily implement photos, video, and audio into our sites for maximum user engagement

## HTML Chapter 16: “Images” (pp.406-427)

- CSS is an ideal way to place and resize images, since you can use it to apply styling rules to several images across your site
- You can align images using CSS by assigning different classes to each image, then applying style rules to those classes
- To center an image, you should use `display: block;` to turn the image into a block-level element. Then there are two ways to center the image:
  1. Apply `text-align: center` to the image's containing element
  2. Set the image's left and right margins to `auto`
- Background images can be set with the `background-image` property
- You can also use the `background-repeat` property to repeat an image, and control how the image repeats with values such as `repeat`, `repeat-x`, `repeat-y`, `no-repeat`, `fixed`, and `scroll`

## HTML Chapter 19: “Practical Information” (476-492)

- Search Engine Optimization (SEO) is the process of making your site more visible by influencing how closely it will appear to the top of search engine results
- There are techniques you can use both **on-page** and **off-page** to improve SEO
- On-page techniques include placing keywords in **seven different locations** on your page to improve SEO:
  1. Page title
  2. URL/Web address
  3. Headings
  4. Text
  5. Link text
  6. Image alt text
  7. Page descriptions
- You can use Google Analytics to analyze information about your site visitors, to give you better data regarding how visitors are using your site. This will help you answer questions like: How many visitors is your site getting? What are your visitors viewing on your site? Where are they coming from?
- In order to publish your site on the web, you will first need to get a domain name and web hosting service

## Video and Audio APIs (MDN Article)

- `<audio>` and `<video>` tags can be used to include audio and video in our web pages
- The `controls` attribute nables the default playback controls
- As an alternative to the standard tags and attributes, there is now (with HTML5) an `HTMLMediaElement` API that allows us to control video and audio players further
  - HTML can include `<button>` tags within `<div>` tags, both with classes specified for further styling and JavaScript
  - CSS can then be used to style the player and its buttons, opacity, etc.
  - Finally, JavaScript can be written to create the interactivity and control what actions take place when each button is pressed. Event handler functions can be added to control how the media player works when forward/rewind buttons are pressed, as well

## Things I want to know more about

- The `querySelector` method being used in the video/audio MDN article

[Back to Home](../README.md)
