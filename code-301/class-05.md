# Class 5 Reading Notes

## Thinking in React

> 5 Steps of implementing UI in React:

- Break the UI into a component hierarchy: drawing and naming components/subcomponents in mockup, consider CSS class selectors, consider how to organize design's layers.

- Build a static version in React: Build a version that renders UI with components and props, but not state as state adds interactivity. Can build top down (simple projects) or bottom up (larger projects).

- Find minimal but complete representation of UI state

- Identify where state should live

- Add inverse data flow - add event handlers so the user input will change state

1. What is the single responsibility principle and how does it apply to components?

- A programming technique wherein a component should only do one thing. If the component grows and has more responsibilities, it should be decomposed into smaller subcomponents.

2. What does it mean to build a ‘static’ version of your application?

- The 'static' version is one that renders the UI from the data model without any interactivity. Build using components that props, but not state.

3. Once you have a static application, what do you need to add?

- Add state to implement interactivity to the static version of the app.

4. What are the three questions you can ask to determine if something is state?

- Does it remain unchanged over time? If so, it isn't state.
- Is it passed in from a parent via props? If so, it isn't state.
- Can you compute it based on existing state or props in your component? If so, it isn't state.

5. How can you identify where state needs to live?

- Identify every component that renders something based on that state, then find the closest common parent components (above in the hierarchy), often times the state can go in the common parent component or it can go in the component above the common parent. If neither of these options makes sense, make a new component for holding state.

## Higher-Order Functions

- Can create new functions, change other functions, and can provide new types of control flow.

1. What is a “higher-order function”?

- *higher order functions* are functions that operate on other functions by either taking them in as arguments or returning them. They allow us to abstract over actions, not just values and come in several forms.

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

- Line 2 is taking the value of m and returning it as a value that is greater than n. So if the value of n is 10, m will return as a value greater than 10.

3. Explain how either map or reduce operates, with regards to higher-order functions.

- Map can be used to produce a new array of elements that is based off of the original input array. For example, if we have an array that has been filtered and we want to return it's elements as a new value, like a name, we would use map to transform the input array and return a new array of names for those elements.
