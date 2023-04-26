# Class 4 reading notes

## React Docs - Forms

- different from other DOM elements in React bc elements naturally keep some internal state

- in HTML, form elements maintain their own state and update it based on user input, in React, mutabile state is kept in the state property of components and only updated with setState()

- combine the two  by making React state be the 'single source of truth', then the React componenent that renders the form also controls what happens in that form on subsequent user input. This is called **'controlled component'**

1. What is a ‘Controlled Component’?

- An input form element whose value is controlled by React by making the React state the 'single sorce of truth' so it contorls what happens inthe form upon user input.

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

- The user's input value is always driven by the React state

3. How do we target what the user is entering if we have an event handler on an input field?

- adding a name attribute to each element and let the handler fuction choose what to do based on that value 

### The Conditional (Ternary) Operator Explained

1. Why would we use a ternary operator?

- makes code more concise and readable 

2. Rewrite the following statement using a ternary statement:
