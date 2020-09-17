# Operators
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

[<-- Back](README.md)