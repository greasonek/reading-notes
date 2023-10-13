# Class 32 Reading Notes

## Scaling Up with Reducer and Context

1. How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose.)

- useReducer and useContext can be combined so that other components can read and update state above it. To do this there are three over-all steps: create contexts, provide contexts from components where reducer is used, use context from components that need to read them. So context would be created for state and for dispatch functions for example but many context-reducer pairs can be created. All of this wiring can live in a single file and export the component that provides context.
