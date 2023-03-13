# Pseudo Classes

In CSS, a pseudo-class is a keyword that is added to a selector to style an
element when it is in a certain state or condition. Pseudo-classes allow you to
apply styles to elements based on user actions, such as hovering over an element
with the mouse or clicking on a link.

## :hover

This pseudo-class is used to apply styles to an element when the user hovers
over it with the mouse. For example, you can change the background color of a
button when the user hovers over it:

```css
button:hover {
  background-color: #ddd;
}
```

## :active

This pseudo-class is used to apply styles to an element when the user clicks on
it. For example, you can change the background color of a button when the user
clicks on it:

```css
button:active {
  background-color: #bbb;
}
```

## :focus

This pseudo-class is used to apply styles to an element when it has focus, such
as when a user clicks on a form field. For example, you can change the border
color of a form field when it has focus:

```css
input:focus {
  border-color: blue;
}
```

## :first-child

This pseudo-class is used to apply styles to the first child element of a parent
element. For example, you can style the first list item in a list differently
from the others:

```css
li:first-child {
  font-weight: bold;
}
```

## :nth-child()

This pseudo-class is used to apply styles to elements based on their position in
a parent element. You can use this pseudo-class to target every other element,
or every third element, and so on. For example, you can style every other row in
a table:

```css
tr:nth-child(even) {
  background-color: #f2f2f2;
}
```

These are just a few examples of the many pseudo-classes available in CSS.
Pseudo-classes allow you to add interactivity and visual cues to your website,
making it more engaging and user-friendly.
