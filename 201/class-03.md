# HTML Lists, Control Flow with JS, and the CSS Box Model

## Learn HTML

### Ordered and Unordered Lists

The `<ol>` tag represents an ordered list of items. It accepts the global attributes as well as reversed (a bool attribute, lists items high to low if true), type (sets numberting type a = lowercase letters, A = uppercase, i = lower roman numerals, I = upper roman nums, 1 = numbers (default)).

`<ol>` is used for lsits where the order is meaningful, like: 

* Steps in a recipe.
* Turn-by turn directions.

`<ul>` tag represents an unordered list. Accepts global attribs & type (circle, disc, square). Used to list items that have no particular order.

### Ordered and Unordered Lists Questions

1. **When should you use an `unordered` list in your HTML document? -** When you have a list with no particular order
2. **How do you change the `bullet style` of unordered list items? -** To make them square change the type `<ul type="square">`
3. **When should you use an `ordered list` vs an `unorder list` in your HTML document? -** When your list requres it to be in a meaningful order.
4. **Describe two ways you can change the numbers on `list items` provided by an `ordered list`? -** You can change the `type` or you can set the `reversed` attribute to true.

## Learn CSS

### The Box Model

Everything in CSS has a box around it, there are several types that can be defined as block or inline.

If a box has an outer display type of block:

* Box will break onto a new line.
* Width & height are respected.
* Padding, margin & border will push other elements away.
* If width isn't specified it will extend to fill inline space in its container. Usually filling 100% of container.

If inline then:

* Box will not break onto new line.
* Width, height will not apply.
* Top & bottom padding, margins, and borders will apply but will not push other inline boxes away.
* Left & right padding, margin, and borders will push other boxes away.

Change the inner display type by setting `display: flex`. It will still display block but all children will become flex items.

Parts of a box:

* Content box: Area where content is displayed. size with `inline-size`, `block-size`, `width`, `height`.
* Padding box: Sits around the content as white space. Size using `padding`.
* Border box: Wraps content and padding. Size using `border`.
* Margin box: Outermost layer, wrapping everything with whitespace. Size with `margin`.

### The Box Model Questions

1. **Describe the CSS properties of `margin` and `padding` as characters in a story. What is their role in a story titled: “The Box Model”? -** Marge(margin) is a client relations manager for a high profile client, she is the first point of contact and the outermost layer of the clients space. Paddy(padding) works as a bodyguard for this client, He obviously keeps the client safe. Both of their jobs is to make sure there is an appropriate amount of space surrounding their client.
2. **List and describe the four parts of an HTML elements box as referred to by the `box model`. -**
   * Content box: Area where content is displayed. size with `inline-size`, `block-size`, `width`, `height`.
   * Padding box: Sits around the content as white space. Size using `padding`.
   * Border box: Wraps content and padding. Size using `border`.
   * Margin box: Outermost layer, wrapping everything with whitespace. Size with `margin`.

## Learn JS

### Arrays. Operators and Expressions. Conditionals. Loops

#### Arrays

Arrays are usually described as list like objects

Declare an array:

```javascript
let myArray = ["Joe", "Chris", "Mel", "Hyrum"];
```

Access a value in an array:

```javascript
let myBrother = myArray[0];
```

* `.length()` - Used to find the length of an array.
* `.indexOf()` - returns the index of the passed item, or -1 if not present.
* `.push()` - Add to the end of the array.
* `.unshift()` - Add to the begining of the array.
* `.pop()` - Remove and return the last item of the array.
* `.shift()` - Remove and return the first item of the array.
* `splice()` - Pass in a specific index to remove and return that item.
* `.map()` - Allows you to do work on every item of the array. Pass in a function and it will call that function for every item in the array.
* `.filter()` - Returns only items that pass or match the test you pass in.
* `.split()` - Turns a string into an array, seperating at a specified character.
* Access all items using the `for/of` loop. `for(var of array)`.

#### Expressions and Operators

An expression is a valid unit of code that resolves to a value. Some have side effects like assigning values, and others only evaluate.

A comparison operator compares its opperands and returns a logical value based on if the comparison is true.

A bitwise operator treats their operands as a set of 32 bits.

`typeof` returns a string indicating the type of the opperand.

Relational Operators:

* `in` - returns true if the specified property is in the specified object.
* `instanceof` - returns true if the specified object is of the specified object type.

#### Conditionals

The if/else statement:

```javascript
if(condition) {
    // Code to run
} else {
    // Other code to run
}
```

The else if:

```javascript
if(condition) {
    // Code to run
} else if(otherCondition) {
    // Other code to run
} else {
    // Yet more code to run
}
```

Switch can be used in place of the if/else statement in some cases.

#### Loops

For Loop:

```javascript
for (initializer; condition; final expression) {
    // Code to run
}
```

* `break`: Exit the loop.
* `continue`: Works similar to break, but doesn't exit the loop and just goes to the next itteration.

While & do/while:

```javascript
while(condition) {
    // Code to run

    final expression;
}
```

The while loop has the chance to never run because it checks a condition before it executes any code.

```javascript
do{
    // Code to run

    final expression;
} while(condition)
```

the do/while loop will always run at least once becuase it checks its condition at the very end.

### Arrays. Operators and Expressions. Conditionals. Loops Questions

1. **What `data types` can you store inside of an `array`? -** Strings, numbers, objects and even other arrays.
2. **Is the `people` array a valid javascript array? If so, how can I access the values stored? If not, why? -** It is! you can access it like so `let person = people[0][1]` to get Petes name.

```javascript
const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

3. **List five shorthand operators for assignment in javascript and describe what they do. -**
   * `=` simply assigns a value.
   * `+=` adds a value.
   * `/=` divides a value.
   * `%=` divides evenly, then assigns the remainder.
   * `-=` subtracts a value.

4. **Read the code below and evaluate the last expression and explain what the result would be and why. -** The result would be "10dog". We first do the work inside the parenthesis, we add 10 to false. Since false evaluates to 0, our math looks like 10+0 which leaves us with 10. Then you add dog to the end of that, and we are left with "10dog".

```javascript
let a = 10;
let b = 'dog';
let c = false;

// evaluate this
(a + c) + b;
```

5. **Describe a real world example of when a conditional statement should be used in a JavaScript program. -** When you have a multiple choice question and need to display or record if the answer is correct or not, you can use a conditional statement to see if the answer is correct, then log it accordingly.

6. **Give an example of when a Loop is useful in JavaScript. -** A loop is useful when you need to do a specific set of actions multiple times, like looping through an array and displaying the items in a list.
