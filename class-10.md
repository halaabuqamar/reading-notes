## javascript book
#### Chapter 10:

* EXECUTION CONTEXT:
Every statement in a script lives in one of three execution contexts:
1.  GLOBAL CONTEXT
Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT
Code that is being run within a function. Each function has its own function context.
3. EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function called eva l {) .

* VARIABLE SCOPE:
The first two execution contexts correspond with the notion of scope:
1.  GLOBAL SCOPEIf a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.

2. FUNCTION-LEVEL SCOPE:When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

* Each time a script enters a new execution context, there are two phases of activity: 
1.  PREPARE:
- The new scope is created
- Variables, functions, and arguments are created
- The value of the this keyword is determined
2. EXECUTE 
- Now it can assign values to variables
- Reference functions and run their code
- Execute statements 

*In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.*

If a JavaScript statement generates an error, then it throws an **exception**. At that point, the interpreter stops and looks for exception-handl ing code. 

*The console helps narrow down the area in which the error is located, so you can try to find the exact error*

* Error objects can help you find where your mistakes are and browsers have tools to help you read them. 
- here are seven types of built-in error objects in JavaScript.

1. Error:Generic error - the other errors are all based upon this error
2. Syntax Error:Syntax has not been followed
3. Ref erenceError: Tried to reference a variable that is not declared/within scope
4. TypeError:An unexpected data type that cannot be coerced
5. Range Error:Numbers not in acceptable range
6. URI Error:encodeURI ().decodeURI(),and similar methods used incorrectly
7. EvalError :eva l () function used incorrectly

* HOW TO DEAL WITH ERRORS:
-  DEBUG THE SCRIPT TO FIX ERRORS :), you will need to debug the code, track down the source of the error, and fix it.
-  HANDLE ERRORS GRACEFULLY :You can handle errors gracefully using try, catch, throw, and f i na 1 ly statements.

*Debugging is about deduction: eliminating potential causes of an error.* 

* WHERE IS THE PROBLEM?
First, should try to can narrow down the area where the problem seems to be. In a long script, this is especially important.
1. Look at the error message, it tells you:
- The relevant script that caused the problem.
- The line number where it became a problem for the interpreter. (As you will see, the cause of the error may be earlier in a script; but this is the point at which the script could not continue.)
- The type of error (although the underlying cause
of the error may be different).
2. Check how far the script is running.
Use tools to write messages to the console to tell how far your script has executed.
3. Use breakpoints where things are going wrong.
They let you pause execution and inspect the values that are stored in variables

- WHAT EXACTLY IS THE PROBLEM?
Once you think that you might know the rough area
in which your problem is located, you can then try to
find the actual line of code that is causing the error.
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script.
2. Break down I break out parts of the code to test smaller pieces of the functionality.
- Write values of variables into the console.
- Calrfunctions from the console to check if they are returning what you would expect them to.
- Check if objects exist and have the methods I properties that you think they do.
3. Check the number of parameters for a function, or the number of items in an array. 

- You can pause the execution of a script on any line using **breakpoints.**
- You can indicate that a breakpoint should be triggered only *if a condition that you specify is met.* The condition can use existing variables. 

* You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.

* You can also place the debugger keyword within a conditional statement so that it only triggers the breakpoint if the condition is met. 

**If you know your code might fail, use try, catch, and finally.Each one is given its own code block.**
*If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them* 

Being able to throw an error at the time you know there might be a problem can be better than letting that data cause errors further into the script.
If you are working with data from a third party, you may come across problems such as:
1. JSON that contains a formatting error
2. Numeric data that occasionally has a nonnumeric value
3. An error from a remote server
4. A set of information with one missing value

