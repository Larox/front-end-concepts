# CSS Positioning Layouts

## Flexbox:

Flexbox is a layout technique in CSS that allows you to create flexible and
responsive layouts with ease. It works by dividing a container into flexible
rows or columns, which can then be used to position and align items within the
container.

Example of how to use Flexbox to create a centered layout:

```css
.container {
  display: flex; /* Tell the browser to use flex*/
  justify-content: center; /* center content horizontally*/
  align-items: center; /* center content vertically */
}
```

## CSS Grid

CSS Grid is another layout technique in CSS that allows you to create more
complex and structured layouts. It works by dividing a container into a grid of
rows and columns, which can then be used to position and align items within the
container.

Example of how to use CSS Grid to create a grid of items:

```css
.container {
  display: grid; /* Tell the browser to use css grid*/
  grid-template-columns: repeat(3, 1fr); /* number of columns */
  grid-gap: 10px;
}

.item {
  grid-column: span 1; /* space to use in the column */
  grid-row: span 1; /* space to use in the row */
}
```

## Positioning

CSS Positioning is a technique that allows you to position elements on a page
using coordinates or relative positioning. You can use absolute positioning,
relative positioning, fixed positioning, or sticky positioning to achieve
different layouts.

Example of how to use CSS Positioning to create a fixed navbar:

```css
.navbar {
  position: fixed; /**/
  top: 0;
  left: 0;
  width: 100%;
  background-color: #333;
  color: #fff;
}
```
