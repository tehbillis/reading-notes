# Object-Oriented Programming, HTML Tables

## Domain Modeling

DOmain modeling is the process of creating a conceptual model in code for a specific problem. That model can define various attributes, behaviors or constraints.

A prototype can be imagined as if it were a bus, lots of people (Objects) can use this bus (Prototype methods/properties) without taking up space and resources at their own home. This is a great way to give everyone access to the same resource while not using too many resources all at once. So it's a good thing to do especially when targeting devices such as mobile that don't have many resources to begin with.

## Domain Modeling Questions

1. **Explain why we need domain modeling. -** In very simple terms it helps us understand the problem we are working with, and our solution to that problem.

## HTML Table Basics

A table is a structured set of data made up of rows and columns. The point of a table is to be rigid and uniform, so that data can be consumed easily.

## HTML Table Questions

1. **Why should tables not be used for page layouts? -** Tables are rigid and fairly inflexible, they reduce accessibility, and they create tag soup.
2. **List and describe 3 different semantic HTML elements used in an HTML `<table>`. -** `<tr>` is the row of the table, `<th>` is a table header usually used to describe the column or row, and `<td>` is the data displayed within the table.

## Constructors

A constructor is just a function called using the `new` keyword. Doing this will:

1. Create a new object.
2. Bind the keywork `this` to that new object.
3. Runs the code inside the constructor.
4. Returns the new object.

Constructors make it easy to modify existing objects and is the best way to create many of the same object type.

You can also create a constructor that will add more functionality to the creation process by automatically binding the this keyword to the object inside the constructor. Be sure to name your constructor with a capitol letter.

```javascript
function Person(name) {
    this.name = name;
};
```

And then to call that constructor you would use the keyword new.

```javascript
const will = new Person("Will");
```

## Constructors Questions

1. **What is a constructor and what are some advantages to using it? -** A constructor is just a function that is called with the `new` keyword. It makes it easy to create a lot of objects of that are the same and allows you to easily modify those objects in one place rather than each individual object.
2. **How does the term `this` differ when used in an object literal versus when used in a constructor? -** In an object literal, `this` refers to the the object that it is within. While in a constructor, `this` refers to the object that will be created and will only be available if the object was created with the `new` keyword. so, one is in the present tense and the other is in the future tense.

## Object Prototypes Using A Constructor

When an object is crated from another object, and there is a failed property lookup on the child, JavaScript will delegate that lookup to the parent object that it was created from. In this way, the child object inherits these properties from its parent object.

Every object in javascript has a prototype that references an object.

Javascript allows for the use of classes to create object. It keeps everything related to our object in one nice tidy package.

A helper method, is a method that needs to be used by a cerain object, but not all objects of that type. So you add the method to the class as a static method. Now it can be accessed via `Class.method();` instead of `object.method();`.

`object instanceof Class` will return true or false.

Arrow functions don't have their own `this` keyword. So they can't be used as a constructor function. Arrow functions also don't have a prototype property.

## Object Prototypes Questions

1. **Explain prototypes and inheritance via an analogy from your previous work experience. -** Let's imagine a cheese pizza is our pizza `prototype`. It has properties such as `crust`, `sauce`, `topping`. Now let's imagine we have other types of pizza's, like hawaiian, or meat lovers, or BBQ chicken. all these pizza's inherit the basic properties of a pizza, and then they add their own specialized properties such as different toppings.

## Things I want to know more about

1. Javascript Classes
2. Arrow Functions
