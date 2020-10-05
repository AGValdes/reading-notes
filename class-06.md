# Class 06 Reading Notes

## Chapter 3: Object Literals 
Objects group together variables and functions to create a model of something in the real world I.E. the hotel example
- If a **variable** is part of an object it is called a **property**
- **functions** inside of objects are called **methods** and represent tasks associated with the object.
- `var hotel = {`
- ` name: 'Quay',`
- `booked: 25,`
- `gym: true,`
- ` roomTypes: ['twin','double', 'suite'],`
- `checkAvailability; function() {`
- `return this.rooms - this.booked; }`
**keys** are used to access their corresponding value.
**property keys:**  name, rooms, booked, gym roomTypes
**property values:** string, number, number, Boolean, array

## Chapter 5: Document Object Model
Browsers represent a page using a **DOM tree** Dom trees have 4 types of nodes:
- **document nodes**
- **element nodes** can be selected by their id or class attributes, by tag name, or by using CSS selector syntax. 
- **ex:** `getElementById()` `querySelector` `getElementsByClassName()` `getElementsByTagName()` `querySelectorAll()` 
- **move between element nodes** `parentNode` `previousSibling/nextSibling` `firstChild/lastChild`
- **attribute nodes**
- **text nodes**
Whenever a DOM query can return more than one node, it will always return a **NodeList**
- From an element node you can access and update it content **EX:** `textContent` and `innerHTML` or using DOM manipulation techniques.
- An element node con contain multiple text nodes and **child elements** that are **siblings** to each other.
**JQuery** is often used because using DOM in older browsers in inconsistent I.E. the problem with white space being read as extra text nodes.

[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)