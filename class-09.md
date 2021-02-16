## html book

#### Chapter 7:

- HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to
your site.

*There are several types of form controls that you can use to collect information from visitors
to your site.
1. ADDING TEXT
2. Making Choices
3. Submitting Forms

* How Forms Work
- A user fills in a form and then presses a button to submit the information to the server.
- The name of each form control is sent to theserver along with the value the user enters or selects
- The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
- The server creates a new page to send back to the browser based on the information received.

* Form Structure
1. <form>
Form controls live inside a<form> element. This element should always carry the action attribute and will usually have a method and id attribute too
2. action
Every <form> element requires an action attribute. Its value is the URL for the page on theserver that will receive the information in the form when it is submitted
3. method
Forms can be sent using one of two methods: **get** or **post**.

**The get**                                               
method is ideal for:
* short forms (such as search boxes)
* when you are just retrieving data from the web server (not sending information that should be added to or deleted from a database)

**post method** :
* allows users to upload a file
* is very long
* contains sensitive data(e.g. passwords)
* adds information to, or deletes information from, a database.

<input>
The <input> element is used to create several different form
controls. The value of the type attribute determines what kind of input they will be creating.

*type="password"* When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking overthe user's shoulder, they cannot see sensitive data such as passwords

- <textarea>
The <textarea> element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag

- *type="radio"*
Radio buttons allow users to pick just one of a number of options.

- *type="checkbox"* Checkboxes allow users to select (and unselect) one or more options in answer to a question.

- <select>
A drop down list box (also known as a select box) allows users to select one option from adrop down list.

- *type="file"* This type of input creates a box that looks like a text input followed by a browse button. 

- type="submit" The submit button is used to send a form to the server.

- <button>
The <button> element was introduced to allow users more
control over how their buttons appear, and to allow other
elements to appear inside the button.
This means that you can combine text and images between the opening <button>
tag and closing </button> tag.

The <label> element can be used in two ways. It can:
1. Wrap around both the text description and the form input
(as shown on the first line of the example to your right).

2. Be kept separate from the form control and use the for
attribute to indicate which form control it is a label for (as shown
with the radio buttons)


Grouping Form Elements:
<fieldset>You can group related form controls together inside the
This is particularly helpful for longer forms. Most browsers will show the fieldset with a line around the edge to show how they are related. The appearance of these lines can be adjusted using CSS

*HTML5 introduces new form elements which make it easier for visitors to fill in forms.*

**Validation** helps ensure the user enters information in a
form that the server will be able to understand when the form is submitted:
- Reduce the amount of work the server has to do
- Enables users to see if there are problems with the form faster than if validation were
performed on the server.


#### Chapter 14:
list-style-type :allows you to control the shape or style of a bullet point (also known as a marker).

* Unordered Lists
For an unordered list you can use
the following values:
 none
 disc
 circle
 square
* Ordered Lists
For an ordered (numbered) list
you can use the following values:
- decimal
1 2 3
- decimal-leading-zero
01 02 03
- lower-alpha
a b c
- upper-alpha
A B C
- lower-roman
i. ii. iii.
- upper-roman
I II III


*You can specify an image to act as a bullet point using the list-style-image property*

* Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points:
1. outside
2. inside

*list-style, and it allows you to express the markers' style, image and position properties in any order*

*  use the *empty-cells* property to specify whether or not their
borders should be shown. Since browsers treat empty cells in different ways, if you want to explicitly show or hide borderson any empty cells then you should use this property. It can take one of three values:
1. show
2. hide
3. inherit

**font-size** sets the size of the text entered by the user.
**color** sets the text color, and
**background-color** sets the background color of the input.
**border** adds a border around the edge of the input box, and
**border-radius** can be used
to create rounded corners (for browsers that support this property).
**focus** pseudo-class is used to change the background color of the text input when it is being used
**hover** psuedo-class applies the same styles when the user hovers over them

### javascript book:

##### Chapter 6:
 - Scripts often respond to these events by updating the content of the web page  which makes the page feel more interactive.

 DIFFERENT EVENT TYPES:
 1. UIEVENTS Occur when a user interacts with the browser's user interface (UI) rather than the web page
 2. KEYBOARD EVENTS Occur when a user interacts with the keyboard (see also input event)
 3. MOUSE EVENTS Occur when a user interacts with a mouse. trackpad, or touchscreen

- When an event has occurred, it is often described as having fired or been raised. In the diagram on the right, if the user is tapping on a link, a
cl ick event would fire in the browser.
- Events are said to trigger a function or script. When the click event fires on the element in this diagram, it could trigger a script that enlarges
the selected item. 

4. FOCUS EVENTS Occur when an element (e.g., a link or form field) gains or loses focus 
5. FORM EVENTS Occur when a user interacts with a form element
6. MUTATION EVENTS Occur when the DOM structure has been changed by a script 

**event handling** :When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code.
steps:
- Select t he element node(s) you want the script to respond to. 
- Indicate which event on the selected node(s) will trigger the response. 
- State the code you want to run when the event occurs

* THREE WAYS TO BIND AN EVENT TO AN ELEMENT :
1. HTML EVENT HANDLERS:This is *bad practice*, but you need to be aware of it because you may see it in older code.
2. TRADITIONAL DOM EVENT HANDLERS :All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler.
3. DOM LEVEL 2 EVENT LISTENERS : more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers. 

*Because you cannot have parentheses after the function names in event handlers or listeners, passing arguments requires a workaround.*

- When an event occurs, the **event object** tells you information about the event, and the element it happened upon. 

1. The function is called check Length() rather than checkUsername (). It can be used on any text input.
2. The event object is passed to the event listener. The code includes fallbacks for IES-8
3. In order to determine which element the user was interacting with, the function uses the event object's target property (and for IES-8 it uses the equivalent s rcEl ement property)

Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element

* BENEFITS OF EVENT DELEGATION:
 - WORKS WITH NEW ELEMENTS 
 - SOLVES LIM ITATIONS WITH this KEYWORD
 - SIMPLIFIES YOUR CODE

The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event. 
- reventDef au 1t () 
- stopPropagation() 
- USING BOTH METHODS 

When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see
the approach below used; it relies on the **this** keyword:The this keyword refers to the owner of a function

* Events are defined in:
- The W3C DOM specification
- The HTMLS specification
- In Browser Object Models 

User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it, e.g., a page having loaded or the browser window being resized. 

The HTML elements you can interact with, such as links and form
elements, can gain focus. These events fire when they gain or lose focus. 

The **mouse events** are fired when the mouse is moved and also when its
buttons are clicked. 
- *mousedown* Fires when the user clicks down on any mouse button.
- *mouseup* Fires when the user releases a mouse button.
- *mouseover* Fires when the cursor was outside an element and is then
moved inside it
- *mouseout* Fires when the cursor is over an element, and then moves onto another element - outside of the current element or child of it 
- *mousemove* Fires when the cursor is moved around an element. This event is repeatedly fired

* The aim of this example is to use the **c1ick** event to remove the big note that has been added to the middle of the page. 
The keyboard events are fired when a user interacts with the keyboard 

The **keyboard events** are fired when a user interacts with the keyboard 

input Fires when the value of an <input> or <textarea> element changes
keydown Fires when the user presses any key on the keyboard.
keypress Fires when the user presses a key that would result in a character being shown on the screen.
keyup Fires when the user releases a key on the keyboard

**MUTATION EVENTS & OBSERVERS** 
is triggerd by Whenever elements are added to or removed from the DOM, its
structure changes. 

*Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.*

*The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events*