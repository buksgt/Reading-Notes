# table of contents
## code 301 reading notes
[Class 3 Reading Notes](./class-03.md)

What does .map() return?

The .map() function in JavaScript, frequently used in React, returns a new array. Each element of this array is the result of calling a provided function on every element in the original array. Using .map() to Display Array Values in JSX:

In React, to loop through an array and display each value in JSX, you use .map().

Unique Key Requirement for List Items:

Each list item in a map operation in React should have a unique key. The key helps React identify which items have changed, are added, or are removed. Purpose of a key:

A key is a special string attribute you need to include when creating lists of elements in React. Keys give the elements a stable identity, enabling efficient update and re-render of lists. The Spread Operator in JavaScript What is the spread operator?

The spread operator (...) in JavaScript is used to expand elements of an iterable (such as an array) into individual elements, or to expand object properties. Four Uses of the Spread Operator:

Combining Arrays: Merging two or more arrays into one. Cloning Arrays and Objects: Creating a shallow copy of an array or object. Function Arguments: Passing the elements of an array as separate arguments to a function. Object Property Spread: Combining properties from multiple objects into a single object.

A. Depending on your background, you can think about splitting up a design into components in different ways:

Programming—use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents. CSS—consider what you would make class selectors for. (However, components are a bit less granular.) Design—consider how you would organize the design’s layers.

B. Which of these are state? Identify the ones that are not:

Does it remain unchanged over time? If so, it isn’t state. Is it passed in from a parent via props? If so, it isn’t state. Can you compute it based on existing state or props in your component? If so, it definitely isn’t state!

C. There are two types of “model” data in React: props and state. The two are very different:

Props are like arguments you pass to a function. They let a parent component pass data to a child component and customize its appearance. For example, a Form can pass a color prop to a Button.

State is like a component’s memory. It lets a component keep track of some information and change it in response to interactions. For example, a Button might keep track of isHovered state.

D. Props and state are different, but they work together. A parent component will often keep some information in state (so that it can change it), and pass it down to child components as their props. It’s okay if the difference still feels fuzzy on the first read. It takes a bit of practice for it to really stick!