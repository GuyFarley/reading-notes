# Code 201 - Class 14a - CSS Transforms, Transitions, and Animations

## [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

- The `transform` property is new with CSS3 and brings some new techniques for positioning elements on a page
- This property can be used for 2D or 3D transformation

### 2D Transforms

- 2D transforms work on the horizontal and vertical (x and y) axes
- Values that can be used with the `transform` property for 2D include:
  - `rotate` - Rotates an element from 0 to 360 degrees
  - `scale` - Changes the appeared size of an element
  - `translate` (and `translateX` and `translateY`) - Moves the element in different directions without interrupting the normal flow of the document
  - `skew` (and `skewX` and `skewY`) - Distorts an image
  - `transform-origin` - Changes the origin position for transforming an element
  - `perspective` - Modifies the **vanishing point** for 3D drawings

### 3D Transforms

- `rotateX`, `rotateY`, and `rotateZ`
- `scaleZ`
- `translateZ`

## [CSS Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

- CSS3 also offers the ability to create transitions and animations without the need for Flash or JavaScript

### Transitions

- Transitions require an element to have a change of state, with different styles applied to each state
- Use the `:hover`, `:active`, `:focus`, and `:target` pseudo-clases to determine styles for these different states
- `transition-property` - Determines which properties will be altered in combination with the other transitional properties below
- A property must have an identifiable halfway point in order to be transitioned. These properties include:
  - `background-color`
  - `text-shadow`
  - `right`
  - `width`
  - `opacity`
  - and many others...
- `transition-duration` defines the time period over which the transition takes place, and can be set using seconds and milliseconds
- `transition-timing-function` sets the spead at which a transition will occur
- A "card flip" transition can be written using the following HTML and CSS code:

```
<div class="card-container">
  <div class="card">
    <div class="side">...</div>
    <div class="side back">...</div>
  </div>
</div>
```

```
.card-container {
  height: 150px;
  perspective: 600;
  position: relative;
  width: 150px;
}
.card {
  height: 100%;
  position: absolute;
  transform-style: preserve-3d;
  transition: all 1s ease-in-out;
  width: 100%;
}
.card:hover {
  transform: rotateY(180deg);
}
.card .side {
  backface-visibility: hidden;
  height: 100%;
  position: absolute;
  width: 100%;
}
.card .back {
  transform: rotateY(180deg);
}
```

### Animations

- Animations require transitions to have multiple states
- The `@keyframes` rule includes the animation name, breakpoints, and properties to be animated. Properties to include:
  - `animation-name`
  - `animation-duration`
  - `animation-timing-function`
  - `animation-delay`
- Animations can be customized, as well
  - `animation-iteration-count` can determine how many times the animation will run, for instance (rather than stopping at one iteration)
  - `animation-play-state` will allow an animation to be paused and resumed when buttons are pushed

## [8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

- There are many transitions that can be easily added to a site that will elevate its impact! These include:
  - Fade in
  - Change color
  - Grow and Shrink
  - Rotating elements
  - Square to circle
  - 3D shadowing
  - Swing
  - Inset border

[Back to Home](../README.md)
