# Functional Programming

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

Functional Programming is a **programming paradigm** that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### Pure Functions

- A function is considered pure if it returns the same result if given the same arguments (also referred as deterministic).
- It does not cause any observable side effects.

### Immutability

- Immutability and Pure Function are big advantages to build side-effect-free functions, making it easier to maintain systems.

### Impure Functions

- An example of an impure function is one that uses a global object that was not passed as a parameter to the function.

### Reading Files and Random Number Generation

- Functions that read external files or rely on a random number generator cannot be pure.

### Observable Side Effects

- Examples include modifying a global object or a parameter passed by reference.


### Functional Programming Concepts Questions

1. **What is functional programming? -**
2. **What is a pure function and how do we know if something is a pure function? -**
3. **What are the benefits of a pure function? -**
4. **What is immutability? -**
5. **What is Referential transparency? -**

## Videos - [Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

### Modules and require() Questions

1. **What is a module? -** a standalone javascript file that holds functionality, like a function, outside of the main.js file.
2. **What does the word ‘require’ do? -** it imports that module into your file.
3. **How do we bring another module into the file the we are working in? -** we set a variable equal to the required file.
4. **What do we have to do to make a module available? -** We need to export something from that module.

## Things I Would Like To Know More About
