<p  align="center">
<img  width="100%"  src="https://raw.githubusercontent.com/dennisfrijlink/development-utilities/cf7fdbdd8d7c0e43278bce968de518b8387d62a4/images/Flexboxgrid.svg"  alt="logo of React Single Page Application Repository">
</p>
<p  align="center">
A simple 12 columns, responsive CSS grid based on flexbox and the CSS library Bulma
</p>

## ✨ Quick Start
Download [flexboxgrid.css](css/flexboxgrid.css) and load the stylesheet

### Link import
```html
<link rel="stylesheet" href="flexboxgrid.css">
```
### CSS import
```css
@import url("flexboxgrid.css");
```
### JSX import
```js
import  './flexboxgrid.css';
```

For more examples check: https://bulma.io/documentation/columns/

## Key Features
* Reusable Columns- Reusable columns to divide your web application
* Sizes - Change the size per column
* Responsiveness - Handle  **different**  column layouts for each  **breakpoint**
* Nesting - A simple way to build  **responsive columns**
* Gap - Customize the  **gap**  between the columns
* Multiline - Make the columns multiline except for one row
* Centering columns - Instead of using _empty columns_ you can use `.is-centered` on the parent `.columns` element

## ⚙️ Usage
To split the view into columns, you just have to do two things:

 1. Add a ```columns``` container
 2. Add as many  ```column``` elements as you want

For example:
```html
<div class="columns">
  <div class="column">
    First column
  </div>
  <div class="column">
    Second column
  </div>
  <div class="column">
    Third column
  </div>
  <div class="column">
    Fourth column
  </div>
</div>
```

## Column sizes
You can define the  **size**  of each column  **individually**.

If you want to change the  **size**  of a single column, you can use one of the following classes:
-   `is-three-quarters`
-   `is-two-thirds`
-   `is-half`
-   `is-one-third`
-   `is-one-quarter`
-   `is-full`
-    `is-four-fifths`
-   `is-three-fifths`
-   `is-two-fifths`
-   `is-one-fifth`

The  _other_  columns will fill up the  **remaining**  space automatically.

### 12 columns system
As the grid can be divided into  **12**  columns, there are size classes for each division:
-   `is-1`
-   `is-2`
-   `is-3`
-   `is-4`
-   `is-5`
-   `is-6`
-   `is-7`
-   `is-8`
-   `is-9`
-   `is-10`
-   `is-11`
-   `is-12`

## 📱 Mobile columns
By default, columns are only activated from **tablet** onwards. This means columns are stacked on top of each other on **mobile**.  
If you want columns to work on **mobile too**, just add the `is-mobile` modifier on the `columns` container:

```html
<div class="columns is-mobile">
  <div class="column">1</div>
  <div class="column">2</div>
  <div class="column">3</div>
  <div class="column">4</div>
</div>
```
If you  _only_  want columns on  **desktop**  upwards, just use the  `is-desktop`  modifier on the  `columns`  container:
```html
<div class="columns is-desktop">
  <div class="column">1</div>
  <div class="column">2</div>
  <div class="column">3</div>
  <div class="column">4</div>
</div>
```

## Multiline
Whenever you want to start a new line, you can close a `columns` container and start a new one. But you can also add the `is-multiline` modifier and add more column elements than would fit in a single row.
```html
<div class="columns is-multiline is-mobile">
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-half">
    <code>is-half</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column is-one-quarter">
    <code>is-one-quarter</code>
  </div>
  <div class="column">
    Auto
  </div>
</div>
```
## PurgeCSS
I recommend to use [PurgeCSS](https://purgecss.com/) by using the Flexbox Grid.  The `.css` file `flexboxgrid.css` has a lot of  css classes. PurgeCSS is a tool to remove unused CSS. So you optimize your application by purging (deleting) the classes you don't use.

## You may also like...

* [React SPA Boilerplate](https://github.com/dennisfrijlink/react-spa-boilerplate) - A boilerplate for single page applications based on the React.js Library
* [Nuxt SPA Boilerplate](https://github.com/dennisfrijlink/nuxt-spa-boilerplate) - A boilerplate for single page applications based on the Vue.js Framework, Nuxt.js
* [Nuxt SSG Boilerplate](https://github.com/dennisfrijlink/nuxt-ssg-boilerplate) - A boilerplate for static site generation based on the Vue.js Framework, Nuxt.js

If you're looking for other reusable tools, check my repository [Development Utilities](https://github.com/dennisfrijlink/development-utilities). It's a collection of my favorite development utilities for (progressive) web and hybdrid apps.
