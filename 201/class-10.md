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

The debugger is a tool that allows you to watch the values of your variables as well as pause your code and step through it to see what it's doing. Pausing your code is called setting a breakpoint, a place for your code to stop so you can watch it step by step.

The browser also offers you a developer console that lets you see output of your code that is logged to the console and execute code within the console.

The call stack is a place where you can see all the code that was executed to get to the line of code you are on. It's helpful so you can trace the patch of your logic.

And scopes shows you the values of variables available to you in the code.

## JS Debugger Questions

1. **How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development? -** The debugger is a tool that lets you watch the values of your variables as well as pause your code so you can see what it's doing. This all helps to see where your code is having problems.
2. **Define what a breakpoint is. -** It's a place where you can pause your code and then walk through it step by step to see what's going on.
3. **What is the call stack? -** A section that shows you all the code that was executed up to the line of code you are on now.

## Things I Want To Know More About
