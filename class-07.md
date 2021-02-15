## article 

**Domain modeling** is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

![picture](https://camo.githubusercontent.com/55928963ae0dc919186799ab35c1cd669724ddbeb0658d0ca4b9e79b38e1804e/68747470733a2f2f692e696d6775722e636f6d2f47326250456c462e706e67)

* This is object-oriented programming in JavaScript at its most fundamental level.

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.


* Model its behaviors with small methods that focus on doing one job well.
* Create instances using the new keyword followed by a call to a constructor function.
* Store the newly created object in a variable so you can access its properties and methods from outside.
* Use the this variable within methods so you can access the object's properties and methods from inside.

## Html Book
*A table* represents information in a grid format,Examples of tables include financial reports, TV
schedules, and sports results.

* Basic Table Structure:

1. <table> :The <table> element is used to create a table. The contents
of the table are written out row by row.

2. <tr> :You indicate the start of each row using the opening <tr> tag.
(The tr stands for table row.)It is followed by one or more<td> elements (one for each cell
in that row). 

3. <td> :Each cell of a table is represented using a <td>
element. (The td stands for table data.)

*You can make cells of a table span more than one row or column using the rowspan and colspan attributes.*

* three elements that help distinguish between the
main content of the table and the first and last rows :

1. <thead>: The headings of the table should sit inside the <thead> element. 
2. <tbody>:The body should sit inside the <tbody> element
3. <tfoot>: The footer belongs inside the <tfoot> element.


## Javascript Book:
 Programmers use functions, methods, and objects to organize their code. 

 ##### **Functions** 
 let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements.

 - When you ask it to you expect it to provide you Instead, they are executed as perform its task, it is known as with an answer, the response is soon as the interpreter comes calling the function.
 - Pieces of information passed  to a function are known as parameters. 
 - When you write a function and you expect it to provide you  with an answer, the response is s known as a return value


* A **function declaration** creates a function that you can call later in your code.

* **function expression**If you put a function where the interpreter would
expect to see an expression, then it is treated as an expression

*LOCAL VARIABLES*
When a variable is created inside a function using the var keyword, it can only be used in that function.
It is called a local variable or function-level variable.

*GLOBAL VARIABLES*
If you create a variable outside of a function, then it can be used anywhere within the script. It is called a
global variable and has global scope

##### Objects :

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,
variables and functions take on new names. 

- f a variable is part of an object, it is called a *property*. 
- If a function is part of an object, it is called a *method*

* The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates. 

Arrays and objects can be used to create complex data
sets (and both can contain the other).