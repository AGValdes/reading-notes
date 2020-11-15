# Class 11 Reading Notes: EJS

- EJS is a **node package** that you can install with npm-- similarly to express, cors, etc.
- you can make a **.ejs file**, like an index, and insert variables into them to evaluate variables and display them on the page.
- use `<%= %>` wrapped around your variable to evaulate it.
- otherwise wrap you loops and if statements etc. with `<% %>`
- you can **iterate over an array** of values with a for loop right in the index page this way to display multiple things, such as an array of objects.
- you can also incorporate **if else** statements right into your index
- **layouts** are not native to express, you have tp do npm i express-ejs-layouts to install them. just like **templating**
- **partials** are native to to ejs
- a use case for partials would be like nav bars, or footers, essentially a reusable piece of text.