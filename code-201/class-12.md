# Charts.js

* Chart.js: a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page.
* It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more.

#### Setting up

* The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script.
* Drawing a line chart: To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.
  
  ```html
  <canvas id="buyers" width="600" height="400"></canvas>
  ```

# Basic usage of canvas

* a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes.
* Indeed, the `<canvas>` element has only two attributes, width and height.
* When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
* The `<canvas>` element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas.
* Fallback content The `<canvas>` element differs from an `<img>` tag in that, like for `<video>`, `<audio>`, or `<picture>` elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it.

# Drawing shapes with canvas

* The grid:it is canvas grid or coordinate space.
* All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y).

# Applying styles and colors

* If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
* Transparency:  we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

# Drawing text

* The canvas rendering context provides two methods to render text:
fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

* 
