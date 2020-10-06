# Class 07 Reading Notes

## Domain Modeling
**Domain Modeling:** a process of creating a conceptual model in code for a specific problem. 
- **A model:** describes the various entities, their attributes and behaviors, and constraints that govern the problem domain.
- **object-oriented model:** stored data in properties and stores behaviors in methods
To define the same properties between many objects, use a **constructor function**
`var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);`

- storing data within properties ensures any newly created object can access the data later
- After the constructor function definition, two objects are **instantiated** with the new keyword and their properties are **initialized** by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables.
- The new keyword instantiates (i.e. creates) an object.
- The constructor function initializes properties inside that object using the this variable.
- The object is stored in a variable for later use.
- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.

## Chapter 6: Tables
- `<table>` element adds tables to page
- `<tr>` elements contain each row of the table
- `<td>` element represents cells inside each row or `<th>` if it is a header.
- you can make calls of a table span more than one row or collumn using **rowspan** and **colspan** attributes.
- for long tables, split it into a `<thead>`, `<tbody>`, `<tfoot>`

## Chapter 3: Functions, Methods, and Objects:
Sometimes you want several objects that represent similar things:
- **object constructors** use a function as a template for creating objects.
- **EX:** page 108
- you create new **instances** of the object using the constructor function using the keywords **new** followed by a call to the function with the properties of each object given as arguements to the function/
- `function Hotel (name,rooms,booked)`
- `var quayHotel = new Hotel('Quay', 40, 25);`
### Built-in Objects
#### Browser Object Model
- The **window object** represents the current browser window or tab. it is the topmost object in the BOM
- find examples of properties and methods of the window object **page 124**
#### Document Object Model
- the **document object** is the topmost object in the DOM and represents the web page loaded into the current browser or tab.
- find examples of properties and methods of the document object **page 125**
#### Global objects: string object
- whenever you have a value that is a string, you can use the properties and methods of the STring object on that value.
- find example of properties and methods of the String object **page 128**
- each character in a string is given an **index number** which starts at 0 like an array.
#### Global objects: number object
- used whenever you have a value that is a number
- examples "" **page 132**
- **integer:** a whole number
- **real number:** a number that can contain a fractional part
- **floating point number:** a real number that uses decimals to represent a fraction.
- **scientific notation:** a way of writing numbers that are too big or too small.
#### Global objects: math object
- the Math object has properties and methods for mathmatical constants and functions
- Examples: **page 134** 
#### Global objects: Date (and time) Objects
- Examples: **page 137**

[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)