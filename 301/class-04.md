# React and Forms

## [How to use forms in react](https://www.robinwieruch.de/react-form/)

For acceibility reasons an HTML label can use htmlFor attribute (react specific) which links to the input id.

use `event.preventDefault()` to prevent default submit on a form.

Gain access to the HTML inputs with reacs `useRef`. The lazy way is to read them from the forms event, this is good for forms that don't need state tracking.

Using react state is the best way to manage a form with react. either by using individual handlers for each input, or by tracking the entire form if there are too many inputs. Keep in mind performance can take a hit because a rerender happens every time state is changed.

You can use an initial state object to set and reset a form easily.

A form is dirty if one of its fields has been changed by a user.

## How to use forms in react Questions

1. **What is a ‘Controlled Component’? -** A controlled component is a form component that is controlled by react.
2. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why. -** Depending on your needs, it may be best to update the sate right away so that you can perform validation on the input fields.
3. **How do we target what the user is entering if we have an event handler on an input field? -** we would use the onChange property of the input field.

## [The conditional (Ternary) operator explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

Composition of a ternary:

`condition ? value if true : value if false;`

Composition of a nested ternary:

`condition1 ? value if C1 is true : condition2 ? value if C2 is true : value if both false`

Composition of multiple operations:

`condition ? (value if true, action if true) : (value if true);`

## The conditional (Ternary) operator explained Questions

1. **Why would we use a ternary operator? -** to shorten an if statement and bring it down to a single line.
2. **Rewrite the following statement using a ternary statement:**

```javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

would be rewriten as:

```javascript
  x===y ? console.log(true) : console.log(false);
```

## Bookmark and Review

- [React Bootstrap - Forms](https://react-bootstrap.github.io/docs/forms/overview)
- [React Docs - conditional rendering](https://react.dev/learn/conditional-rendering)

## Things I Want To Know More About