# Class 26 Reading Notes

## React Quick Start

1. What are the building blocks of a React app?

- Components - break the UI into a component hierarchy then build a static versionin React with no interactivity. Find the minimal representation of UI state and identify where state should live then add inverse data flow.

2. What is the difference between an HTML element and a React component?

- HTML elements are static, native to web browsers and have limited interactivity. React components are dynamic, they are custom elements and are highly interactive.

3. What is JSX and why do we use it?

- A syntax extension for JS used in React to define the structure and layout of UI. It allows devs to write HTML code in JS.

4. Describe the process of embedding JavaScript expressions in JSX.

- In JSX, you can embed JavaScript expressions and code within curly braces.

5. Does React or JSX have any special features for iteration or conditional logic?

- Conditional rendering in JSX -> with ternary operator or logical && operator.
- Iteration in JSX -> using .map() for lists to iterate over an array. Use array.map() with components to iterate over an array of data.

6. How does React know to respond to a user’s inputs?

- React responds to user input through event handling and componenet based architecture.

7. What word indicates that a React component manages data with a Hook?

- Hooks are designed for managing state, side effects etc so 'useState', 'useEffect', 'useContext' are Hook functions

8. How can two react components share data?

- Through props, callback functions

## Render & Commit

1. What are the three steps of refreshing a React UI?

- Triggering a render
- Rendering the component
- Commiting to the DOM

2. How do you trigger updates to a component after the initial render?

- You can trigger renders by updating its state with the set function, updating state auto queues a render.

3. Does React recreate DOM nodes on every rerender?

- No, it reconciles the updated parts of the DOM that have been changed.

4. After React has updated the DOM, what still needs to happen before the user sees the change?

- Repaint - redrawing the pixels ont he screen to reflect changes in the DOM