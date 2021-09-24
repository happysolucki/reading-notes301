# Passing Functions as Props

### Lists and Keys

1. What does .map() return?

A new array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

```jsx
const nums = [7, 14, 21, 28, 35];
const headerItems = nums.map((num) => <h2>{num}</h2>);
ReactDOM.render(
  <div>{headerItems}</div>,
  document.getElementById('root')
);
```

3. Each list iten needs a unique ___.

key

4. What is the purpose of a key?

To specify to React which component it should re-render.

### Spread Operator

1. What is the spread operator?

An operator that allow one to add items to array, combine arrays or objects, and spread an array out into a function's arguments.

2. List 4 things that the spread operator can do.

- Concatenate or combine arrays
- Use array as arguments
- Add item to a list
- Add to state in react

3. Give an example of using the spread operator to combine two arrays.

```js
const nums1 = [1,2,3,4];
const nums2 = [5,6,7,8,9];
const numArr = [...nums1, ...nums2];
```

4. Give an example of using the spread operator to add a new item to an array.

```js
const names = ['John', 'Bradley', 'Kelly'];
const name = 'Thomas';
names = [...names, name];
```

5. Give an example of using the spread operator to combine two objects into one.

```js
const person = {
  firstName: 'Kevin',
  lastName: 'Mitchell'
};
const grade = { score: 100 };
const student = { ...person, ...grade };
```

### Passing functions between components

1. In the video, what is the first step that the developer does to pass functions between components?

Pass it to a component like you would any other prop

2. In your own words, what does the increment function do?

It takes in a name as an argument. It maps through the people array that's saved in state and checks to see if the name passed in matches the name of any of the objects in the array. If there's a match, increment that object's count by 1. The state of the people array is then updated with this newly created one.

3. How can you pass a method from a parent component into a child component?

Pass it like you would any other prop. If you wanted to pass a function named `handleClick` to a `Car` component, it'd look something like this:

```jsx
// functional and class component
<Car handleClick={handleClick}>;
<Car handleClick={this.handleClick}>
```

4. How does the child component invoke a method that was passed to it from a parent component?

Carrying on from the previous example, you'd do this:

```jsx
// functional and class component
<Car onClick={props.handleClick}>
<Car onClick={this.props.handleClick}>
```
