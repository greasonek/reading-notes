# Class 38 Reading Notes

## Redux - Asynchronous Actions

### Async Actions

1. Why use Redux middleware?

- Middleware allows the app to perform necessary 'side effect' actions like loggin a value, saving a value, allowing asynchronous behavior, modifying state that exists outside of a function or mutating arguments to a function. Middleware can do *anything* when it sees a dispatched action. Redux middleware also allows us to pass asynchronous functions to dispatch instead of just action objects.

2. Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

- A user input action is triggered like a click of a button, the event is sent to the event handler function and dispatched as an action to the middleware. The middleware receives the action and sends the request to the API, the API processes the request and sends a response back to the middleware which continues the dispatched action to the store. The store holds the reducer and the state is sent to the reducer along with the dispatched action. State is modified here and the action response is continued to completion where the user can now see the change per their initial input action.

3. How are we accommodating async in our Redux app?

### Thunk Middleware

1. Why would you need redux-thunk middleware?

- Redux-thunk middleware allos us to write functions that can interact with the sotre's dispatch and getState methods. The functions can have async logic that can dispatch actions and read the store state as needed.

2. Redux Thunk middleware allows you to write action creators that return a **_FUNCTION_** instead of an action.

3. Describe how any return value from the inner thunk function will be made available.

- A return value from the inner function will be available as the return value of dispatch itself.
