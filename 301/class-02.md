# State and Props

## React Lifecycle

The 3 phases of component lifecycle are mounting, updating, and unmounting.

Avoid calling this.setSate() in the constructor. it can cause strange behavior and errors.

Using setState() in componentDidRender will work, but causes a render and can cause performance issues.

## React Lifecycle Questions

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? -** the `render` happens first.
2. **What is the very first thing to happen in the lifecycle of React? -** The `constructor`.
3. **Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`. -** constructor, render, react updates, componentDidMount, componentWillUnmount.
4. **What does `componentDidMount` do? -** is invoked right after a component is mounted and lets you make a network request to load data or allows you to initialize the DOM.

## React State vs Props

State an be changed inside components. Props are only passed to the component and can't be changed.

## State vs Props Questions

1. **What types of things can you pass in the props? -** strings, numbers, Data in general.
2. **What is the big difference between props and state? -** A Component can't modify its props, but can modify state.
3. **When do we re-render our application? -** whenever state is changed
4. **What are some examples of things that we could store in state? -** current count, form data.

## Bookmark and Review

- [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
- [React Docs - Handling Events](https://reactjs.org/docs/handling-events.html)
- [React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)
- [React Bootstrap Documentation](https://react-bootstrap.github.io/)
- [Bootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
- [Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)
- [Netlify](https://www.netlify.com/)

## Things I Want To Know More About

