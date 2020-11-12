# Class 09 Reading Notes: Refactoring

## Functional Programming Concepts

- **Functional Programming:** a programming paradigm, or a style of building the structure and elements of computer programs, that treats computation as the evaluation of mathematical functions and **avoids changing-state and mutable data**

**Pure Functions:** 
- return the same result if given the same arguments (it is also referred as deterministic)
 - do not cause any observable side effects

 - **Impure Example:**
 - `let PI = 3.14;` 
 - `const calculateArea = (radius) => radius * radius * PI;`
 - `calculateArea(10); // returns 314.0`
-  it uses a global object that was not passed as a parameter to the function, if the value of PI is changed it will change results.

- **Pure Example:**
- `let PI = 3.14;`
- `const calculateArea = (radius, pi) => radius * radius * pi;`
- `calculateArea(10, PI); // returns 314.0`
- now we are just accessing parameters passed to the function.

- If our function  **reads external files**, it’s not a pure function — the file’s **contents can change**.
- Any function that relies on a **random number generator** cannot be pure

### Benefits to Pure Functions
- The code is easier to test

### Imutibility 
- When data is **immutable**, its state cannot change after it’s created. 
- If you want to change an immutable object, you can’t. Instead, you **create a new object** with the new value.

### Functions as First Class Entities:
- The idea of functions as first-class entities is that functions are **treated as values** and **used as data** and can:
- refer to it from constants and variables
- pass it as a parameter to other functions
- return it as result from other functions

### Higher Order Functions:
- takes one or more functions as arguments, or
- returns a function as its result

### Filter:
- The filter function expects a **true** or **false** value to determine if the element should or should not be included in the result collection

### Map:
- The `map()` method **transforms** an array by applying a function to all of its elements and **building a new array** from the returned values.

### Reduce:
- The idea of reduce is to receive a **function** and an **array**, and return a value created by combining the items.

## Refactoring

- Functions should be broken up so they only do 1 thing.
- this improves readability when multiple people are working on one code base.
- it is also important to get code right the first time, because in many businesses there isn't much value in refactoring.


[<-- Back](301readingnotes.md) [Back to Home](README.md)
