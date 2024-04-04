# table of contents
## code 301 reading notes
## Clas 09 reading notes
### Reading Class 009, 4 APR

Reading:Links to an external site.
1. What is Functional Programming?

Functional programming is a programming paradigm or style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. It emphasizes the application of functions, in contrast to the procedural programming approach, which focuses on changes in state and the sequence of actions in the program.

2. What is a Pure Function and How Do We Know If Something Is a Pure Function?

A pure function is a function where the return value is determined only by its input values, without observable side effects. This means the function always returns the same result if the same arguments are passed in. It does not depend on any state, or data, change during a program’s execution rather it only depends on its input arguments.
To determine if a function is pure, check for the following:
Given the same input, the function always returns the same output.
The function does not cause any observable side effects, such as modifying a global object or a parameter passed by reference.

3. What are the Benefits of a Pure Function?

Predictability: Since they always produce the same output for the same input, pure functions are easier to predict and test.
Reusability: Pure functions can be reused throughout the code.
Parallelizable: Pure functions can run in parallel without causing deadlocks or race conditions since they don't modify shared state.
Cacheable: The result can be cached and reused if the function is called again with the same inputs.

4. What is Immutability?

Immutability in the context of functional programming refers to the concept that data objects should not be modified after they are created. Instead of modifying an existing object, you create a new object with the changed value. This approach simplifies complex data transformations and helps to avoid side effects.

5. What is Referential Transparency?

Referential transparency is a property of expressions in programming whereby an expression can be replaced with its corresponding value without changing the program's behavior. This concept is closely related to pure functions – if a function call is referentially transparent, you can replace it with its return value without affecting the outcome of the program.


 

Video:Links to an external site.
1. What is a Module?

A module in JavaScript is a file that encapsulates code—usually functions and variables—into manageable and reusable units. Each module can export its functionalities and import functionalities from other modules. This system provides a way to organize large codebases by dividing them into smaller, more manageable and independent blocks.

2. What Does the Word ‘Require’ Do?

The term require in Node.js is used to import modules, JSON files, and local files. When you use require in your code, it reads a JavaScript file, executes the file, and then proceeds to return the exports object. This function is a part of the CommonJS module system used in Node.js.

3. How Do We Bring Another Module into the File We Are Working In?

To bring another module into the file you're working on, you can use the require function in Node.js or the import statement in ES6 (ECMAScript 6) syntax. For instance, if you have a module named exampleModule.js, you would use const example = require('./exampleModule') in Node.js, or import example from './exampleModule' in ES6, to include it in your current file.

4. What Do We Have to Do to Make a Module Available?

To make a module available to be used in other files, you need to export it. In Node.js, you can use module.exports to export functions, objects, or values from a module. In ES6, you can use the export keyword before the elements (like functions, classes, or variables) you wish to export from the module. Once exported, these can then be imported into other files as needed.

## Things I want to know more about.