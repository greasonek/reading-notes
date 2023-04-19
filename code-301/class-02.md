# React: Compotent Lifecycle Events

- **component lifecycle events**: compenents = classes or functions - methods used on these are lifecyle events - can be called during lifecycle of component and allow to update UI and app states

- *RENDER PHASE* - pure, no side effects, can be paused aborted or restarted

- *PRE-COMIT PHASE* - Can read DOM

- *COMMIT PHASE* - Can work with DOM, run side effects, schedule updates

- **3 PHASES OF THE COMPONENT LIFECYCLE**

- *MOUNTING PHASE* - When an instance of a component is being created and inserted into DOM: constructor, getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount **in this order**

- *UPDATING* - When a component is updated or state changes, it is re-rendered.

- *UNMOUNTING* - final stage; when component is removed from DOM; componentWillUnmount is the only lifecycle event in this phase

**constructor()** - called before is mounted; if is a subclass, call super(props) or the props will be undefined. can be used to assign state using this.state or to bind event handle methods to an instance

**componentDidMount()** - method is invoked immediately after a component is mounted; use to load anything using a network request or initialize the DOM; use to set up subscriptions(must also use componentWillUnmount to unsubscribe)

- where setState() is called - will cause a re-render

**shouldComponentUpdate()** - set to false prevents re-rendering after every state change

**componentWillUnmount()** - allows to clean up the DOM and network requests/subscriptions

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? 

- Render phase happens first.

2. What is the very first thing to happen in the lifecycle of React?

- Mounting phase occurs first. Creation of component and insertion in the DOM

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- constructor, render, react updates, componentDidMount, componentWillUnmount

4. What does componentDidMount do?

- Used to load anything using a network request or initialize the DOM; also used to set up subscriptions

# React State vs Props

1. What types of things can you pass in the props?

props = arguments to a function

- initial components; example, in a couter application, props would pass in the initial count (what the count should start at); another example is if we want something to display a title and subtitle to the user that will never change, this would be passed through the props

2. What is the big difference between props and state?

- props pass into a component and are handled/updated outside the component, state is handled inside the component and updated inside component - using the example above, state would handle/manage the counter to increase or decrease depending on user actions, while props holds the initial count that we started at which would be zero

3. When do we re-render our application?

- When the state is changed, the app is re-rendered

4. What are some examples of things that we could store in state? state stores something we're going to be updating based on what the user does; prop displays something that won't change; For example, state is useful in a form so it can be updated or changed by the user and stored


## Things I want to know more about

- structing props and state in react and practice with this