# table of contents
## code 301 reading notes
## Class 04 reading notes
### Reading Class 004, 28 Mar 

### Reading:
## How to Use Forms in React

### 1. What is a ‘Controlled Component’?
A controlled component in React is an input element (like a form input) where the value of the input is controlled by the state of the component. This means that every change to the input updates the state, and the value of the input is always synchronized with the state.

### 2. Should we update the state with users' responses as soon as they enter them or wait until they submit the form? Why?
We should update the state with users' responses as soon as they enter them. This is because it allows the component to maintain control over the input's values, which is necessary for validating, manipulating, or using the data dynamically while the user is still filling out the form.

### 3. How do we target what the user is entering if we have an event handler on an input field?
To target what the user is entering in an input field with an event handler, use the `event.target.value` property within the event handler function. This property will give you access to the current value of the input field after every keystroke.

## The Conditional (Ternary) Operator Explained

### 1. Why would we use a ternary operator?
We use a ternary operator as a shorthand for the if-else statement when we want to make code more compact. It is typically used to assign a value to a variable based on a condition, or to execute one of two expressions.

### 2. Rewrite the following statement using a ternary statement:
**Original statement:**

### if(x === y){
###  console.log(true);
### } else {
###  console.log(false);
### }

### Ternary statement version:

### console.log(x === y ? true : false);

# Things I want to know more about.

### https://react-bootstrap.github.io/docs/forms/overview
### https://react.dev/learn/conditional-rendering