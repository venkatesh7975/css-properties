# CSS Properties Documentation

This document provides a detailed explanation of the CSS properties used in the `style.css` file. Each section covers specific properties, their values, descriptions, and examples.

## Table of Contents

1. [Reset](#reset)
2. [General Styles](#general-styles)
3. [Containers](#containers)
4. [Colors Section](#colors-section)
5. [Positioning Section](#positioning-section)
6. [Backgrounds Section](#backgrounds-section)
7. [Borders Section](#borders-section)
8. [Box Model Section](#box-model-section)
9. [Transitions and Animations Section](#transitions-and-animations-section)
10. [Typography Section](#typography-section)
11. [Display Section](#display-section)
12. [Footer](#footer)

## Reset

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

- `margin: 0;`: Resets the margin of all elements to zero.
- `padding: 0;`: Resets the padding of all elements to zero.
- `box-sizing: border-box;`: Changes the box model to include padding and border within the element's total width and height.

## General Styles

```css
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  background: #f4f4f4;
  color: #333;
}
```

- `font-family: Arial, sans-serif;`: Sets the font of the text to Arial with a fallback to sans-serif.
- `line-height: 1.6;`: Sets the line height to 1.6 times the font size.
- `background: #f4f4f4;`: Sets the background color to a light grey.
- `color: #333;`: Sets the text color to a dark grey.

## Containers

```css
.container {
  width: 80%;
  margin: auto;
  overflow: hidden;
}
```

- `width: 80%;`: Sets the container's width to 80% of its parent.
- `margin: auto;`: Centers the container horizontally.
- `overflow: hidden;`: Hides overflow content.

## Colors Section

```css
#colors {
  padding: 2rem;
  background: #fff;
}
.color-box {
  width: 100px;
  height: 100px;
  display: inline-block;
  margin: 0.5rem;
}
.bg-primary {
  background: #3498db;
}
.bg-secondary {
  background: #2ecc71;
}
.bg-tertiary {
  background: #e74c3c;
}
.text-primary {
  color: #3498db;
}
.text-secondary {
  color: #2ecc71;
}
.text-tertiary {
  color: #e74c3c;
}
```

- `padding: 2rem;`: Adds padding around the section.
- `background: #fff;`: Sets the background color to white.
- `.color-box`: Defines a box with specific dimensions and margins.
- `display: inline-block;`: Allows the box to sit inline with other elements while retaining block properties.

## Positioning Section

```css
#positioning {
  padding: 2rem;
  background: #fff;
}
.relative-box {
  position: relative;
  top: 20px;
  left: 20px;
}
.absolute-box {
  position: absolute;
  top: 20px;
  right: 20px;
}
.fixed-box {
  position: fixed;
  bottom: 20px;
  left: 20px;
}
.sticky-box {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
}
```

- `position: relative;`: Positions the element relative to its normal position.
- `position: absolute;`: Positions the element absolutely relative to its nearest positioned ancestor.
- `position: fixed;`: Fixes the element relative to the viewport.
- `position: sticky;`: Makes the element stick to a defined position within its scrollable container.

## Backgrounds Section

```css
#backgrounds {
  padding: 2rem;
  background: #f4f4f4;
}
.background-image {
  background: url("path/to/image.jpg") no-repeat center center/cover;
  height: 200px;
}
.background-gradient {
  background: linear-gradient(to right, #3498db, #2ecc71);
  height: 200px;
}
```

- `background: url('path/to/image.jpg') no-repeat center center/cover;`: Sets a background image with no repeat, centered, and scaled to cover the entire area.
- `background: linear-gradient(to right, #3498db, #2ecc71);`: Sets a linear gradient background.

## Borders Section

```css
#borders {
  padding: 2rem;
  background: #fff;
}
.borders-container div {
  margin-bottom: 1rem;
  padding: 1rem;
  text-align: center;
}
.border-solid {
  border: 2px solid #3498db;
}
.border-dashed {
  border: 2px dashed #e74c3c;
}
.border-dotted {
  border: 2px dotted #f1c40f;
}
.border-radius {
  border: 2px solid #9b59b6;
  border-radius: 10px;
}
```

- `border: 2px solid #3498db;`: Creates a solid border with a width of 2px and a color of #3498db.
- `border-radius: 10px;`: Rounds the corners of the border with a radius of 10px.

## Box Model Section

```css
#box-model {
  padding: 2rem;
  background: #f4f4f4;
}
.box-model-container div {
  margin-bottom: 1rem;
  padding: 1rem;
  text-align: center;
}
.box-padding {
  background: #3498db;
  color: #fff;
  padding: 20px;
}
.box-margin {
  background: #e74c3c;
  color: #fff;
  margin: 20px;
}
.box-border {
  background: #f1c40f;
  color: #fff;
  border: 5px solid #fff;
}
.box-content {
  background: #2ecc71;
  color: #fff;
  content: "Box with content";
}
```

- `padding: 20px;`: Adds padding inside the element.
- `margin: 20px;`: Adds margin outside the element.
- `border: 5px solid #fff;`: Creates a solid border with a width of 5px and a color of #fff.

## Transitions and Animations Section

```css
#transitions {
  padding: 2rem;
  background: #fff;
}
.transition-box {
  background: #3498db;
  color: #fff;
  padding: 1rem;
  text-align: center;
  transition: background 0.3s ease;
}
.transition-box:hover {
  background: #2ecc71;
}

@keyframes example-animation {
  0% {
    background: #e74c3c;
    transform: translateX(0);
  }
  50% {
    background: #f1c40f;
    transform: translateX(50px);
  }
  100% {
    background: #3498db;
    transform: translateX(0);
  }
}
.animation-box {
  background: #e74c3c;
  color: #fff;
  padding: 1rem;
  text-align: center;
  animation: example-animation 3s infinite;
}
```

- `transition: background 0.3s ease;`: Smoothly transitions the background color over 0.3 seconds.
- `@keyframes example-animation`: Defines an animation sequence.
- `animation: example-animation 3s infinite;`: Applies the animation with a 3-second duration and infinite repetition.

## Typography Section

```css
#typography {
  padding: 2rem;
  background: #f4f4f4;
}
.typography-container p {
  margin-bottom: 1rem;
  padding: 1rem;
  text-align: center;
}
.font-family {
  font-family: "Courier New", Courier, monospace;
}
.font-size {
  font-size: 1.5rem;
}
.font-weight {
  font-weight: bold;
}
.line-height {
  line-height: 2;
}
.letter-spacing {
  letter-spacing: 2px;
}
```

- `font-family: 'Courier New', Courier, monospace;`: Sets a specific font family.
- `font-size: 1.5rem;`: Sets the font size to 1.5 rem units.
- `font-weight: bold;`: Makes the font bold.
- `line-height: 2;`: Sets the line height to 2 times the font size.
- `letter-spacing: 2px;`: Adds 2px of spacing between letters.

## Display Section

```css
#display {
  padding: 2rem;
  background: #fff;
}
.display-container div {
  margin-bottom: 1rem;
  padding: 1rem;
  text-align: center;
}
.display-block {
  display: block;
  background: #3498db;
  color: #fff;
}
.display-inline {
  display: inline;
  background: #e74c3c;
  color: #fff;
}
.display-flex {
  display: flex;
  justify-content: center;
  background: #2ecc71;
  color: #fff;
}
.display-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  background: #f1c40f;
  color: #fff;
}
```

- `display: block;`: Makes the element a block-level element.
- `display: inline;`: Makes the element an inline element.
- `display: flex;`: Applies flexbox layout to the element.
- `display: grid;`: Applies grid layout to the element.

## Footer

This file provides a comprehensive guide to the CSS properties used in the stylesheet. For further information, please refer to the official [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS).

```

## Conclusion
This `README.md` file explains every CSS property used in the `style.css` file with detailed descriptions and examples. By following this documentation, you can gain a comprehensive understanding of the CSS properties and how to use them effectively in your web projects.
```
