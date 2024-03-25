# In Memory Storage

## [Understanding the JS call stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

JS engine is a single threaded interpreter comprising of a heap and a single call stack.

The call stack is mainly used for function invocation (call). Since the stack is single threaded, calls are processed one at a time. It operates on the LIFO principle.

Stack overflow happens when there is a refursive function with no exit.

### Call Stack Questions

1. **What is a 'call'? -** A function invocation
2. **How many 'calls' can happen at once? -** Just one
3. **What does LIFO mean? -** Last In First Out
4. **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack. -**

Empty stack -> SecondFunction() -> SecondFunction()|FirstFunction() -> SecondFunction() -> Empty Stack

```javascript 
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

5. **What causes a Stack Overflow? -** A recursive function with no exit.

## [Javascript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

Types of errors:

- Reference errors
- Syntax errors
- Range errors
- Type Errors
- [more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

`debugger;` is like adding a breakpoint in your source code.

### JS Error Messages Questions

1. **What is a ‘reference error’? -** When the item you are trying to reference doesn't exist.
2. **What is a ‘syntax error’? -** When you you incorrect syntax.
3. **What is a ‘range error’? -** When you go outside the range of a object that has a specified length.
4. **What is a ‘type error’? -** When you try to make two variable types interact with one another when they are unable to.
5. **What is a breakpoint? -** a point in your code where the debugger stops and allows you to step through your code.
6. **What does the word ‘debugger’ do in your code? -** It's like a breakpoint in your source code.

## Bookmark And Review

- [Javascript Errors Reference on MSDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

## Things I Want To Learn More About
