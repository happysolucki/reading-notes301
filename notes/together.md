# Putting it all together

### Thinking in React

1. What is the single responsibility principle and how does it apply to components?

Essential, a component should ideally only do one thing, or have one responsibility. If a component takes on more responsibilities, they should be decomposed into smaller subcomponents.

2. What does it mean to build a 'static' version of your application?

To render your application's user interface w/o interactivity. State shouldn't be used at all.

3. Once you have a static application, what do you need to add?

Interactivity through state

4. What are the three questions you can ask to determine if something is state?

- Is it passed in from a parent via props? If so, it probably isn’t state.

- Does it remain unchanged over time? If so, it probably isn’t state.

- Can you compute it based on any other state or props in your component? If so, it isn’t state.

5. How can you identify where state needs to live?

- Identify every component that renders something based on that state.

- Find a common owner component (a single component above all the components that need the state in the hierarchy).

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

### Higher-Order Functions

1. What is a 'higher-order function'?

A function that operates on other functions, either by taking them as arguments or by returning them.

2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Using whatever value is passed as an argument to return a function that checks whether some number is greater than the value that was passed in.

3. Explain how either `map` or `reduce` operates, with regards to higher-order functions.

`map` transforms an array by applying a function to all of its elements and building a new array from the returned values.
