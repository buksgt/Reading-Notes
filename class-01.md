# table of contents
## code 301 reading notes
## Class 01 reading notes
### Reading Class 001, 25 Mar 

### Reading:
## READING

## Component-Based Architecture
[Learn more about Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

### 1. What is a “Component”?
A component in React is a self-contained unit that encapsulates all the logic, rendering, and behavior that might be necessary for a chunk of the user interface (UI). It acts like a JavaScript function that takes in optional inputs (called "props") and returns React elements describing how a section of the UI should appear.

### 2. What are the Characteristics of a Component?
- **Encapsulation**: Components encapsulate their behavior and rendering, providing a modular piece of the UI.
- **Reusability**: Components are designed to be reusable. The same component can be used in multiple UI areas or in different projects.
- **Isolation**: Ideally, components should be isolated and independent. This means changes in one component shouldn’t directly affect the state of another.
- **Composability**: Components can be nested within other components to build complex applications from simple building blocks.
- **Statefulness**: Components can maintain internal state data (using `useState`, `useReducer` or class state).
- **Lifecycle Management**: Class components in React have lifecycle methods that allow execution of code at particular times during the component’s life (e.g., `componentDidMount`, `componentDidUpdate`, `componentWillUnmount`).

### 3. What are the Advantages of Using Component-Based Architecture?
- **Maintainability**: Components can be individually managed and updated, which simplifies upkeep and potential upgrades.
- **Scalability**: Large applications can be built from small, manageable, reusable pieces that can be scaled up efficiently.
- **Reusability**: Components can be reused within different parts of an application or in different applications, which can significantly reduce development time.
- **Efficiency**: Components render independently only when necessary, reducing the load on the system and improving performance.

## React Props: Explanation and Overview
[What is Props and How to Use it in React](https://www.freecodecamp.org/news/how-to-use-props-in-reactjs/)

### 1. What is “Props” Short For?
"Props" in React is short for "properties". These are read-only attributes which provide data to React components.

### 2. How are Props Used in React?
Props are used in React to pass data and event handlers down to child components from a parent component. They are how components talk to each other and are mainly used for static data that doesn't change over the lifetime of the component.

### 3. What is the Flow of Props?
Props in React have a unidirectional (one-way) flow. This means data is passed from parent components down to child components through props. The unidirectional flow ensures that the data in your application is easier to track and understand. It flows down the component tree, allowing child components to receive data from their parent component, but not vice versa unless explicitly arranged (e.g., through callback functions).

This architecture helps in creating predictable and easy-to-understand code structures, which are crucial in large applications.

# Things I want to know more about.

### https://reactjs.org/tutorial/tutorial.html
### https://reactjs.org/docs/hello-world.html
### https://reactjs.org/docs/introducing-jsx.html
### https://reactjs.org/docs/rendering-elements.html
### https://reactjs.org/docs/components-and-props.html