# Class 9 Reading Notes

## How to Structure a Web Form

- **form element** defines a form and attributes that will determine the form's behavior **never nest forms inside of forms**

- **fieldset element** creates groups of widgets that share same purpose for styling and semantics; can label by using a *legend element* below the opening tag - text content of legend defines purpose of the fieldset
  - for long forms, putting different related sections inside different fieldsets improves usability

- **label element** - most important element for building accessible forms; **for attribute** ensures assistive technologies understand relationship between widget and label

1. Forms are important to web development because they help gather information from the users and they create interaction between a visitor and the site. 

2. Key things to keep in mind when designing a form for user experience is accessibility. Some screen readers will read the form's code differently. 

3. 5 form elements include form, fieldset, label, legend and section. Form element defines a form and attributes that will determine the form's behavior. Fieldset creates groups of widgets that share same purpose for styling and semantics. Label is the most important element for building accessible forms. Legend element labels a fieldset element and the conent of the legend describes the purpose of the fieldset. Section functionality is used to create a container for each set of separate functionality.  


## Intro to Events

- **Events** things that happen in the system being programmed that the system will tell you about so the code can react to them (<a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events">Source</a>)
  - need an **event handler (event listener)** to react to an event - block of JS code that runs when event fired.
    - ex) user clicks button to change background color of the page and event handler code is as follows:
    const btn = document.querySelector("button");

function random (number)  {
  r eturn Math. floor(Math.random() * (number + 1));
}

btn.addEventListener ("click", () => {
  c onst rndCol  = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
  document.body. style.backgroundColor = rndCol;
} ) ;
  <a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events">example source</a>

1. How would you describe events to a non-technical friend? An event is something that happens in a webpage like the user is interacting with the webpage by clicking a button, and the event will tell the code to react by displaying what the user is intending to see. So if the user clicks a button that says "see more info here" the code will react by showing them the info they're clicking to see.

2. When using the addEventListener() method, what 2 arguments needed are one to indicate that we want the code to listen to the event occuring and a function to call when the event is happening.

3. **Event Object (event, evt, or e)** is passed to event handlers to provide extra features and info.  The target within the event object is a reference to the leement the event occured upon so if the user clicked a button to change the background color of a page, the button is the target of the event, not the page. (<a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events">source</a>)

4. **Event bubbling** describes how the browser handles events targeted at nested elements while **event capturing** is the same thing but in reverse. Instead of the event firing on the inner element targeted, it fires on the outside elements first, then on the inner elements. 