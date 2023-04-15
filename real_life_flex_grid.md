# Real life flex-vs-grid

Sure, here are some real-life examples where Flexbox or CSS Grid can be used with examples:

### **Flexbox:**

##### * Navigation menus:

* Flexbox can be used to create horizontal or vertical
  navigation menus that are easy to navigate on different screen sizes.

```css
<nav class="nav-menu">
  <a href="#">Home</a>
  <a href="#">About</a>
  <a href="#">Services</a>
  <a href="#">Contact</a>
</nav>

<style>
.nav-menu {
  display: flex;
  flex-direction: row; /* or column for vertical navigation menu */
  justify-content: space-between; /* evenly distributes navigation items */
  align-items: center; /* vertically centers navigation items */
}
.nav-menu a {
  margin: 0 10px; /* adds spacing between navigation items */
}
</style>
```



##### Pricing tables

Flexbox can be used to create responsive pricing tables with evenly spaced columns and rows.

```css
<div class="pricing-table">
  <div class="pricing-column">
    <h3>Basic</h3>
    <p class="price">$9.99/month</p>
    <ul>
      <li>1GB storage</li>
      <li>10 users</li>
    </ul>
    <button>Sign Up</button>
  </div>
  <div class="pricing-column">
    <h3>Standard</h3>
    <p class="price">$19.99/month</p>
    <ul>
      <li>5GB storage</li>
      <li>50 users</li>
    </ul>
    <button>Sign Up</button>
  </div>
  <div class="pricing-column">
    <h3>Premium</h3>
    <p class="price">$49.99/month</p>
    <ul>
      <li>25GB storage</li>
      <li>unlimited users</li>
    </ul>
    <button>Sign Up</button>
  </div>
</div>

<style>
.pricing-table {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between; /* evenly distributes pricing columns */
  align-items: center; /* vertically centers pricing columns */
}
.pricing-column {
  flex: 1; /* evenly distributes pricing columns */
  max-width: 300px;
  padding: 20px;
  text-align: center;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  margin-bottom: 20px;
}
.price {
  font-size: 2em;
  margin: 20px 0;
}
button {
  background-color: #4CAF50;
  color: white;
  border: none;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 10px 0;
  border-radius: 5px;
}
</style>
```


##### Flexible content containers:

Flexbox can be used to create flexible content containers that adjust
their size and position based on the amount of content they contain.

```html
<div class="content-container">
  <h2>Flexible Content Container</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed eu felis dapibus, dapibus velit in, malesuada dolor. Vestibulum at sapien dolor. Integer nec est lobortis, auctor augue non, feugiat eros. Praesent ullamcorper sodales ex, nec aliquet est semper et</p>
</div>

<style>
.content-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: flex-start; /* aligns content items to the top of the container */
  padding: 20px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  width: 100%;
}
.content-container h2 {
  flex-basis: 100%; /* ensures heading takes up full width of container */
  margin-bottom: 10px;
}
.content-container p {
  flex-basis: calc(50% - 10px); /* sets width of paragraphs to 50% minus 10px for margin */
  margin: 0 0 10px 0;
}
</style>

```


### **CSS Grid:**

##### Image gallery:

CSS Grid can be used to create an image gallery with evenly spaced rows
and columns, and responsive resizing for different screen sizes.

```html
<div class="image-gallery">
  <img src="image1.jpg" alt="Image 1">
  <img src="image2.jpg" alt="Image 2">
  <img src="image3.jpg" alt="Image 3">
  <img src="image4.jpg" alt="Image 4">
  <img src="image5.jpg" alt="Image 5">
  <img src="image6.jpg" alt="Image 6">
</div>

<style>
.image-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* evenly spaces images in rows and columns */
  grid-gap: 10px;
}
.image-gallery img {
  width: 100%;
  height: auto;
}
</style>

```


##### Responsive page layouts:

CSS Grid can be used to create responsive page layouts with multiple
content sections that rearrange themselves based on the screen size.

```html
<div class="page-layout">
  <header>Header</header>
  <nav>Navigation</nav>
  <main>Main Content</main>
  <aside>Sidebar</aside>
  <footer>Footer</footer>
</div>

<style>
.page-layout {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-areas:
    "header"
    "nav"
    "main"
    "aside"
    "footer";
}
@media screen and (min-width: 768px) {
  .page-layout {
    grid-template-columns: repeat(2, 1fr);
    grid-template-areas:
      "header header"
      "nav main"
      "aside main"
      "footer footer";
  }
}
@media screen and (min-width: 1024px) {
  .page-layout {
    grid-template-columns: repeat(3, 1fr);
    grid-template-areas:
      "header header header"
      "nav main aside"
      "footer footer footer";
  }
}
header { grid-area: header; }
nav { grid-area: nav; }
main { grid-area: main; }
aside { grid-area: aside; }
footer { grid-area: footer; }
</style>
```


##### Form layouts

CSS Grid can be used to create form layouts with evenly spaced labels
and input fields that adjust their size and position based on the amount
 of content they contain.

```html
<form class="form-layout">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
</form>

<style>
.form-layout {
  display: grid;
  grid-template-columns: 1fr 2fr; /* sets two equal columns for labels and input fields */
  grid-gap: 10px;
}
.form-layout label {
  text-align: right;
}
.form-layout input[type="text"],
.form-layout input[type="email"] {
  width: 100%;
  padding: 5px;
}
</style>

```


## Use Flexbox for:

* Navigation menus: You can use flexbox to align navigation items horizontally, such as a menu bar at the top of a website.
* Forms: You can use flexbox to align form labels and inputs in a single row or column.
* Small content sections: You can use flexbox to vertically center content in a small content section, such as a pricing table or product card.

## Use CSS Grid for:

* Full page layouts: You can use CSS Grid to create full page layouts with multiple content sections that adjust to different screen sizes and device types.
* Image galleries: You can use CSS Grid to position and resize images in an image gallery with equal spacing between them.
* Card-based interfaces: You can use CSS Grid to create card-based interfaces with multiple cards that resize and rearrange themselves based on the available space.
