# FUNCTIONS & OBJECTS BUILT-IN METHODS 
## WHAT IS A FUNCTION?
**Functions** let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 


Grouping together the The steps that the function On the right, there is an example
statements that are required to needs to perform in order to of a function in the JavaScript
answer a question or perform a perform its task are packaged file. It is called updateMessage () .
task helps organize your code. up in a code block. *You may
remember from the last chapter Don't worry if you do not
Furthermore, the statements in a that a code block consists of one understand the syntax of the
function are not always executed or more statements contained example on the right; you will
when a page loads, so functions within curly braces. (And you do take a closer look at how to write
also offer a way to store the steps not write a semicolon after the and use functions in the pages
needed to achieve a task*
 The closing curly brace - like you do that follow.
script can then ask the function after a statement.)
to perform all of those steps as Remember that programming
and when they are required. Some functions need to be languages often rely upon on
For example, you might have provided with information in name/value pairs. The function
a task that you only want to order to achieve a given task. For has a name, updateMessage,
perform if the user clicks on a example, a function to calculate and the value is the code block
specific element in the page. the area of a box would need (which consists of statements).
to know its width and height. When you call the function by its
If you are going to ask the Pieces of information passed name, those statements will run.
function to perform its task to a function are known as
later, you need to give your parameters. You can also have anonymous
function a name. That name functions. They do not have a
should describe the task it is When you write a function and name, so they cannot be called.
performing. When you ask it to you expect it to provide you Instead, they are executed as
perform its task, it is known as with an answer, the response is soon as the interpreter comes
calling the function. known as a return value. across the





## ANONYMOUS FUNCTIONS
& FUNCTION EXPRESSIONS
*Expressions* produce a value. They can be used where values are expected.
If a function is placed where a browser expects to see an expression,
(e.g., as an argument to a function), then it gets treated as an expression. 


