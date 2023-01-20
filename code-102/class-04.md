# Class 4 Reading Notes

## Wireframing

> Allows to define and plan info hiearchy of design for a website/app/etc based on how you want the user to process the info (based on user info)

- Good way of getting to know how a user interacts with the interface through positioning of buttons and menus by using plain black and white diagram design of where info is going to go - this allows you to plan the layout and interactions without the distracrion of colors and typeface

- hand drawing initial design of how the site will look is easiest to change before designing it on a computer - draw where the head image will go and what will be written there and where it will be written, draw the buttons (calls to action) like log in button on top right corner, draw where the logo will go if it's for a company; etc.

Process can look like this:
SKetch - wireframe - interactive prototype - visual design - code

**wireframing online tools = UXPin, InVision, Wireframe.cc**

1. Understand your audience first to best know how the layout should be when you start wireframe design; detail requirements; create user personas and define use cases; dig into UX trends 
- introducing tracking and data visualization try **Dribbble** and **Behance**

2. Prepare research for reference

3. Have user flow mapped out

4. Don't get lost in the tiny details at this stage; focus on:
- organizing content for user's goals
- most important info
- what to expect where on a page (like where does the log in button go?)
- which buttons or touch points to complete an action?

5. Add detail - usability; calls to actions; etc

6. Run Wireframes into prototypes - can use something like Adobe XD and import to InVision

## **HTML BASICS**

> Structures a web page and its content (paragraphs, bulletet points, images, data tables, etc)
- consists of elements; enclosing tags can make a work or image hyperlink to somewhere else, can italicize, change font size, etc.

- *Element* = opening tag, content, clsoing tag 

- *Attributes* = extra info about the element that you don't want to appear in the actual content; 
    ex) < p class = "editor-note" >My cat is grumpy< / p >
    Class is the *attribute name* - "editor note" = *attribute value*
    - *class attribute* allows to give the element a non-unique identifier that can be used to target it and other elements with same *value*
    - attributes that set a value always have a space between it and element name, attribute name followed by = sign, attribute value wrapped by open and close quotation marks

- *Nesting Elements* = elements inside other elements - can do this to make a word bold, italic, underlined, etc - has to be surrounding the word(s) you want it to affect

- *Void Elements* = has no content (ex. <img>) an image has no inner content, is an element meant to be embeded - img needs source attribue (src)

HTML consists of headings, paragraphs, lists (unordered and ordered), links

## Semantics

> Refers to the *meaning* of a piece of code; what purpose or affect of JavaScript or HTML have 

- search engines consider content important to influence page's SEO
- helps visually impaired users navigate page
- finding blocks of meaningful code easier
- suggests type of data 
- mirrors custom element/component name