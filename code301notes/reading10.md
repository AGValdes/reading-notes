# Class 10 Reading Notes: The Call Stack and Debugging

## Call Stack
- a mechanism for an **interpreter** (i.e. the JS interpreter in a web browser) to keep track of its place in the script that calls multiple functions, what function is **currently being run**, and what functions are **called within that function**, etc.
- uses the **Last In**, **First Out** (LIFO) principle 
- When a script calls a function, the interpreter **adds it to the call stack** and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack **further up**, and run where their calls are reached.
- When the current function is finished, the interpreter **takes it off the stack** and resumes execution **where it left** off in the last code listing.
- If the stack **takes up more space** than it had assigned to it, it results in a **"stack overflow"** error.
- **Stack Overflow:**A stack overflow occurs when there is a **recursive function** (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.
- **Manage Function Invocation:**Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is **synchronous**.
- **Temporarily store**: When a function is called, the **function**, its **parameters**, and **variables** are pushed into the call stack to form a **stack frame**. This stack frame is a **memory location** in the stack. The memory is cleared when the function returns as it is popped out of the stack.

## Javascript Error Messages:
- **Reference Errors:** when use a variable that is not yet declared, common thing when using const and let.
- **Syntax Errors:**  occurs when you have something that cannot be parsed in terms of syntax
- **Range Errors:** manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
- **Type Errors:** show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

### Debugging:
- simplest way is to console.log things
- debugger statement
- try…catch
- **Tools to avoid runtime errors:** JS is not a **compiled language** like Java so your errors will happen at runtime, that means that you can only see whatever is wrong with your code **after you run it**
- **quokka** evalutes code as you type
- **eslint** can pick up on some errors before you run your code.

[<-- Back](301readingnotes.md) [Back to Home](README.md)