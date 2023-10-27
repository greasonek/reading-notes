# Class 36 Reading Notes

## REDUX

1. What is the first principle of Redux?

- Whether your app is simple or complex with a lot of UI and change of state

2. What is a store and what do we use our reducers for within that store?

- Store is an object that holds the state of the application. Reducers specify how the app's state changes in response to actions. Takes in current state and action and returns new state.

3. Name three Redux store methods given to us by createStore and describe their use.

- getState() retrieves current state of redux store
- dispatch() dispatches actions to change state
- subscribe() registers a callback that the redux store calls everytime and action has been dispatched so you can updated the UI of the application to reflect current app state

4. Explain to a non-technical recruiter what combineReducers() does and why it is useful.

- combineReducers() is an organizer that creates smaller reducers to handle different types of data. Like a filing cabinet where different folders hold different types of documents rather than dumping all the documents in the drawer with no organization.
