# Flexbox vs Grid

Flexbox and CSS Grid are both powerful layout systems in CSS that allow
developers to create complex, responsive designs with ease. While both
offer similar functionality, they have different use cases and are
suited to different situations.

Flexbox is designed for one-dimensional layouts, where content is arranged along a single axis, either horizontally or vertically. It's best suited for creating flexible and dynamic layouts that adapt to changes in screen size and content.

CSS Grid, on the other hand, is designed for two-dimensional layouts,
where content is arranged in rows and columns. It allows for more
precise control over layout and is best suited for creating complex
grid-based designs.

Here are some key differences between Flexbox and CSS Grid:

### **Flexbox:**

* Is one-dimensional, meaning it controls either rows or columns, but not both at the same time.
* Is ideal for laying out items in a single row or column.
* Uses the `flex` property to control the layout of items within a container.
* Works well for creating responsive layouts that need to adapt to different screen sizes.
* Is useful for centering items both horizontally and vertically.


Here's an example of how to use Flexbox to center items within a parent container:

```css
.parent {
  display: flex;
  justify-content: center; /* centers items horizontally */
  align-items: center; /* centers items vertically */
}
```

### **CSS Grid:**

* Is two-dimensional, meaning it controls both rows and columns at the same time.
* Is ideal for creating complex grid-based layouts.
* Uses the `grid` property to control the layout of items within a container.
* Allows for precise control over the placement of items within a grid.
* Works well for creating both fixed and responsive layouts.

Here's an example of how to use CSS Grid to create a grid-based layout:

```css
.parent {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr; /* creates three columns of equal width */
  grid-template-rows: 100px 200px; /* creates two rows of specific heights */
  grid-gap: 10px; /* adds 10px of space between each grid item */
}
.child {
  grid-column: 2 / 3; /* places the item in the second column */
  grid-row: 1 / 2; /* places the item in the first row */
}

```
