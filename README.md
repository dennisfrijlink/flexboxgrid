
# flexboxgrid
A simple 12 columns, responsive CSS grid based on flexbox and Bulma CSS

Bulma: https://bulma.io/

## Setup
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

## Usage
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

## Mobile columns
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
## Examples
Check [Bulma Columns](https://bulma.io/documentation/columns/) for some examples