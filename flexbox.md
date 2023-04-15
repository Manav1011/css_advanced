#### CSS Flexbox is a layout module that allows you to create flexible and

responsive layouts. It provides a more efficient way to align,
distribute and space elements within a container, even if the
container's size is not known beforehand.

## Parent-container

`flex-direction`

This property determines the direction of the main axis of the Flexbox container, and can take one of four values: `row` (default), `row-reverse`, `column`, or `column-reverse`.

```css
.container {
  display: flex;
  flex-direction: row;
}

```

`justify-content`

* his property determines how the child elements are distributed along the
  main axis of the Flexbox container, and can take one of six values: `flex-start` (default), `flex-end`, `center`, `space-between`, `space-around`, or `space-evenly`.

```css
.container {
  display: flex;
  justify-content: center;
}

```

`align-items`

This property determines how the child elements are aligned along the
cross axis of the Flexbox container, and can take one of five values: `stretch` (default), `flex-start`, `flex-end`, `center`, or `baseline`.

```css
.container {
  display: flex;
  align-items: center;
}

```

`flex-wrap`

This property determines whether the child elements should wrap onto a
new line when they exceed the width of the container. It can take one of
 three values: `nowrap` (default), `wrap`, or `wrap-reverse`.

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

`align-content`

This property determines how the child elements are distributed along
the cross axis of the container when there is extra space in the
container. It can take one of six values: `stretch` (default), `flex-start`, `flex-end`, `center`, `space-between`, or `space-around`.

```css
.container {
  display: flex;
  align-content: center;
}
```


## Child-Containers

`flex-grow`

This property determines how much the child elements should grow to
fill any available space in the container along the main axis. It takes a
 numeric value, with `0` being the default value (meaning the child will not grow).

```css
.child {
  flex-grow: 1;
}
```


`flex-shrink`

This property determines how much the child elements should shrink to
fit within the container if there is not enough space along the main
axis. It takes a numeric value, with `1` being the default value.

```css
.child {
  flex-shrink: 0;
}

```

`flex-basis`

This property determines the initial size of the child elements along
the main axis before any free space is distributed. It can take a length
value or a keyword value such as `auto` (default).

```css
.child {
  flex-basis: 50%;
}
```

`align-self`

This property overrides the `align-items` property on the
parent container for a single child element. It determines how the child
should be aligned along the cross axis of the container, and can take
the same values as `align-items`.

```css
.child {
  align-self: flex-end;
}
```
