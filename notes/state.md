## State & Props

### React Lifecycle

1. What happens first, the 'render' or the 'componentDidMount'?

Render occurs first

2. What is the very first thing to happen in the lifecycle of React?

The constructor for the component is called

3. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`.

- constructor
- render
- React Updates
- componentDidMount
- componentWillUnmount

4. What does componentDidMount do?

componentDidMount() is invoked immediately after a component is mounted, which essentially means when the component has been fully rendered in the HMTL and available to the DOM. You'd generally use this when fetching data from an external API or when there's a need to perform unique operations with jsx elements.

### Props & State

1. What types of things can you pass in as props?

Pretty anything you can pass as an argument to a function, so strings, numbers, arrays, objects, and other functions.

2. What is the big difference between props and state?

Props are handled outside of the component and must be updated outside of the component, while state is handled within the component and can be updated within the component.

3. When do we re-render our application?

When the state of the application changes

4. What are some example of things that we could store in state?

A counter or a score. A twitter post is an example. Like whether you've liked or retweeted a post. Account information could be stored in state too.
