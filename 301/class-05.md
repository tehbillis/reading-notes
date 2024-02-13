# Putting it all together

## [Thinking in react](https://reactjs.org/docs/thinking-in-react.html)

The 5 steps to impliment UI in react:

1. Break the UI into a compoenent heirarchy.
   - Layout which components will contain which other components.
   - Keep the single responsibility principle in mind.
2. Build a static version in react.
   - Build out your application with no functionality.
   - Look at your data, it is layout out and flows much like how the UI will be layed out and flow.
3. Find the minimal but complete representation of UI state.
   - Figure out what is going to be held in a state variable by following the 3 questions.
     - Does it remain unchanged?
     - Is it passed via props?
     - Can you compute it based on existing state or props?
   - If no to these questions, then it's probably state.  
4. Identify where your state should live.
   - Find all components that use the state and place it in their most common parent, or somewhere in the heirarchy above that parent.
5. Add inverse data flow.
   - With data flowing from parent to child, add routes for data to flow from child to parent. perhaps by passing functions to components.

## thinking in react Questions

1. **What is the `single responsibility principle` and how does it apply to components? -** It's the idea that something should really only do one thing. and if it grows beyond that, it should be decomposed into smaller subcomponents. This idea can be applied to react components, they should only really do one thing.
2. **What does it mean to build a ‘static’ version of your application? -** A static version is just the basic representation of your application, it has no functionality.
3. **Once you have a static application, what do you need to add? -** State and functionality
4. **What are the three questions you can ask to determine if something is state? -** does it remain unchanged? is it passed in via props? can you compute it based on  existing state or props? if no to these, then it's probably best to  use state.
5. **How can you identify where state needs to live? -** Identify all the components that use the state, and if multiple compenents use it, then place it in their most recent common parent. Sometimes you can put it in a component above their common parent. If you can't find a suitable component, then create one above their comon parent.

## [Higher-Order functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

Functions that operate on other functions, either by taking them as argument or by returning them, are higher order functions.

## Higher-Order functions Questions

1. **What is a “higher-order function”? -** It's a function that operates on other functions.
2. **Explore the `greaterThan` function as defined in the reading. In your own words, what is line 2 of this function doing? -** the function is taking in the argument passed to the graterthan10 function and assigning it to m, and since the greaterthan10 function was initialized before, n has been assigned the value of 10. This function takes those two variables and checks if `m` is greater than 10.
3. **Explain how either `map` or `reduce` operates, with regards to higher-order functions. -** They both work as higher order functions by taking another function as an argument.

## Things I Want To Know More About

- the concept of Closure in javascript.