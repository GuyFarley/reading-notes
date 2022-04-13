# Code 201 - Class 08 - More CSS Layout

## [Learn CSS - Layout](https://web.dev/learn/css/layout/)

- The `display` property does two things:
  1. Determines if the box it's applied to acts as inline or block
  >
  >- **Inline elements** sit next to each other in an inline direction
  >- **Block elements** create new lines for themselves
  >
  2. It also determines how an element's children should behave

### Flexbox

- Single-axis layout
- Aligns an element's children next to each other in the inline direction
- Stretches the element's children in the block direction so they're all the same height
- Also converts the child elements to be flex items, allowing you to control how they behave inside the container. Example:

```
.my-element div {
  flex-grow: 1;
  flex-shrink: 0;
  flex-basis: auto;
}
```

### Grid

- Multi-axis layout
- `fr` unit ("franction of remaining space") example: build 12 column grids, with a gap between each item:

```
.my-element {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 1rem;
}
```

- `inline-block` requires surrounding elements to respect block margin or padding on an inline element (like a block element would)
- CSS multicolumn allows you to split a list into multiple columns. Example:

```
.countries {
  column-count: 2;
  column-gap: 1em;
}
```

-------------------------

## Duckett HTML/CSS book: Ch. 15, “Layout” (Revisited...)

*As reviewed previously:*

- CSS treats each HTML element as if it lives in its own box
- These boxes can be **block-level** or **inline**
  - **Block-level** elements start on a new line
  - **Inline** elements flow in between surrounding text
- Containing elements (or parent elements) are block-level elements that contain other block-level elements inside them (for instance, all elements of a footer would be contained within the parent element `<footer>` or `<div>`)
- There are many positioning schemes that CSS provides, which help you control the layout of a page:
  - **Normal flow**: Elements appear one after the other, vertically
  - **Relative positioning**: Elements can be shifted up, down, left, or right (as compared to where they would have been placed)
  - **Absolute positioning**: Positioning an element in relation to its containing element
  - **Fixed positioning**: Similar to absolute positioning, but positions an element in relation to the browser window instead
  - **Floating elements**: Positions an element to the far left or far right of its containing box
- There are many variations in screen size and resolution that users will use to access your site, so this must be taken into account when desiging your page
- CSS frameworks such as **960.GS** make it much easier to style web pages by providing a grid that can help you control and style your elements
  - Class names are used within the HTML to direct the framework how to place boxes on the grid
  - **960.GS** takes care of the layout, leaving us to handle the fonts, coloring, etc.

[Back to Home](../README.md)
