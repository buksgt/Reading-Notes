# table of contents
## code 301 reading notes
## Class 05 reading notes
### Reading Class 005, 29 Mar 

## Reading:
## React Documentation: Thinking in React: https://reactjs.org/docs/thinking-in-react.html

The React documentation, particularly the section on "Thinking in React," covers several important concepts in React development.

### Single Responsibility Principle and Components

The single responsibility principle is a programming concept that suggests a class or a module should have one, and only one, reason to change. This means each component should ideally do only one thing.

### Building a 'Static' Version of Your Application

In React, building a static version means creating a version of your app that renders your data model but has no interactivity.

### Adding to a Static Application

Once you have a static application, the next step is to make it interactive. This involves figuring out the smallest amount of changeable information your app requires, setting up rules for how this information changes.

### Determining if Something is State

To determine if something is state, you can ask three questions:

- Is it passed in from a parent via props? If so, it probably isn’t state.
- Does it remain unchanged over time? If so, it likely isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state.

### Identifying Where State Needs to Live

- Identify every component that renders something based on that state.
- Find a single, shared part in your app (component) that sits above all the parts that need to use the same information.
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component of your app that fits to hold the information, make a new part just for that purpose and place it higher up in the structure.

## Higher-Order Functions: https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK

A higher-order function is a function that either takes one or more functions as arguments or returns a function.

### The greaterThan Function

Compare a given value with another value and return a boolean result. If it's a higher-order function, line 2 might be defining a new function based on a passed-in threshold.

### Map or Reduce in Relation to Higher-Order Functions

- **map**: This transforms an array by applying a function to each element of the array without changing the original array. It returns a new array consisting of the results of applying the function to each element.
- **reduce**: This is a higher-order function that reduces an array to a single value. It applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value. This is often used for summing up values, combining arrays, etc.

# Things I want to know more about.