# Class 02 Reading Notes

## Chapter 2: Text
- Elements in HTML describe the structure of a page as well as provide semantic info **EX:** where you should place emphasis, the definitions of any acronyms you might use, when the text given is a quotation.

### Tags/ Elements:
- **h1-h6:** headings, they decrease in font size from 1 to 6.
- `<p></p>` constitutes a paragraph
- `<b></b>` bold
- `<i></i>` italic
- `<sup></sup>` superscript
- `<sub></sub>` subscript
- `<br />` line break, self closing*
- `<hr />` makes a horizontal line through a line break, self closing*
- `<strong></strong>` similar to bold, implies emphasis on a bti of text.
- `<em></em>` similar to italic, implies emphasis that subtly changes the meaning of a sentence.
- `<blockquote></blockquote>` used to indicate quotes that take up a whole paragraph.
- `<q></q>` indicates a shorter quote, within a paragraph.
- `<cite></cite>` used to cite source material
- `<dfn></dfn>` used to indicate the defining instance of a term
- `<address></address>` used to indicate the contact information of the author
- `<ins></ins>, <del></del>` indicated insertions or deletions to a document
- - `<s></s>` strikethrough

## Chapter 10: Introducing CSS

- CSS treats each HTML element as if it is a box
- uses rules made up of **selectors** amd **declarations** to dictate how elements of the page should look.
- **Declarations** are made up of  **properties** of the element you are changing and the **value** of those properties.
- you can do css externally by linking a css file `<link href="css/styles.css" type="text/css"` or inline by using a `<style></style>` tag.
- Example:`p {color: blue;}`
- CSS "cascades", meaning the rules are read top to bottom, i.e. things writen lower down on the code can effect things higher up

## Chapter 2: Basic JavaScript instructions

- **Statement:** Each individual step or instruction for the browser to follow. **EX:** `document.wrtie(greeting);`
- **Comment** in your code using `/*...*\` for **multi-line comments** and `//...` for **single-line comments**
-**Variable:** a way to store bits of data.
Declare values with **var** and assign them values with **=**. 
## Three Data Types:
- **Numeric**
- **String**
- **Boolean**
- You can change the value of variable later in the script.

## Arrays
- are like variables, but store lists of data instead.
- **EX:** `var colors; colors = ['white', 'black', 'custome'];` array literal
`var colors= new Array ('white', 'black', 'custome');` array constructor
- Each item in an array is automatically given a number or **index**. Index starts at 0. 
- **EX:** to access the 3rd item in this array: `var itemThree; item Three = colors[2];`
- **length:** the number of items in an array
- **EX:** `var numColors; numColors = colors.length;`
- you can change the value of an item in an array by selecting it and reasigning it.

## Expressions:
Expressions evaluate or result in a single value
- assign a value to a variable : `var color = 'beige';`
- use two or more values to return a single value `var are = 3 * 2;`

## Operators:
Expressions rely on operators. Operators allow programmers to create a single value from one or more values
- **Assignment**
- **Arithmatic**
- **String**
- **Comparison**
- **Logical**

# Chapter 4: Decisions and Loops
Two components to a decision:
1. An expression is evaluated, which returns a value.
2. A conditional statement says what to do in a given situation.

**Comparison operators** allow you to evaluate a situation by comparing one value in the script to what you expect it might be. The result will be **Boolean**, or true or false.
- `==` "is equal to" compares 2 values, prefered to use the strict method.
- `===` "strict equal to" compares two values to see if data type and value are the same.
- `!=` "is not equal to"
- `!==` "strict not equal to"
- `>` "greater than"
- `>=` "greater than or equal to"
- `<` "less than"
- `<=` "less than or equal to" 
**Logical Operators** While comparison operators usually return single values of true or false, logical operators allow you to compare more than one comparison operator. 
- `&&` "logical AND"
- `||` "logical OR"
- `!` "logical NOT"
Logical expressions are evaluated **left** to **right**
- if the first condition can provide enough info to get the answer, there is no need to read second evaluation. I.E. *false* `&&` **anything** will be false *true* `||` **anything** will be true.

# Loops
Loops check a condition, if it runs **true** a code block will run, then the condition is checked again and repeats until the condition returns **false**.
- **"for" loops:** used to run code a specific number of times, the condition is usually a counter that tells how many times to run the loop. /
**EX:** `for (var i = 0; i < 10; i++) { document.write(i); }`
- *var i = 0*: initialization, creates initial variable or index, this one is set to 0.
- *i < 10;*: condition, the loop should continue to run until the counter reaches the specified number, 10.
- *i++*: update, every time the loop has run the statements in the curly braces, it adds one to the counter.
- **"while" loops:** the condition can be somethign other than a counter, and the code will run the loop as long as the condition is true.
- **"do while" loops:** similar to "While" but will always run the statements inside the curly braces at least once, even if the condition is false.

[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)



