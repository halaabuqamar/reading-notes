
# html book

### chapter 3:
three different types of lists in html:
1. ordered list (ol)
2. unordered list (ul)
3. defintion list (dl)

You can put a second list inside
an (li) element to create a **sublist** or **nested list**.


*Ordered lists* use numbers.
*Unordered lists* use bullets.
*Definition lists* are used to define terminology
 
 
 ### chapter 13:

*CSS treats each HTML element as if it has its own box.*
 
 **Box dimensions** width and height 
 - The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems

**limitng width**  
, the
**min-width** property specifies the smallest size a box can be displayed at when the browser
window is narrow, and the **max-width** property indicates the maximum width a box can
stretch to when the browser window is wide

**limiting hight**
*mini height*
*max height*

**over flowing content**
The overflow property tells the
browser what to do if the content
contained within a box is larger
than the box itself
- hidden
- scroll

Every box has three available properties that
can be adjusted to control its appearance:
1. boarder
2. margin
3. padding

*Border color* 
It is possible to individually
control the colors of the borders
on different sides of a box using:
border-top-color
border-right-color
border-bottom-color
border-left-color

The **visibility property** allows you to hide boxes from users
but It leaves a space where the element would have been.
This property can take two
values:
1. hidden
This hides the element.
2. visible
This shows the element. If the visibility of an element
is set to hidden, a blank space will appear in its place.
If you do not want a blank space to appear, then you should use
the display property with a value of none instead

CSS3 has introduced the ability to create image
borders and rounded borders



# javascript book

### chapter 2:

**ARRAYS**
An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 
we use it when :list or a set of values that
are related to each other

This technique for creating
an array is known as an *array literal*. It is usually the preferred method for creating an array.
You can also write each value ona separate line:
colors= ['white',
'black',
'custom'];

On the left, you can see an array created using a different
technique called an array constructor. This uses the new
keyword followed by Array();
The values are then specified in parentheses (not square brackets), and each value is
separated by a comma. You can also use a method called i tern()
to retrieve data from the array. (The index number of the item is
specified in the parentheses.) 

**VALUES IN ARRAYS**
1. NUMBERING ITEMS IN AN ARRAY Each item in an array is
automatically given a number called an index
2. ACCESSING ITEMS IN AN ARRAY To retrieve the third item on the
list, the array name is specified along with the index number in
square brackets. 
3. NUMBER OF ITEMS IN AN ARRAY Each array has a property called
length, which holds the number of items in the array. 


### chapter 4 :

Scripts often need to behave differently depending upon how the user interacts with the web 

1. EVALUATIONS 
2. DECISIONS
3. LOOPS 

there are two components to a decision:
- an expression is evaluated, which returns a value
- a conditional statment says what to do in a given situation 

**opeartors:**
- logical eg)  & || 
- arythmatic eg) + = % 
- comparission eg) <= >=  == the answer should be T or F

**USING IF STATEMENTS:** Conditional statements allow your code to make
decisions about what to do next.
- if
- if else *allow you to run one set of code if a condition is true, and another if it is false.* 



 **switch** statement is to present the user with a different message depending on which level they are at. The message is stored in a variable called msg.*allow you to compare a value against possible outcomes (and also provides a default option if none match).*

*If you use a data type JavaScript did not expect, it tries to make sense of the operation ratherthan report an error* 

Logical operators are processed left to right. They short-circuit (stop) as soon as they have a
result - but they return the value that stopped the processing (not necessarily true or fa1se). 

loops:
- for loop
- while loop 
- do while loop


