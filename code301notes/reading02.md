# Class 02 Reading Notes: JQuery, Events, and the DOM

## JQuery
A JavaScript file you can include in your page.
- Link JQuery to your html page using the `script` tag, as you would link your own app.js
- Uses **CSS-style selectors** to target nodes on the DOM tree.
**Ex:**pg. 302
- Has **built-in methods** to work with elements in that selection.
**Ex:** 
- the `ready()` method, used to check if the DOM has been constructed before running the script.
- `attr()` , `removeAttr()` add and remove attributes to html elements
- `append()` , and `prepend` add html elements after and before another element, respectively
- **pg. 304**
### Syntax:
- **"$"** accesses JQuery
- $("selector").action();
### Looping
When a selector returns multiple elements, you can update all of them using one method, instead of having to use a loop.
### Chaining
You can use more than one method at a time:
- **Ex:** `$('li[id!="one"').hide().delay(500).fadeIn(1400);`
- *animations take in times in Milliseconds as a parameter*
### Each:
Jquery allows you to recreate the functionality of a loop on a selection of elements, using  the `each()` method.
- use `this` to access the current element as the method goes through the elements in a selection.
### Event Methods:
- `on()` method is used like addEventListener.
**Ex:** `$('selector').on(event, function() {...});`
### CDN:
Content Delivery Network: a series of servers that are designed to serve static files very quickly.
- you can include JQuery in your page using a CDN
- **Ex:** pg 355
It is best to put you scripts right before your **closing body tag**

## Pair Programming is:
- Efficient, studies have shown it might take slightly longer, but produces bettr results. having 2 eyes on the code base makes it easier to catch mistakes and bugs.
- Engaging, pair programming promotes focus.
- An oppertunity to learn from others.
- An opportunity to hone social skills.
- Promotes job interview readiness, shows your ability to work on a team.
- Promotes work environment readiness, pair programming is very common place in the industry.

[<-- Back](301readingnotes.md) [Back to Home](README.md)