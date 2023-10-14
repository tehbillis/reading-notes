# Problem Domain, Objects, And the DOM

## Javascript

### Objects Basics

An object is a collection of related data and/or functionality. Inside these objects, variables and functions are called properties and methods.

Basic object declaration:

```javascript
const person = {};
```

And now with properties and a mothod:

```javascript
const person = {
    name: ["will", "Green"],
    age: 35,
    introduceSelf: function() {
        console.log('Hi my name is $this.name[0].');
    },
};
```

An altername way to write the method above, and a way that is much shorter, is:

```javascript
introduceSelf() {
    console.log('Hi my name is $this.name[0].');
},
```

Object literals are written out and created in the code, and are not instantiated from a class. They're good for sending structured data items so you can send one item as an object and not individual items.

Dot notation is a way to access object data and is the prefered way of doing so.

```javascript
person.age;
person.introduceSelf();
```

You can make object properties objects themselves and access those values with dot notation.

```javascript
const person = {
    name: {
        firstName: "Will",
        lastName: "Green",
    },
};

person.name.firstName;
person.name.lastName;
```

Bracket notation is another way to access object data. It can be used to create custom object members and data.

```javascript
person["age"];
person["name"]["firstName"];
```

You can set an object members value similar to how you retrieve it.

```javascript
person.age = 40;
```

The `this` keyword refers to the current object that the code is being written inside of. It makes it easy to share code among your object litterals.

You can create many objects programatically and modify each one as needed. One way to do this is by writing it as a function:

```javascript
function createPerson(name) {
    const obj = {};
    obj.name = "Will";
    obj.introduceSelf = function () {
        console.log('Hi my name is $this.name.');
    };
};
```

You can also create a constructor that will add more functionality to the creation process by automatically binding the `this` keyword to the object inside the constructor. Be sure to name your constructor with a capitol letter.

```javascript

function Person(name) {
    this.name = name;
};
```

And then to call that constructor you would use the keyword `new`.

```javascript
const will = new Person("Will");
```

### Objects Questions

1. **How would you describe an object to a non-technical friend you grew up with? -** It's a collection of related data or functionality. Like a filing cabinet. It holds lots of data and the drawers function by rolling in and out.
2. **What are some advantages to creating object literals? -** It's a nice way to pass all related data to the server in one simple to use item, rather than a bunch of items on their own.
3. **How do objects differ from arrays? -** Objects map strings to values where arrays map numbers to values.
4. **Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation. -** When creating custom object members and their values.
5. **Evaluate the code below. What does the term `this` refer to and what is the advantage to using `this`? -** It refers to the current object that the code is in. It makes it so you can reuse code among objects without tailoring that code to each individual object.

```javascript
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

### Introduction to the DOM

### DOM Questions

1. **What is the DOM? -**
2. **Briefly describe the relationship between the DOM and JavaScript. -**

## Things I Want To Know More About

* Creating custom object members programatically.