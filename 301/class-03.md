# Passing Functions As Props

## Lists and Keys

React requires you to use a key with your list so that it knows what's going on with the element if you update, remove, or move it.

## List and Keys Questions

1. **What does .map() return? -** Typically a copy/modified array of the original array.
2. **If I want to loop through an array and display each value in JSX, how do I do that in React? -** You could use the .map() function to return <li> and then display them in a list.
3. **Each list item needs a unique ____. -** Key.
4. **What is the purpose of a key? -** So react can keep track of the element.

## The Spread Operator

`...` can be used to expand an iterable object or variable into individual items.

Only iterable values like array or string can be spread in array litterals & argument lists. But arrays can be spread in object litterals & enumerates. Spreading in object litterals will turn them into propertires. NOTE that all primitives can be spread into object litterals, but only iterable items will create properties.

When calling a constructor with `new` you can populate the properties with spread.

Can be used to copy a simple array, but isn't suitable to copy a multidimensional array.

Can be a great way to concat arrays. .This can also be done conditionally.

## Spread Operator Questions

1. **What is the spread operator? -** A way to expand iterable items, represented with `...`
2. **List 4 things that the spread operator can do. -** it can make a copy of a simple array, populate an object literal, concat arrays, and pass arguments into functions.
3. **Give an example of using the spread operator to combine two arrays. -** 

```javascript
  let array1 = ['a', 'b', 'c'];
  let array2 = ['d', 'e', 'f'];

  let array = [...array1, ...array2];
  
  // array1 now Returns ['a', 'b', 'c', 'd', 'e', 'f']
```

4. **Give an example of using the spread operator to add a new item to an array. -** You could do it conditionally:

```javascript
  const condition = true;

  const array = [1, 2, ...(condition ? [3] : [])];

  // Since the condition is true, array would return [1, 2, 3]
```

5. **Give an example of using the spread operator to combine two objects into one. -**

```javascript
  const obj1 = { minutes: 30, seconds: 2 };
  const obj2 = { month: "Feb", days: 3, hours: 9 };

  const mergedDate = { ...obj2, ...obj1 };

  // mergedDate returns { month: "Feb", days: 3, hours: 9, minutes: 30, seconds: 2 }
```

## How to Pass Functions Between Components

## Pass Functions Questions

1. **In the video, what is the first step that the developer does to pass functions between components? -** This seems like a trick question, it's either to create a parent component and child component, or create the function in the parent component.
2. **In your own words, what does the `handleClick` function do? -** It informs you that the function has been called, since we called it from the child, it really tells us when the button in the child componenet is clicked. And really, this can be called from any child within the parent as long as the function is passed through the props.
3. **How can you pass a method from a parent component into a child component? -** You can pass it as a prop.
4. **How does the child component invoke a method that was passed to it from a parent component? -** from the props that have been passed to it, in the `handleClick` instance we saw, it was invoked in the buttons `onClick` event.

## Bookmark and Review

- [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

## Things I Want To Know More About
