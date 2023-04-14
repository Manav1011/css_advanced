- A CSS media query is a feature in CSS that allows you to apply different styles based on the characteristics of the device or browser that is being used to view your website. For example, you can use a media query to apply different styles to your website when it's viewed on a small mobile device versus a larger desktop computer.
  ```css
  /* Styles for screens smaller than 600px */
  @media (max-width: 600px) {
    body {
      background-color: lightblue;
    }
  }

  /* Styles for screens larger than 600px */
  @media (min-width: 600px) {
    body {
      background-color: lightgray;
    }
  }
  ```

###### Here are some more examples

```scss
@media (min-width: 600px) and (max-width: 1024px) {
  /* Styles for screens between 600px and 1024px */
  /* ... */
}

```

```css
@media (orientation: portrait), (orientation: landscape) {
  /* Styles for screens in either portrait or landscape mode */
  /* ... */
}

```
