## Understanding the JavaScript Call Stack
1. What is a ‘call’?

`primarily used for function invocation (call)`

2. How many ‘calls’ can happen at once?

`one at a time`

3. What does LIFO mean?

`Last In, First Out `

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();

```

4. What causes a Stack Overflow?

` occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.`

## JavaScript error messages

1. What is a ‘refrence error’?

` when you try to use a variable that is not yet declared`

2. What is a ‘syntax error’?

`when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse`

3. What is a ‘range error’?

`when you try to manipulate an object with some kind of length and give it an invalid length`

4. What is a ‘tyep error’?

`when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable`

5. What is a breakpoint?

`when you  put a debugger statement in your code in the line you want to break.`

6. What does the word ‘debugger’ do in your code?

`the process of detecting and removing of existing and potential errors`
