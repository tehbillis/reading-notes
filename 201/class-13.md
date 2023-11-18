# Local Storage

## Local Storage and How To Use It On Websites

To use local storage, all you need to do is modify the `localStorage` object in JS. This can be done directly, but is cleaner to use the `setItem()` and `getItem()` methods.

```javascript
localStorage.setItem('itemName', 'Item Contents');
```

To remove an item from storage use the `removeItem()` method.

If you only want to hold onto data while the window is ipen you can use the `sessionStorage` object instead of `localStorage`.

Local storage only stores string, it won't store objects. to get around this you can use `JSON.stringify()` and `JSON.parse()` to store and reteive an object.

You can combine all this to:

* Store web service data locally.
* Maintain the state of an interface

## Local Storage Questions

1. **Why would a developer use local storage for a web application? -** To keep track of the websites state without forcing a user to sign up and store that information on an external server.
2. **What information should not be stored in local storage? -** Sensitive and private information, or large amounts of data.
3. **Local storage can store what type of data? How would you convert it to that type before storing? -** Strings. You can use `JSON.stringify()` to convert objects into strings.

## Things I Want To Learn More About

the use cases for `sessionStorage`.