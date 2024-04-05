# table of contents
## code 301 reading notes
## Class 10 reading notes
### Reading Class 010, 5 APR

Understanding the JavaScript Call StackLinks to an external site.

 

What is a call?

A ‘call’ in JavaScript refers to the invocation of a function.

 

How many "calls" can happen at once?

In the JavaScript call stack, only one call can happen at a time because it's single-threaded.

 

What does 'LIFO' mean?

LIFO stands for Last In, First Out. It's a principle where the last function that gets pushed into the stack is the first one to be popped out when it returns.

 

Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

Function A is invoked.
Inside Function A, Function B is invoked.
Inside Function B, Function C is invoked.
The call stack will have C at the top, then B, and A at the bottom.

What causes a Stack Overflow?

A Stack Overflow is caused by a recursive function (a function that calls itself) without an exit point, leading to an infinite loop of calls.

 

JavaScript error messagesLinks to an external site.

 

What is a "reference error"?

A 'Reference Error' occurs in JavaScript when trying to use a variable that has not been declared or is not within the current scope.

 

What is a "Syntax Error"

A 'Syntax Error' is an error in the syntax of a programming code. It happens when the rules of the programming language are not followed.

 

What is a "Range Error"

A 'Range Error' occurs when a numerical value is outside the allowed range.

 

What is a "Type Error"?

A 'Type Error' happens when an operation is performed on a variable that is not of the expected type, like trying to call something that's not a function.

 

What is a "breakpoint"?

A breakpoint is a tool used in debugging. It is a marked location in the code where the debugger will pause the execution of the program, allowing the developer to inspect the state of the application at that point.


What does the word "debugger" do in your code?

The word 'debugger', when used in code, is a statement that invokes any available debugging functionality, such as setting a breakpoint.

## Things I want to know more about.