# class 04
### html book


#### chapter 4:
**Links** are the defining feature of the web because they allow you to move from
one web page to another.

*Writing  Links are created using the <a> element.*

linking to **other sites**:
Links are created using the <a> element which has an attribute
called href. The value of the href attribute is the page that
you want people to go to when they click on the link

Linking to Other **Pages on the Same Site** :
When you are linking to other pages within the same site,
you do not need to specify the domain name in the URL. You
can use a shorthand known as a relative UR

Directory Structure:
- The top-level folder is known as the root folder

**email links**
To create a link that starts up the user's email program and addresses an email to a specified
email address, you use the <a> element. However, this time the value of the href attribute starts
with mailto: and is followed by the email address you want the email to be sent to

*You can use the id attribute to target elements within a page that can be linked to.*

#### chapter 15:

*CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.* 

1. Block-level elements start on a new line Examples include:
<h1> <p> <ul> <li>

2. Inline elements flow in between surrounding text
Examples include:
<img> <b> <i>

**Position of Elements**
- normal flow : position:static
- relative positioning : position:relative
- absolute positioning : position:absolute

**box offset properties**
- fixed positioning
- floating positionig 

*If you want to control which element sits on top, you can use the z-index property*

Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens 



* <div> elements are often used as containing elements
to group together sections of a page.

* Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.

* The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)

* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).

* Grids help create professional and flexible designs.

* CSS Frameworks provide rules for common tasks.

* You can include multiple CSS files in one page.

# javascrit book:

#### Chappter 13:

*complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code*

1. functions and methods:Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).
 - function declaration: creat a name and then write the statment needed to achive 
 - call function: one word used to execute all of the statments.


Often functions are used to ensure that the variable names do not conflict
with each other (especially if the page uses more than one script

IMMEDIATELY INVOKED FUNCTION EXPRESSIONS (llFE) Pronounced "iffy," these functions are not given
a name. Instead, they are executed once as the
interpreter comes across them.

The location where you declare a variable will affect where it can be used
within your code. If you declare it within a function, it can only be used
within that function. This is known as the **variable's scope**.

**LOCAL VARIABLES**
When a variable is created inside a function using the
var keyword, it can only be used in that function.
It is called a local variable or function-level variable

**GLOBAL VARIABLES**
If you create a variable outside of a function, then it
can be used anywhere within the script. It is called a
global variable and has global scope. In the example
shown, wa 11 Size is a global variable.

*Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.*