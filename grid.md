# Grid

* CSS Grid Layout is a powerful layout system that allows web developers
  to create complex and responsive layouts with ease. It is a
  two-dimensional grid-based layout system that allows you to arrange HTML
  elements into rows and columns.
* The grid is defined by creating a parent container and specifying the
  number of rows and columns in the grid. This is done using the `grid-template-columns` and `grid-template-rows`
  properties. You can define the size of each row and column using
  various units like pixels, percentages, or fractions of available space.
* Once the grid is defined, you can place HTML elements in specific cells of the grid using the `grid-column` and `grid-row` properties. You can also use the `grid-area` property to assign a name to a grid cell and then place an HTML element in that cell using the name.
* CSS Grid also provides many advanced features such as grid gaps, grid
  alignment, and the ability to create responsive layouts. Grid gaps allow
  you to add space between grid cells, while grid alignment allows you to
  align items within the grid both horizontally and vertically.
* Overall, CSS Grid is a powerful layout system that provides web
  developers with a flexible and easy-to-use solution for creating complex
  and responsive layouts on the web.

#### Parent container

Here's an explanation of all the CSS Grid Layout parent container properties with examples and values:

`display`

This property is used to define the type of layout container. To use CSS Grid, you need to set the display property to `grid`.

```css
.container {
  display: grid;
}
```

`grid-template-columns`

This property defines the number and size of columns in the grid. You can use different units to define the size of the columns, such as pixels, percentages, or fractions of the available space.

```css
.container {
  display: grid;
  grid-template-columns: 100px 1fr 2fr;
}
```

`grid-template-rows`

This property defines the number and size of rows in the grid. It works similarly to `grid-template-columns`.

```css
.container {
  display: grid;
  grid-template-columns: 100px 1fr 2fr;
  grid-template-rows: 50px 1fr;
}
```

This will create two rows in the grid, with the first row being 50 pixels tall and the second row taking up one fraction of the available space.

`grid-gap`

This property defines the size of the gap between rows and columns in
the grid. You can use different units to define the size of the gap,
such as pixels, percentages, or ems.

```css
.container {
  display: grid;
  grid-template-columns: 100px 1fr 2fr;
  grid-template-rows: 50px 1fr;
  grid-gap: 10px;
}
```

`justify-items` and `align-items`

These properties define how the items in the grid are aligned both horizontally and vertically.

```css
.container {
  display: grid;
  grid-template-columns: 100px 1fr 2fr;
  grid-template-rows: 50px 1fr;
  justify-items: center;
  align-items: center;
}
```

This will center all items both horizontally and vertically in the grid. These are the most commonly used CSS Grid parent container properties, but there are many more available that allow you to create even more complex and flexible layouts.

#### align-content vs align-items

In CSS Grid Layout, `align-content` and `align-items`  are two properties that are used to align grid items  vertically within the grid container. However, they have slightly different behaviors.

`align-items` aligns items along a single row or column, whereas `align-content` aligns rows or columns as a group.

`align-items`

This property aligns items along a single row or column axis.

```css
.container {
  display: grid;
  align-items: center;
}
```

In the example above, the `align-items` property is set to `center`, which aligns all items in the center of their row or column.

`align-content`

This property aligns rows or columns as a group within the grid container.

```css
.container {
  display: grid;
  align-content: center;
}
```


In the example above, the `align-content` property is set to `center`, which centers all rows or columns as a group within the grid container.

If there is only one row or column in the grid, `align-items` and `align-content` will have the same effect. However, if there are multiple rows or columns, the difference between the two becomes apparent.

For example, if there are multiple rows in the grid and the `align-items` property is set to `center`, each row will be centered individually. On the other hand, if the `align-content` property is set to `center`, all rows will be centered as a group within the grid container.

In summary, `align-items` aligns items along a single row or column axis, while `align-content` aligns rows or columns as a group within the grid container.


#### **Child container**
