# table of contents
## code 301 reading notes
## Class 02 reading notes
### Reading Class 002, 26 Mar 

### Reading: [React Component Lifecycle Events](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. **What happens first, the `render` or the `componentDidMount`?**
   - The `render` method happens first. After rendering is complete, `componentDidMount` is called.

2. **What is the very first thing to happen in the lifecycle of React?**
   - The very first thing is the execution of the `constructor` of the component class, where you can set up state and bind methods.

3. **Order of events: componentDidMount, render, constructor, componentWillUnmount, React Updates**
   - **Constructor**
   - **Render**
   - **ComponentDidMount**
   - **React Updates** (when state or props change, leading to re-rendering)
   - **ComponentWillUnmount**

4. **What does componentDidMount do?**
   - `componentDidMount` is used for actions that need to occur after the component is initially rendered and displayed on the screen, such as API calls, subscriptions, or generally setting up any long-running processes.

### Videos: [YouTube](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. **What types of things can you pass in the props?**
   - You can pass a variety of data types through props, including numbers, strings, functions, objects, arrays, and even JSX elements.

2. **What is the big difference between props and state?**
   - **Props** are read-only and passed from parent to child components, used to configure a component.
   - **State** is managed within the component and can be changed. State allows React components to create and manage their own data.

3. **When do we re-render our application?**
   - A React application re-renders whenever there is a change in its state or props.

4. **What are some examples of things that we could store in state?**
   - Examples include:
     - User input data 
     - Data fetched from an API
     - Interaction states 
     - UI state changes

# Things I want to know more about.

### https://reactjs.org/docs/state-and-lifecycle.html
### https://reactjs.org/docs/handling-events.html
### https://reactjs.org/tutorial/tutorial.html
### https://react-bootstrap.github.io/
### https://getbootstrap.com/docs/5.0/examples/cheatsheet/
### https://bootstrapshuffle.com/classes
### https://www.netlify.com/