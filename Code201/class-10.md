** "Debugging is twice as hard as writing the code in the first place. Therefore, if you write the code as cleverly as possible, you are, by definition, not smart enough to debug it.
"**

-Brian Kernighan and P.J. Plauger, The Elements of Programming Style

![error](https://i.morioh.com/200721/48d32e3d.webp)

# Errors types in HTML
There are six types of errors that usually occur in JavaScript –

+ Eval Error :An error has occurred in the eval() function
+ Range Error :A number “out of range” has occurred
+ Reference Error:An illegal reference has occurred
+ Syntax Error :A syntax error has occurred
+ Type Error :A type error has occurred
+ URI Error :An error in encodeURI() has occurred

## What is an Execution Context?
An execution context is an abstract concept of an environment where the Javascript code is evaluated and executed. Whenever any code is run in JavaScript, it’s run inside an execution context.


### Types of Execution Context
There are three types of execution context in JavaScript.
+ Global Execution Context : This is the default or base execution Context
+ Functional Execution Context : Every time a function is invoked, a brand new execution context is created for that function. 
+ Eval Function Execution Context : Code executed inside an eval function also gets its own execution context.


## Execution Stack / Call Stack

A call stack is a data structure used by the JavaScript engine to manage execution contexts. The call stack uses a principle known as the LIFO (last-in-first-out) principle and whatever is at the top of the call stack will get executed first, then popped off the stack, until the stack is empty. Since the global execution context is created at the beginning of every script execution, it is placed in the call stack before any other execution context and remains at the bottom until script execution is complete
