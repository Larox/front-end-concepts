# Relative Measures

## em

Unit equal to the relative length unit that is based on the computed value of
the element on which it is used. `1em` is equal to the computed `font-size` of
the element.

For example, if the font-size of a paragraph element is set to 16px, then 1em is
also equal to 16px. If you set the font-size of a child element to 1.5em, then
the computed font-size of the child element will be 1.5 times the computed
font-size of the parent element.

One of the benefits of using em units is that they are relative to the font size
of the element, which means that they will scale proportionally if the font size
of the element changes. This can be useful for creating responsive layouts that
adjust to different screen sizes.

```css
.container {
  font-size: 16px; /* 1em*/
}

.box {
  font-size: 1.5em; /* 1.5em * 16px = 24px */
  padding: 1em; /* Now 1em = 24px since font-size new value is 24px */
}

@media screen and (max-width: 768px) {
  .container {
    font-size: 14px; /* this will be the value to compute 1em for 768px screen size*/
  }
}
```

## rem

rem unit is relative to the font-size of the root element instead of the element
itself, like em.

The benefit of using rem units is that they are not affected by the font-size of
the element on which they are used, which can make it easier to maintain
consistent spacing and layout across the site, especially when different
elements have different font sizes.

```css
html {
  font-size: 16px; /* root element*/
}

.container {
  font-size: 1.2rem; /* 16px * 1.2: 19.2px */
  padding: 1rem; /* from root element: 16px */
}

@media screen and (max-width: 768px) {
  html {
    font-size: 14px; /* root element font-size for 758px screen size */
  }
}
```

## vw/vh

These are relative length units to the width and height of the viewport, or visible area of the browser

### vw

Viewport width, 1vw = 1% of the width of the viewport.

Example: viewport width = 1000px -> 1vw = 10px

### vh

Viewport height, 1vh = 1% of the width of the viewport.

Example: viewport height = 800px -> 1vh = 8px

The benefit of using vw and vh units is that they allow you to create responsive
designs that are based on the size of the viewport, rather than the size of the
content or the device. This can be useful for creating layouts that adjust to
different screen sizes and aspect ratios.

```css
.box {
  width: 50vw; /* width: 50% of viewport width */
  height: 50vh; /* height: 50% of viewport height */
  font-size: 2vw; /* font-size: 2% of viewport width */
}

@media screen and (max-width: 768px) {
  .box {
    width: 100vw; /* width: 100% of viewport width */
    height: 30vh; /* height: 30% of viewport height */
    font-size: 3vw; /* font-size: 3% of viewport width */
  }
}
```

## Percentages (%)

This is a relative lenght unit that is based on the size of the cointaining element.

The benefit of using % units is that they allow you to create layouts that are
relative to the size of the containing element, rather than fixed to a specific
size. This can be useful for creating responsive designs that adjust to
different screen sizes and resolutions.

Example:

```css
.container {
  width: 80%; /* width: 80% of containing element */
  margin: 0 auto; /* center horizontally */
}

.box {
  width: 50%; /* width: 50% of containing element */
  float: left;
}

@media screen and (max-width: 768px) {
  .box {
    width: 100%; /* width: 100% of containing element */
    float: none;
  }
}
```
