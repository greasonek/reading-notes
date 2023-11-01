# Reducers

## Multiple Reducer Examples

1. Why create multiple reducers?

- To manage multiple parts of a complex application state. Modularization and maintaibability, scalability by being able to add more reducers to handle pieces of state, reusability across parts of the app.

2. How would you combine multiple reducers?

- combineReducers() creates a single root reducer. Create individual reducers, define initial state, combine reduders.

3. How will you manage state as an immutable object? why?

- create new state objects based on previous state and action payload.

## Redux Docs: Using Combined Reducers

1. combineReducers is a utility function to simplify the most common use case when writing _**REDUX**_ _**REDUCERS**_ .
2. Explain how combineReducers assembles the new state tree.

- Each reducer function defines initial state for specific slice of state before actions are dispatched, combineReducers combines multiple of these into a root reducer by passing in an object where each key represents a slice and the value is the render function managing that slice.

3. How would you define initial state in an app using combineReducers?

- initial state refers to the initial values of each state slice being managed by the combined reducers.

## Redux Docs: Combined Redux Syntax

1. Why will you want to split your reducing functions as your app becomes more complex?

- By splitting reducer functions you are able to manage independent parts of state for the app.

2. The **_combineReducer_** helper function turns an object whose values are different reducing functions into a single reducing function you can pass to **_createStore_**.
3. What is a popular convention when naming reducers?

- Name reducers after the state slices they manage for property shorthand notation.
