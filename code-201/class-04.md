# Class 4 Reading Notes

## Creating hyperlink

- Block level links - 

- Make an img a link by using <a> element and referencing image with an <img> element. 
<a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks">for example</a>

<a  href= "https://www.mozilla.org/en-US/" >
  < img src="mozilla-image.png" alt="Mozilla homepage" />
< /a>

- URL’s use paths to find files - one directory contains the entire site (called the **root*) - contains index.html (can have multiple index.html’s if they’re in separate filesystem locations 

- **document fragment** - link a specific part of the html document, would need to assign an ID to the element you want to link. For instance, to link to the heading of a section of the page like <h2>, would need to assign ID to <h2>  → example: <h2 id=”contact_info”>Contact Info</h2> → then to link to this id you would add a “#” ex) <a href=”contacts.html#contact_info.”>Contact Info</a>

- **absolute** vs **relative** URL’s

- Absolute links to absolute location
- Relative points to a location relative to file you’re linking from

- When linking to something that is downloadable like music, image or PDF, add wording to reduce confusion (like for music, add “stream opens in separate tab)

1. To create a basic link, we wrap text inside a <a> (anchor) element with a “href” attribute.

2. The href attribute is a hypertext reference (or target) that contains a web address (URL). It can also contain a title attribute within the <a> tag that contains additional info about the page that is linked.

3. Include keywords in your link text to describe what is being linked to for screen readers.Descriptive link text is useful for visual readers who skim pages and whose eyes are drawn to page features. Don’t include URLs in link text. Screen readers tell user’s there is a link so there is no need to include “link” or “link to” in link text. Keep link text short and try to use different text in different link texts instead of using the same text in different places as this can become confusing to the user.

## CSS Layout - Normal Flow

- *Block Level* - appear within a <body> element; create larger structures than inline elements - can contain inline elements or other block level elements; by default block level content will start on a new line while inline elements can begin on the same line. Some “block level” elements include: <article>, <address>, <block quote> <details>, <dialouge>, <dd> (describes term in description list) <aside> (aside content), <div> (document division>, <dt> (description list term> , <footer>, <header>, <ol>. <ul>, <li> etc.

- *Inline* - presentational element and usually specified in CSS; cannot adjust width and heigh on inline elements, they sit in the content of the blocklevel elements (except images!! -- can be resized); to change size of inline element must make it behave like block level element by use of display:block or display:inline-block

- *Absolute positioning*: no longer exisits inthe normal document flow, it sits on its own layer allowig to create isolated UI features that don't interfere with the layout of other elements on the page like a pop up box

- *z-index* - references the z-axis (imaginary line running from surface of the screen to your face); determines the way things stack on the page if there are multiple elements with absolute positioning.

- *fixed positioning* - fixes element in place relative to visible portion of the viewport; ie. persistent nav menus, 'accept cookies' alerts, etc. 
ex. in CSS -->
    h1 {
        position: fixed;
        top:0; //fixes the h1 element to the top of the screen.
    }

- *sticky positioning* - hybrid of relative & fixed; allows for elements to behave like relative positioning until the user scrolls past a certain threshold then the element will become fixed. - used for scrolling index:
<a href="https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning">example:</a>

<dl>
  <dt>A</dt>
  <dd>Apple</dd>
  <dd>Ant</dd>
  <dd>Altimeter</dd>
  <dd>Airplane</dd>
  <dt>B</dt>
  <dd>Bird</dd>
  <dd>Buzzard</dd>
</dl>

< dt > elements in css will be given sticky positioning with top:0; so the "A" and "B" etc will stick to the top of the page as the user scrolls

1. Normal flow is the way elements lay themselves out on a webpage if you haven’t changed anything about their layout and no CSS is applied to change the way they behave. Normal flow is designed to make a web page easily readable for all users.

2. Block level elements appear within the <body> element of html and create larger structures than inline elements. They cancontain inline elements. By default, block level content will start on a new line while inline elements start on the same line. Inline elements are presentational. Unless it is an image, inline element's size cannot change, it must be changed with display:block or display:inline-block to behave like a block element.

3. Static positioning is the default for every html element.

4. Absolute positioning allows for isolated features like pop up boxes that don't interfere with other lements in the layout of the page.

5. Absolute positioning fixes elements in place relative to nearest positioned ancestor (or inital containing block), fixed positioning fixes an element in place relative to the visible portion of the view block ( <a href="https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning">source</a>)

## Functions - Reusable blocks of code

- **Functions** allow to store pieces of code that does single task inside defined block and then call back to that code when needed (rather than typing multiple times)

- **invoke** = run or execute

- **methods** - functions that are part of objects; 

- parameter - value that needs to be included in a function's parentheses to do it's job. Some are optional in which case the function will revert to a default behavior. 

- *Invoking* - used if you want to run a function after it's been defined. using name of the function followed by ()
ex) function myFunction() {
    alert('hello!');
}

1. A function must first be declared before it can be invoked. Declaring a funtion allows pieces of code that perform a task to be stored so it can be called back to (invoked) later in the code without having to be written again.

2. Parameters are values that need to be included in a functions parenteses for the function to do it's job. An argument is used to access the parameter passed to a function. It's only availabe within a function.

## 6 Reasons for Pair Programming

Greater efficiency + job interview readiness

Implementing the four fundemental skills that help with learning coding languages via pair programming would definitely make me a more efficient coder. It's one thing to listen to lecture and write based off of looking at someone else's code but describing the code and it's functions without actually typing out the code would help me to better understand what I'm coding, what it means, how it works, etc. Having the skills I will learn in pair programming would give me a leg up in the interview process in which I would need to work with another individual on a coding project. I will have already developed the collaboration and communication skills necessary to perform such a task. 

