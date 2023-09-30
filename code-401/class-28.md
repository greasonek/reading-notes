# Class 28 Reading Notes

## useEffect hook

1. What is the main intended use case for the useEffect hook?

- Connecting to an external system (APIs, 3rd party libraries, etc) while they're being displayed on the page.

2. How does the effect’s logic interact with the component?

- Two arguments need to be passed in (a setup function and a list of dependencies). The setup function has a setup code that connects to the system and a cleanup function with a cleanup code to disconnect. The list of dependencies includes every value from the component used inside those functions.

- After every re-render of your component where dependencies have changed, the cleanup code runs the old props and state and the setup code runs with the new props and state.

3. What is the importance of the return value from the effect’s logic function?

- It can be used to specify when the component updates.