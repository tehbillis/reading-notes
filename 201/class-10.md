# Debugging and Error Handling

## Troubleshooting Javascript

Usually there are two types of errors that you will run into.

1. Syntax Errors - Spelling mistakes in the code.
2. Logic Errors - Your code not working as you intended.

The developer console in the browser will inform you of syntax errors and where they are in your code.

Using `console.log()` can be a valuable tool when trying to debug your code.

Some common mistakes to watch out for:

* Missing semi-colon.
* Improper value assignment. Like using `=` when you meant to use `===`.
* Parenthesis, either too many or too few.

## Troubleshooting Questions

1. **Name some key differences between a `Syntax Error` and a `Logic Error`. -** Syntax Error is an issue with the way your code is written. like a missing semi-colon. A logic error is a problem with the way that your code operates. Like an infinite loop.
2. **List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them. -** When looping through an array that was initialized without a value, it would return an error saying it wasn't defined instead of the expected number value. So after some testing a few different console logs and tweaks to some pieces of the code, i found out that i needed to initialize the array with empty quotes, so that it began with something, even if it was an empty value.
3. **How will this topic continue to influence your long term goals? -** Error handling is something I use every time I write code. I think i've only once written code that didn't throw an error, and that was long ago. This is a tool that I will carry with me allways.

## The Javascript Debugger

## JS Debugger Questions

1. **How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development? -**
2. **Define what a breakpoint is. -**
3. **What is the call stack? -**