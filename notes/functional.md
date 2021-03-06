# Functional Programming

### Functional Programming Concepts

1\. What is functional programming?

  It is a programming paradigm that treats computation as the evaluation of mathematical functions and values immutability

2\. What is a pure function and how do we know if something is a pure function?

  A function that:
  - returns the same result when given the same arguments
  - doesn't cause any observable side effects

3\. What are the benefits of a pure function?

  Increased testability and reliablity

4\. What is immutability?

  When the state of some data can't be changed after its creation

5\. What is Referential transparency?

  When a function consistently yields the same result when given the same input. A simple equation is this:

  pure functions + immutable data = referential transparency

## JS Modules

1\. What is a module?

  It's pretty much just code that serves a particular function. It stays in its own file so it's easier to extend to other sections of your app or to other projects entirely

2\. What does the word 'require' do?

  It allows you to import js modules

3\. How do we bring another module into the file the we are working in?

  const module = require('./path/to/module')

4\. What do we have to do to make a module available?

  export it
