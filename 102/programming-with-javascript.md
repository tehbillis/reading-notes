# Programming With Javascript

**Control Flow** is the order in which the computewr executes statements in a script.

Code runs in order from top to bottom unless told otherwise by structures that change control flow, such as conditionals, loops, and functions.

### JS Functions

A JS function is a block of code designed to peform a particular task. It is executed whech "something" invokes (Calls) it.

**Syntax** 

A function is defined with the `function` keyword, followed by the __Name__ of the function, the followed by parenthesis (). Function names can contain letters, digits, underscores, and dollar signs (Same as variables). Inside the parenthesis, you can include parameter names eperated by commas. The code to be executed by the function goes between curley brackets {}.

```javascript
    function name(param1, param2) {
        //code to execute
    }
```

Function arguments are the values of the parameters, but reside inside the brackets. the arguments behave like variables.

**Function Invocation**

A function can be invoked (Called) in a few ways:

* when an event occurs.
* When called form JS Code.
* Automatically (Self invoked).

**Function Return**

When JS reaches a `return` statement, the function will stop executing. If the function was called from a statement, it will return to the statement and continue executing the code after the call. Functions will often compute a return value.

Functions allow you to "reuse" code and call it over and over again at any time. You can use it with the same or different arguments, to produce different results.

**The () Operator**

() invokes the cuntion. If you use incorrect parameters in the () it can return incorrect answers. Calling a function without () will return the entire function as it is, and not a result.

**Functions Can Be Used As Variable Values.**

**Local Variable Values**

When you define a variable inside a function, you can only access and manipulate that variable inside of that functon and nowhere else.

### JS Operators

Types of Operators:

* Arithmetic Operators - Used to perform arithmetic on numbers.
* Assignment Operators - Assigns values to variables.
* Comparison Operators - Compares things.
* String Operators - Manipulate Strings.
* Logical Operators - And, Or, Not &&, ||, !
* Bitwise Operators - Works on 32 bit numbers.
* Ternary Operators
* Type Operators - Return type, and bool to check if type.

## Answer

1. **What is `control flow`? -** Is the order in which the computer executes statements in a script.
2. **What is a JavaScript `function`? -** A block of code designed to perform a particular task.
3. **What does it mean to `invoke` - or `call` - a function? -** to execute a block of code inside that function.
4. **What are the parenthesis `()` for when you define a function? -** They let you pass parameters to the code inside the function.
