# html Book
### Images:

- You can control the size of an image using the width and height properties in CSS, just like you can for any other box. 
Rather than using the <img> element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:

1. The float property is added to the class that was created to represent the size of the image

2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page.
These class names are used in addition to classes that indicate the size of the imag

* there are two common ways in which you can horizontally center an image:
1. On the containing element, you can use the text-align property with a value of center.
2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

The background-image property allows you to place an image behind any HTML element.

* Repeating images:
- background-repeat
1. repeat
The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat property isn't used).
2. repeat-x
The image is repeated horizontally only (as shown in the first example on the left).
3. repeat-y
The image is repeated vertically only.
4. no-repeat
The image is only shown once.


- background-attachment
1. fixed
The background image stays in the same position on the page.
2. scroll
The background image moves up and down as the user scrolls up and down the page

*The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property.*

* it is possible to create a link or button that changes to a second style when a user moves their mouse over it (known as a **rollover**) and a third style when they click on it.

- When a single image is used for several different parts of an interface, it is known as a **sprite**. 


If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible:
1. High Contrast:The majority of photographs have quite a high contrast, which means that they are not ideal for use as a background image.
2. Low Contrast : Image editing applications such as Photoshop and GIMP have tools that allow you to manually adjust your images to have lower contrast.
3. Screen :To overlay text on an image with high contrast, you can place a semi-transparent background color (or "screen") behind the text to improve legibility

### Chapter 19:
- SEO is a huge topic and several books have been written on the subject. The following pages will help you understand the key concepts so you can improve your website's visibility on search engines.

* In every page of your website there are seven key places where keywords :
1. Page Title: The page title appears at the top of the browser window or on the tab of a browser. It is specified in the <title> element which lives inside the <head> element.

2. URL / Web Address: The name of the file is part of the URL. Where possible, use keywords in the file name.

3. Headings: If the keywords are in a heading <hn> element then a search engine will know that this page is all about that subject and give it greater weight than other text.

4.  Text: Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read

5. Link Text: Use keywords in the text that create links between pages (rather than using generic expressions such as "click here").

6. Image Alt Text: Search engines rely on you providing accurate descriptions of images in the alt text. This will also help your images show up in the results of image-based searches.

7. Page Descriptions: The description also lives inside the <head> element and is specified using a <meta> tag. It should be a sentence that describes the content of the page. (These are not shown in  the browser window but they may be displayed in the results pages of search engines.)

* Determining which keywords to use on your site can be one of the hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.
1. Brainstorm
2. Organize
3. Research
4. Compar
5. Refine
6. Map

**Analytics**: Learning about your Visitors
- As soon as people start coming to your site, you can start analyzing how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics

The overview page gives you a snapshot of the key information you are likely to want to know. In particular, *it tells you how many people are coming to your site.*

- The traffic sources link on the left hand side allows you to learn where your visitors are coming from:
1. Referrers
This shows the sites that have linked to you and the number of people who have come via those sites. 
2. Direct
This shows which page a user arrived on if they did not come via a link on another site.
3. Search Terms
This shows the terms users entered into a search engine to find your site. This can help you learn how visitors describe what they're looking for


- In order to put your site on the web you will need a domain name and web hosting:

* **DOMAIN NAMES** WEB HOSTING Your domain name is your web address (e.g. google.com or bbc. co.uk). There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name.

* **WEB HOISTING** So that other people can see your site, you will need to upload it to a web server. Web servers are special computers that are constantly connected to the Internet. They are specially set up to serve web pages when they are requested

**Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website  tools (to save you writing them from scratch)**


- To transfer your code and images from your computer to your hosting company, you use something known as **File Transfer Protocol.**
Here is a list of some popular
- FTP applications:
- FileZilla
filezilla-project.org
Windows, Mac, Linux
- FireFTP
fireftp.mozdev.org
Windows, Mac, Linux
- CuteFTP
cuteftp.com
Windows, Mac
- SmartFTP
smartftp.com
WIndows
- Transmit
panic.com/transmit
Ma