# Class 12 Reading Notes:

## Chart.js API
Charts are a more visually appealing way to display data than tables.
- **Chart.js** js plugin that uses HTML5's **canvas** element to draw the graph onto the page.
- you can make **line charts** **Pie Charts** or **bar charts**


## The Canvas Element
- `<canvas>` element has 2 attributes: **width and height** if these arent specified it will default to 300px wide and 150px high.
### Drawing Shapes with Canvas
- only supports 2 shapes: **rectangle and paths**
- **paths** are lists of points connected by lines (other shapes can be made by combining one or more paths)
#### Rectangle: 
- `fillRect(x, y, width, height)` draws a filled rectangle.
- `strokeRect(x, y, width, height)` draws a rectangle outline.
- `clearRect(x,y,width,height)` clears the specified rectangular area, making it transparent.

#### Paths:
EX: function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }

  - To **draw arcs or circles**, we use the `arc()` or `arcTo()` methods.
  - `arc(x, y, radius, startAngle, endAngle, anticlockwise)`
  - `arcTo(x1, y1, x2, y2, radius)`
  - **Bézier curves**, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.
  - `quadraticCurveTo(cp1x, cp1y, x, y)`
  - `bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)`
  - there's no limitation to the number or types of paths you can use to create a shape.

### Adding Color and Styling: 
You can add color and styling to your shapes with JS as well 
- `fillStyle = color`
- `strokeStyle = color`
- play with transparency with `globalAlpha = transparencyValue`
- There are several properties which allow us to **style lines**.
- `lineWidth = value`
- `lineJoin = type`
- `miterLimit = value`
- `getLineDash()`
- `setLineDash(segments)`
- `lineDashOffset = value`
- you can add gradients by creating a CanvasGradient object.
- you can also add patterns of images with the **createPattern() method**.
### Styling Text:
- `fillText(text, x, y [, maxWidth])`
- `strokeText(text, x, y [, maxWidth])`
- `font = value`
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
- `textAlign = value`
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
- `textBaseline = value`
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
- `direction = value`
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
- `measureText()`
Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.