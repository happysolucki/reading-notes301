# React and Forms

1. What is a 'Controlled Component'?

An input form element whose value is controlled by the state of the component

2. Should we wait to store users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why?

Update the state with their responese as soon as they enter them. It guarantees that the displayed value will update as the user types, essential making the state the source of truth.

3. How do we target what the user is entering if we have an event handler on an input field?

event.target.value

### Ternary operator

1. Why would we use a ternary operator?

To simplify & condense conditional statements that only have one condition that determines two outcomes.

2. Rewrite the following statement using a ternary statement:

```js
if (x === y) {
  console.log(true);
} else {
  console.log(false);
}
```

```js
x === y ? console.log(true) : console.log(false);
```
