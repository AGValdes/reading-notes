# Class 03 Reading Notes

## Chapter 3: Lists
- **Ordered List:** numbered list `<ol></ol>`
- **Unordered List:** not numbered, displays bullet points by default `<ul></ul>`
both ordered and unordered lists will contain list items using tag `<li></li>`
- **Definition List:** set of terms and their definitions
- create list with `<dl></dl>`
- contain the term in `<dt></dt>`
- contain the definition in `<dd></dd>`
- you can create nested lists, or sublists, inside an `<li>` element

## Chapter 13: Boxes
You can manipulate how the browser displays boxes using CSS
### Properties:
- **height, width:** controls dimensions of boxes
- **min/max-width, min/max-height:** used to limit dimensions for responsive design
- **overflow:** tells the browser what to do with content that doesn't fit in the box, can use **hidden** to hide it or **scroll** to be able to scroll through it
- **border:** the very outter edge of the box, you can change border *width* *style* and *color*
- **border-image:** takes an image and divides into nine pieces, requires: the url of the image, where to slice the image, what to do with straight edges, either **stretch**, **repeat**, **round**
- **border-radius:** creates rounded corners on boxes.
- **margin:** space around the *outside* of the border. you can specify top, right, bottom, and left margins. 
- **padding:** space *inside* the border *outside* of the content **padding is added to the width of the box**  you can specify top, right, bottom, and left padding.
- **box-shadow:** creates a drop shadow around a box.
- to **center** boxes you can set right and left margins to **auto**
- IE6 includes padding and margins in width of the box, you can avoid this by ensuring to include a DOCTYPE declaration.
- **display:** use **inline** to make a block-level element inline, use **block** for the opposite, use **inline-block** to maintain the block-level element while causing them to flow like an inline element *EX: a nav bar*, use **none** to hide the element as if it is *not on the page at all.* 
- **visibility:** **hidden** hides the element, a blank space will appear

## Chapter 2 Review:
### Arrays
- are like variables, but store lists of data instead.
- **EX:** `var colors; colors = ['white', 'black', 'custome'];` array literal
`var colors= new Array ('white', 'black', 'custome');` array constructor
- Each item in an array is automatically given a number or **index**. Index starts at 0. 
- **EX:** to access the 3rd item in this array: `var itemThree; item Three = colors[2];`
- **length:** the number of items in an array
- **EX:** `var numColors; numColors = colors.length;`
- you can change the value of an item in an array by selecting it and reasigning it.

## Chapter 4: Decisions and Loops, cont.
**Switch Statement:** starts with a variable called the **switch value** each case indicates a possible value for this variable and the code that should run if the variable matches said value.
- the entire statement is in one code block, at the end of each case is the **break;** keyword
#### if/else vs. switch
- **if/else:** there is no need to have an **else** option, with a series of if statements, *all are checked* even if a match has been found **performes more slowly than switch**
- **switch:** you have a **default** option that is run if none of the cases match, if a match is found, the code is run; then the **break** statement stops the rest from running **performs faster**
#### Type Coercion:
- data types can be coverted to different data types
- **weak typing:** when a data type for a value can change, like in JS
- **strong typing:** requires specification on what data type each variable will be.
- type coercion can lead to unexpected values in your code, thats where the `=` `==` and `===` come in
#### Truthy and Falsy Values
- **falsy:** values are treated as if they are false
- **EX:** `var highScore = false;` boolean false `var highScore = 0;` the number 0 `var highScore = '';` empty string `var highScore = 10/'score';` NaN or Not a Number `var highScore;` a variable with no value.
- **truthy:** values are treated as if they are true
#### Checking Equality and Existence
- objects and arrays are often used to check for the existence of an element within a page
- because of type coercion, the strictly equals operators result in fewer unexpectded values. 
#### Short Circuit Values
Logical operators are processed from left to right, they **short circuit** or stop as soon as they have found a result, but return the *value* that stopped the processing, not necessarily *true* or *false*
- put code most likely to be **true** first in **OR** operations and **false** first in **AND** operations.
- place options that require the most processing power last, in case another value returns true and they do not need to be run.
#### Loops
Loops check a condition, if it runs **true** a code block will run, then the condition is checked again and repeats until the condition returns **false**.
- **"for" loops:** used to run code a specific number of times, the condition is usually a counter that tells how many times to run the loop. /
**EX:** `for (var i = 0; i < 10; i++) { document.write(i); }`
- *var i = 0*: initialization, creates initial variable or index, this one is set to 0.
- *i < 10;*: condition, the loop should continue to run until the counter reaches the specified number, 10.
- *i++*: update, every time the loop has run the statements in the curly braces, it adds one to the counter.
- **"while" loops:** the condition can be somethign other than a counter, and the code will run the loop as long as the condition is true.
- **"do while" loops:** similar to "While" but will always run the statements inside the curly braces at least once, even if the condition is false.

[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)