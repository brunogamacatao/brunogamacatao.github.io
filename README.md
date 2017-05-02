## Website Performance Optimization portfolio project

### Getting started
Having installed the gulp in the machine, run:
`$> compass watch`

### Optimizations
#### Time to resize pizzas
- Removing much of the `resizePizzas()` function. Now the function is restricted to just changing the class for resize's with `display: flex` property of the CSS.

#### `onscroll` with 60fps on pizza.html
- Decrease from 200 to 50 background pizzas. Most of the pizzas didn't appear in the viewport.
- Change the motion property `left` to` transform: translateX` to take advantage of GPU usage.
- Remove the `var items = document.querySelectorAll('.move');` from inside the function `updatePositions()` because there's no need to select all the pizzas at each move.

#### Others
- Importing thumbnails images for optimization.
- Resized thumbnail of the pizza. A 2000px image was used for a space of 100px.
- Images optimization.
- Scripts JS with `async`.
- Gulp for build css compacted and minified.
