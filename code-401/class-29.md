# Class 29 Reading Notes

## Extracting State Logic into a Reducer

1. What is the motivation for adding a reducer?

- Reducers are different ways to handle state.

2. What are actions in the context of a reducer? How are they different than setting state directly?

- Instead of telling React what to do by setting state, you specify what the user just did by dispatching actions frome event handlers (add, change, delete).

3. What common list operation is useReduce named for, and why?

- dispatch

4. When should you switch from useState to useReducer?

- Use useReducer if you often encounter bugs due to incorrect state updates in components
