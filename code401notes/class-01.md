#Class 01: Exception handling and Debugging

##Debugging for Absolute Beginners:
*link was broken*

##Try/Catch Blocks:
- if a code block might throw an exception, put it in a **try** block.
- **catch** blocks written below will are used the handle exceptions.
**EX:**[Code Example Link](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions)

- The CLR catches exceptions not handled by the catch blocks, causing a debug dialogue box to come up, or stopping the execution with a dialogue block with information about the exception.

##Statement Keywords:
statements are program instructions and are run in sequence
- **Selection statements:**if, else, switch, case
- **Iteration statements:**do, for, foreach, in, while
- **Jump statements:**break, continue, default, goto, return, yield
- **Exception handling statements:**throw, try-catch, try-finally, try-catch-finally
- **Checked and unchecked:**checked, unchecked
- **fixed statement**fixed
- **lock statement:**lock

##Therac-25:

A computer-controled radiation therapy machine that, due to programming errors, or race conditions, accidently overdosed many patients with excessive amounts of radiation. The problem? Amongst many, there wasn't enough debugging before it was assembled and used at the hospital. Always thoroughly debug your code and analyse all of its outcomes.

##Ariane_5:

I didn't understand the purpose of this article, but I had fun reading it! Spaceships are pretty cool. 