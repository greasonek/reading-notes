# Class 27 Reading Notes

## Thinking in React

1. Summarize the five steps of thinking in react.

- **Step 1**: *Break the UI into a component hierarchy* - Draw boxes around each component in the mockup, compenent can be split in different ways (programming, CSS, design); UI and data models often have the same info architecture - separate UI into components where each one matches a piece of the data model

![component-mockup](./imgs/Screenshot%202023-09-26%20at%206.02.09%20PM.png)

- **Step 1**: *Build a static version in React* - Build a version of the app that renders the UI from the data model with no interactivity. Build components that reuse other components and pass data using **props**. The component at the top of the hierarchy will take the data model as a prop (*one way data flow* - data flows one way top down)

- **Step 3**: *Find the minimal but complete representation of UI state* - To make the UI interactive, need to let users change data model using *state*.

- **Step 4**: *Identify where your state should live* - Identify which component is responsible for changing state. Identify every component that renders something based on state, find their closest common parent component, decide where state should live (often can be inside common parent, can be in a component above the parent, can make one solely for holding state); **Hook - special functions that let you 'hook' into React (ex: useState())**

- **Step 5**: *Add inverse data flow* - add onChange event handlers to allow the user to change state

## State: A Component's Memory

1. What is one reason a local variable isn’t sufficient for managing a React component?

- Local variables don't persist between renders. It renders from scratch and therefore does not consider changes made to the local variables. Changes to local variables don't trigger renders.

2. What is the argument to the useState hook, and what are the two parts of its return array?

- The argument is the initial value of the state variable. The return array contains a state variable to retain data between functions and a setter function to update the variable and trigger React to render the component again.

3. How can Component A access state from Component B?

- Pass the state down as props from B to A if B is the parent of A, or create a new component to hold the parent and pass it down as props.
