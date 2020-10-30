# Class 01 Reading Notes: SMACCSS and Responsive Web Design

## Shay Howe's Intro to RWD:

RWD: Responsive Web Design: building a website suitable to work on every screen size.
- **Responsive:** to react fluidly and wuickly to any change.
- **Adaptive:** built to a group of pre-set factors
- **Mobile:** To build a seperate webiste, typically iwth a new Domain, soley for the mobil users. Downside: new code base, browser sniffing

### Flexible Layouts:
Building the layout of a website with a **flexibile grid**, capable of dynamically resizing to any width.
- uses **relative** length units (% or em) when declaring width, margin, or wadding.

### Relative Viewport Lengths:
- use `vw`, `vh`, `vmin`, `vmax` properties

### Media Queries:
Can target certain individual browser and device circumstances for styling
- use `@media` rule inside of an existing stylesheet
- Media Query Syntax: `@media mediatype oneormoreexpressions`
- **Media Types:** all, screen, print, tv, braille
- Expressions allocate to true or false, when feature + value = true, the style is applied.
**Logical Operators:** and, not, only
- **EX:** `@media all and (min-width: 800px) and (max-width: 1024px){...}` selects all media types between 800 and 1024 px.
- **Not** negates the query: `@media not screen and (color){...}` applies to any device w/o a colored screen.
- **Only** is newer and not supported by HTML4
- when using not or only, you can leave off the media type, it defaults to all

### Media Features:
**Height and Width:**
- min/max width: min = values greater than or equal to, max = values less than or equal to.
- based on the height and width of the view port rendering area, for example the browser window.
**Orientation:**
- determines if a device is in landscape or portrait mode.
### Aspect Ratio Media Features:
`aspect-ratio` and `device-apect-ratio` features specify the h/w pixel ratio of target render area.
- Value consists of 2 positive integers seperated by a forward slash: w/h
- **EX** `@media all and (min-device-aspect-ratio: 16/9){...}`
- `device-pizel-ratio` feature is good to use to identify HD devices, like retina displays
- `resolution` specifies the resolution of the output device.

### Mobile First Design:
Using styles targeted at smaller viewports as the default.
- design with the constraints of a mobile user in mind
- loading styles for the desktop to have them be overwritten is a waste of bandwidth.
- avoid using CSS3 shadows, gradients, transformations and animations- they drain battery and cause heavy loading
- Use `@viewport` rule in CSS to set height and width values to the device height and width

### Viewport Scale:
- minimum, maximum and intitial scale determines how a website is scaled or zoomed on a mobile device
- you can combine viewport values, seperated with a comma
### FLexible Media: 
videos, images and other types of media must be scalable as well.
-`img,video,canvas {max-width:100%;}` is a quick way to ensure any media will scale down as the viewport gets smaller according to its container's width.

## Floats:
- Page elements with the **float** property remain **in the flow** of the webpage, unlike absolutely positioned items.
- left, right, none (default) inherit values.
- **inherit:** assumes the float value of parent element
- **clear** will move element down passed the float
- if the parent element contains all floated items, it may collapse.
**Tips to clear floats when you don't always know the succeeding element:**
- Empty Div Method
- OverFlow Method
**Bugs in IE and how to get around them:**
- **Push Down** happens when an element inside the float is wider that the float itself, fix by using `overflow: hidden` to cut off the excess.
- **Double Margin Bug:** if you apply a margin in the same direction as a float, it will double the margin. To fix use `display: inline`
- **3px Jog** when the text next to a floated item is kicked away by 3px, fix by setting a w or h on affected text
- **Bottom Margin Bug** when a floated parent element has floated children, the bottom margin on children is ignored. Fix by using a bottom padding on the parent instead.

[<-- Back](301readingnotes.md) [Back to Home](README.md)