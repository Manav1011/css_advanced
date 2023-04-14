#### CSS Flexbox is a layout module that allows you to create flexible and

responsive layouts. It provides a more efficient way to align,
distribute and space elements within a container, even if the
container's size is not known beforehand.


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
