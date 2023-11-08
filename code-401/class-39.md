# Class 39 Reading Notes

## Redux - Additional Topics

### Redux Toolkit (RTK)

1. What concerns are addressed by Redux Toolkit?

- The complicated nature of configuring a Redux store, adding multiple packages to get Redux to work, oversaturation of boilerplate code.

2. What does configureStore() do?

- Wraps createStore() to provide simplified configuration options. It combines slice reducers, adds middleware you provide and includes redux-thunk.

3. How would I use createSlice()?

- CreateSlice() simplifies the process of creating Redux slices. You can define the reducer and action creators in a straightforward manner. Start by defining a name, the initialState for the slice and the reducers (objects that define reducer functions for the slice). Reducer function should take the current state + an action as arguments and be used to modify state.

### MobX

1. What is Mobx?

- A library that provides a scalable state management solution by making it impossible to produce inconsistent state.

2. How does MobX make it “impossible” to produce an inconsistent state?

- Make sure that everything that can be derived from the application state will be derived automatically. So when observalbe values change, MobX automatically re-evaluates and updates any computed values and components that depend on it.

3. How would we build a reactive user interface?

- We can alter the class constructor to make things in state observable to signal MobX that the values may change over time. When the observable variables change, they are detected and changes are made automatically to anything that depends on them.
