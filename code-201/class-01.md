# Class 1 Reading Notes

## How the Web Works - 

> Understanding what happens in the background of the web
- Computers connected to internet = *clients* and *servers* - client sends request to server, server responds to client

- Clients = devices and web-accessing software (Chrome, Safari, etc)

- Servers = computers that store web pages, apps, etc. 

- TCP/IP = Transmission Control Protocol and Internet Protocol - define how data travels across internet

- DNS = Domain Name System - yellow pages for websites

- HTTP = Hypertext Transfer Protocol - defines language for servers to speak to each other

- Code files (html, css, JS); Assets (images, videos, music, PDFs etc)

### What Happens? 

- Browser goes to DNS server, finds address and sends HTTP request message to server using TCP/IP, if approved, server sends “200 OK” message and sends files to the browser which is then assembled to complete a web page

- Browser sends requests to servers for HTML files containing <link> elements (external CSS stylesheets) and <script> elements (external JS scripts) - order is important! - generates DOM tree for parsed HTML, generates CSSOM structure from parsed CSS, compiles and executes parsed JS - as this is done the user sees the visual representation of all these elements and can interact with it

- DNS - makes a web address (like google.com) that matches the IP address of the website that looks something like 64.345.234.98
Components of website sent in smaller chunks so exchange is faster and website more efficient

## Website Design and Process -

> What does the website look like? What does it do and how do users aesthetically interact with the information it provides?

- Ask yourself what is your website about? What info is presented on the subject - write title and paragraph, maybe an image -What does the website look like? 

- Adding images - add filter to google image search to avoid copyright infringement by clicking **Tools** button then **Usage rights** option, choose **Creative Commons License** – find an image, right click and save image as OR copy image’s web address
   
## JavaScript Basics - What is JavaScript? 

> JS adds interaction to the webpage, can create games, identify behavior responses between users and webpages, create data forms, buttons that are interactive, and create animation. 

- Functionality includes browser APIs (to create HTML and CSS, generate 3D graphics, etc) 3rd party APIs to include functionality from other sites (like Twitter, Facebook, IG) and 3rd party frameworks

- *browser reads code in order it appears in file*

- *Variable* is a container that stores value, declared with the “let” keyword followed by the name you give the variable (Ex. let myVariable;) ← can give the variable a value (ex. myVariable = Bob”; **or** let myVariable = “Bob”;) → after assigning value to variable, can change it later in the code. Variables are necessary to do anything dynamic like personalize a page greeting or change an image in an image gallery or customize a data entry box

- String - signified by ‘ ‘ or “ “ around the value (ex) let myVariable = “Bob”; → “Bob” is the string.

- Number - doesn’t have quotation marks (ex) let myVariable = 10; 

- Boolean - a true/false sort of statement

- Array - allows to store multiple values in a single reference (ex) let myVariable = [1,’Bob’10];

- Object - can be anything (Ex) let myVariable = document.querySelectgor(‘h1’); (or any above examples)

1. POEM?

2. Browser sends requests to servers for HTML files containing <link> elements (external CSS stylesheets) and <script> elements (external JS scripts) - order is important! - generates DOM tree for parsed HTML, generates CSSOM structure from parsed CSS, compiles and executes parsed JS - Components of website sent in smaller chunks so exchange is faster and website more efficient

3. Adding images - add filter to google image search to avoid copyright infringement by clicking **Tools** button then **Usage rights** option, choose **Creative Commons License** – find an image, right click and save image as OR copy image’s web address

4. Strings and Numbers are types of values that can attributed to a variable, a sting differs from a number in that it is encased with ‘ ‘ or “ “ → let myVariable = “10”;  is a sting whereas let myVariable = 10; is a number

5. Variable is a container that stores value, declared with “let” keyword followed by the name you give the variable (Ex. let myVariable;) ← can give the variable a value (ex. myVariable = Bob”; **or** let myVariable = “Bob”;) → after assigning value to variable, can change it later in the code. Variables are necessary to do anything dynamic like personalize a page greeting or change an image in an image gallery or customize a data entry box


## HTML

> HTML tells the browser how to structure a web page - consists of elements and tags

- Anatomy of HTML consists of opening tag, content, closing tag (<p>Hello World!</p>)

