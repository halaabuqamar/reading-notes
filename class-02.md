# Html
## Chapter 2 :

* **Structural markup**: the elements that you can use to
describe both headings and paragraphs.

* **Semantic markup**: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on

*HTML* elements are used to describe the structure of
the page* (e.g. headings, subheadings, paragraphs).

1. structural markup
HTML has six "levels" of
headings:
<h1> is used for main headings
<h2> is used for subheadings

<p>
To create a paragraph, surround
the words that make up the
paragraph with an opening <p>
tag and closing </p> tag.

2. semantic markup

eg) Strong & Emphasis

## chapter 10 :

**CSS** allows you to create rules that specify how the content of
an element should appear

* The key to understanding how CSS works is to
imagine that there is an invisible box around
every HTML element.

**block element** Block level elements look
like they start on a new line.
Examples include the <h1>-
<h6>, <p> and <div> elements

**inline element** Inline elements flow within the
text and do not start on a new
line. Examples include <b>, <i>,
<img>, <em> and <span>.

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts:**a selector and a declaration**

*Selectors* indicate which
element the rule applies to.
The same rule can apply to
more than one element if you
separate the element names
with commas.

*Declarations* indicate how
the elements referred to in
the selector should be styled.
Declarations are split into two
parts (a property and a value),
and are separated by a colon.

#### External CSS : 

1. The <link> element :can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page.

2. href:This specifies the path to the
CSS file (which is often placed in
a folder called css or styles 

3. type:This attribute specifies the type
of document being linked to. The
value should be text/css.

#### CSS Selectors
 allow you to target rules to specific elements
in an HTML document. 

1. Universal Selector
2. Type Selector
3. Class Selector
4. ID Selector1.
5. Child Selector
6. Descendant Selector
7. Adjacent Sibling
8. Selector
9. General Sibling
10. Selector

* Different types of selectors allow you to target your
rules at different elements

Rules are made up of **selectors** (that specify the elements the rule applies to) and **declarations** (that
indicate what these elements should look like)

**Declarations** are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. 


#  Duckett JS

## Chapter 2:

* **script** is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

* You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 

/* Th i s script displays a greeting to the user based upon the current time.
It is an example from JavaScript & jQuer y book */ 

MULTI-LINE COMMENTS (/* note */)
SINGLE-LINE COMMENTS (//note)

* **variables**: Variables are used to temporarily store pieces of information used in the script.
 - first you need to give it a name second asighn them to a value 

DATA TYPES :
1. NUMERIC DATA TYPE eg) 1234879
2. STRING DATA TYPE  eg) "jordan" "90" 
3. BOOLEAN DATA TYPE eg) true,fales

* **Array**: is a special type of variable. It doesn't
just store one value; it stores a list of values. 

* **operators** they allow programmers to create a single value from one or more values.
- ARITHMETIC OPERATORS
- STRING OPERATOR


## Chapter 4:

Scripts often need to behave differently depending upon how the user interacts with the web
page and/or the browser window itself. To determine which path to take, programmers often
rely upon the following three concepts: 
1. evaluation
2. DECISIONS
3. loops

* There are two cmponents to a decision:
1. an expression is evaluated , which returns a value
2. a conditional statment says what to do in a given situation 

comparison operators :
* == is equalto
* != is not equal to
* === strict equal to
* !== strict not equal to 
* >< greater than less than 
* >= =< greater than or equal to ,less than or equal to 

logicaloperators:
* && logical and
* || logical or 
* ! logical not 

#### loops
- for loop
- while loop 
- do while loop 