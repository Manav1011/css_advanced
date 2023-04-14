* ***The `display` property in CSS determines how an element is displayed on the page. There are several values that the `display` property can take, each with its own specific behavior. Here are some of the most common `display` property values and their meanings, along with examples:***

`block` - Elements with `display: block` take up the full width of the parent container and create a new line after them. Examples of elements that default to `display: block` include `<div>`, `<p>`, and `<h1>-<h6>` tags.

```css
div {
  display: block;
}

```

`inline` - Elements with `display: inline` take up
 only as much width as necessary to fit their content, and do not create
 new lines after them. Examples of elements that default to `display: inline` include `<span>`, `<a>`, and `<img>` tags.

```css
`span {   display: inline; } `
```

`inline-block` - Elements with `display: inline-block`
 behave like inline elements, but can also have width, height, padding,
and margin properties applied to them. This makes them useful for
creating elements that need to be horizontally aligned, such as buttons
or images.

```css
button {
  display: inline-block;
  width: 100px;
  height: 40px;
  margin: 10px;
  padding: 5px;
}

```

`flex` - Elements with `display: flex` create a
flexible container that can be used to create flexible layouts. Flexbox
allows for easy alignment and distribution of elements within the
container.

```css
.container {
  display: flex;
  justify-content: space-between;
}

```

`grid` - Elements with `display: grid` create a
two-dimensional grid layout. Grid allows for even more fine-grained
control of layout than Flexbox, and allows for the creation of complex,
responsive layouts.

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 10px;
}

```
