# Reading O3 Notes: Mustache and FlexBox

## Mustache 
- **Templating:**  fast and efficient technique to render client-side view templates with Javascript by using a **JSON data source**

- **Mustache** is a templating syntax
-  can be used for HTML, config files, source code.
- works by **expanding tags** in a template using **values** provided in a **hash** or **object**
- often referred to as **logic-less** because there are no if statements, else clauses, or for loops. Instead, there are only **tags**.
- **EX:** `Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” }); // returns: Hello, Sherlynn`

![Mustache Chart](https://miro.medium.com/max/1050/1*LbqYj87xlazySm6wE0Q2lA.png)

## FlexBox
[FlexBox Guide](https://css-tricks.com/product/css-flexbox-poster/)
- set `display:` to flex
### Examples of parent properties:
- **flex-direction:**
- row (default): left to right in ltr; right to left in rtl
- row-reverse: right to left in ltr; left to right in rtl
- column: same as row but top to bottom
- column-reverse: same as row-reverse but bottom to top

- **justify-content:**
- flex-start (default): items are packed toward the start of the flex-direction.
- flex-end: items are packed toward the end of the flex-direction.
- start: items are packed toward the start of the writing-mode direction.
- end: items are packed toward the end of the writing-mode direction.
- left: items are packed toward left edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
- right: items are packed toward right edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
- center: items are centered along the line
- space-between: items are evenly distributed in the line; first item is on the start line, last item on the end line
- space-around: items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.
- space-evenly: items are distributed so that the spacing between any two items (and the space to the edges) is equal.

### Examples of Child Properties:
- **align-self:** This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

[<-- Back](301readingnotes.md) [Back to Home](README.md)