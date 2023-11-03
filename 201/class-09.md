# Forms and JS Events

## HTML Forms

### First Webform

Forms are a way for users to input data that can be sent to a server or used right away to update a web page.

The `form` element formally defines a form. It is standard practice to always set the `action` and `method` attributes. Action defines the location (URL) that the forms data is sent. And method defines the way it is sent. Either `get` or `post`.

`input` and `text area` define elements that allow you to input text. They let you do it either as a single line item or as a large input box. They are usually paired with `label` elements.

Button elements are what you use to submit the form to the predefined URL. It's attribute `type` will accept 3 values.

* submit - to submit the form.
* reset - to reset the form.
* button - to do nothing! It's very useful for creating custom buttons with JS.

When submiting a form, it's important to define the `name` attribute on all the inputs so that they can be properly ahjandled on the back-end.

### How to structure a web form

`<form> ` is the top most element of a form and contains, usually, all other form elements.

`<fieldset>` groups widgets and `<legend>` is the label for it. Try building a fieldset so that when it is read by a screenreader, it flows and makes sense as naturally as possible.

`<label>` is the formal way to define a label for a widget and is used by accessibility software. You can nest a widget within the lael to associate them, but it's still best practice to set the `for` attribute.

Since forms are just HTML, you can use other HTML structures to help structure them, Like lists or divs ot sections.

## HTML Forms Questions

1. **Why are forms so important in web development? -** It's how we get data from the user to our application.
2. **When designing a form, what are some key things to keep in mind when it comes to user experience? -** It's important to make sure your widgets are labeled, and in such a way that it makes sense when reading them because if you don't, people who use screen readers and other accessibility software will have a hard time understanding your form.
3. **List 5 form elements and explain their importance. -**

1. `<form>` defines and usually contains the form itself.
2. `<input>` Allows users to input text.
3. `<fieldset>` Allows you to group widgets together, like radio buttons or checkbox's.
4. `<button>` Allows you to submit the form. Or not.
5. `<label>` Allows you to associate a variable being sent to the backend with a variable name, as well as allow the users to know what the particular input is for.

## JS Events

## JS Events Questions

1. **How would you describe events to a non-technical friend? -** An event is something that you are alerted of so that you can take the appropriate action that you want to do. Like when the low air pressure light comes on in your car, You are alerted that the tires are low on air and now you can take action to adjust their pressure to the proper levels.
2. **When using the `addEventListener()` method, what 2 arguments will you need to provide? -** You provide the event you're listening for, and the function you want to run.
3. **Describe the event object. Why is the target within the event object useful? -** The event object is special object that contains data about the event that just occured. The target is a reference to the object that called that particular event. So if a button was clicked, the target would be the button. So it's useful because you can make changes to the element that caused the event.
4. **What is the difference between event bubbling and event capturing? -**

## Things I Want To Know More About

* The event object.

