# Class 31 Reading Notes

## Choosing the State Structure

1. Summarize the five principles for structuring state.

- Group related state -> if updated more than one state variables at the same time, merge them to a single state variable
- Avoid contradictions in state -> avoid situations where state is structured in a way that pieces of state disagree with one another
- Avoid redundant state -> if info can be calculated from props or during rendering, don't have it in state as well
- Avoid duplication in state -> don't have the same data duplicated in multiple state variables to avoid confusion
- Avoid deeply nested state -> it is not convenient to update hierarchical state

## Passing State Deeply with Context

1. What problem do Contexts aim to solve?

- Context lets a parent component provide data to the entire tree. It also lets you write components that adapt to their surroundings.

2. What is one technique to try before useContext?

- Passing props. This provides explicit data flow on projects with more than one dev.

3. What hook complements useContext for complex applications?

- useReducer is commonly used with useContext to manage complex state and pass it down to distant components.