- Nesting - elements placed within other elements

- Block vs Inline elements - block elements = <heading><li><nav> or <footer> - create a new line; inline elements are contained within block elements(<a> creates hyperlink, <em> or <strong> create emphasis; do not create a new line

- Void elements do not contain closing tag (ex, <img>)

- *Attributes* -  extra info about the element that won’t appear in the content. For example, class attribute targets element with style info - should have space, equal sign, and value wrapped in quotations (ex, <p class=”editor-note”>Hello World</p>

- <a> anchor tag - can have number of attributes including **href**, **title**, **target** (displays link in a new tab)
ex) <p>A link to my <a href="https://www.mozilla.org/" title="The Mozilla homepage" target="_blank">favorite website</a>.</p>

- Boolean attributes = those without values, can only have one value which is the same as the attribute name. 

### Anatomy of HTML document 

> !DOCTYPE html> starts every page
- <html></html> is the root element, wraps all content on the page

- <head></head> container for everything that isn’t content shown to viewer (like <title></title> or keywords or page description for search results or CSS, etc)

- <meta> element contains metadata like <base> <script> <link> <style>; <charset> attribute sets character set for document to UTF-8 which includes most characeers from majority of written languages *(<meta charset=”utf-8”>*

- <title> sets title of page that appears in tab the page is loaded in. 

- <body></body> contains all content displayed on page

### Website Structure

- Header, nav bar, main content, sidebar (<aside>), footer

- HTML ELEMENTS - main, used once per page inside body. <article> encloses a block of related content that makes sense without the rest of the  content of the page like a blog post while <section> groups together a part of the page that makes up a single piece of the functionality like a set of article headlines or a theme. <article>s can be broken up into different <section>s and visa versa, header (intro content) nav bar to secondary links, and footer

- non-semantic wrappers - <div> <span> 

### Metadata in HTML

- <title> appears in bookmark tab or in tab when you open a webpage in browser, <h1> is part of the content of the page is is top level heading to body content

- Specifying description with metadata including keywords relating to content of the page is useful in making the page appear higher in search engines 

1. Attribute = extra info about the element that won’t appear in the content. For example, class attribute targets element with style info

2. Anatomy of HTML element - consists of opening tag, content, closing tag (ex. <p>Hello World!</p>

3. <article> encloses a block of related content that makes sense without the rest of the  content of the page like a blog post while <section> groups together a part of the page that makes up a single piece of the functionality like a set of article headlines or a theme. <article>s can be broken up into different <section>s and visa versa

4. A typical web page structure contains the following elements: header, navigation bar, main content, sidebar and a footer (<header></header>, </nav></nav>, <main></main>, <aside</aside>, <footer></footer>)

5. <meta> element contains metadata like <base> <title><script> <link> <style>; <charset> attribute sets character set for document to UTF-8 which includes most characeers from majority of written languages *(<meta charset=”utf-8”>*



## Miscellaneous

### Designing a website

1. First step to designing a website is **product ideation** where essential questions must be answered: what do I want to accomplish? How will my website help me reach my goals? What needs to be done, in what order, to reach my goals? 

2. Most important question to answer when designing a website is “What do I want to accomplish?” because this question drives everything else. List all the goals you want to reach and prioritize from most to least important. 

### Semantic

> *semantics* = meaning of a piece of code – name describes data (ex. <article>, <footer>, <header>, <main>, <nav>)

1. You use an <h1> element over a <span> element to display top level heading because by default, most browser’s stylesheets will style an <h1> element with a large font size to make it **look** like a heading. <span> will render it to look like a top level heading, it has no semantic value and is just a presentation which is CSS’s job. HTML should be coded to represent data, not presentation. 

2. Benefit of using semantic tags in HTML? Good for SEO, search engines will consider it as important key words to influence a page's reach. Screen readers can use it to help visually impaired users. Finding blocks of meaningful code is easier than searching through div’s. The names of semantic tags describe the data being populated. 

### JavaScript

1. Two things that require JS in the browser are browser APIs (built into web browsers) and 3rd party APIs (not built into browsers but can grab their code and info from somewhere else on the web like Google Maps or Twitter).

2. Add JS to an HTML document by using the <script> element and adding the JS file within your <head> tag.
