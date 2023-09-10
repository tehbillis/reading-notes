# Basics of HTML, CSS & JS

## Introduction to HTML

### HTML Text Fundamentals

There are 6 levels to headings, from `<h1>` to `<h6>`. It's important to try to only have a single `<h1>` per page.

Adding structure is important so our content is easily readable and accessible. It can also allow us to make our content interactive.

Semantic elements give meaning, function, or appearance to our code.

Lists come in 2 types. Ordered lists:

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
```

And Unordered lists:

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>
```

You can also nest your lists!

```html
<ol>
    <li>Item 1</li>
    <li>Item 2
        <ul>
            <li>nested 1</li>
            <li>nested 2</li>
        </ul>
    </li>
    <li> Item 3</li>
</ol>
```

You can give meaning to your text with emphasis tags such as `<strong>`. You can also Bold `<b>`, Underline `<u>` or Italicise `<i>` your text.

### HTML Advanted Text Formatting

There is actually a third type of list. A description list. You can even have multiple descriptions per term if you wish.

```html
<dl>
    <dt>Description term 1</dt>
    <dd>Description definition 1</dd>

    <dt>Description term 2</dt>
    <dd>Description definition 2</dd>
</dl>
```

You can wrap info in a `<blockquote>` tag to indicate that it is a quote & apply default style to it. You can inline a quote with the `<q>` tag when you don't need paragraph breaks. Browswers don't really do much the the `cite` attribute.

Use the `<abbr>` tag to add contexgt to an abbreviation. Fill out the `title` attribute for its meaning.

You can add contacg information with the `<address>` tag. Try not to use it in a list of addresses and keep it relevent to the page or site.

Superscript `<sup>` and subscript `<sub>` tags are useful when marking up dates, math equations, or chemical formulas.

Some tags for marking up code are `<code>` for generic code, `<pre>` for retaining white space in large code blocks, `<var>` for variable names, `<kbd>` for keyboard input, and `<samp>` for computer program output.

Use the `<time>` tag to markup times and dates.

### Introduction to HTML Answers

1. **Why is it important to use semantic elements in our HTML? -** It gives meaning, functon, or appearance to our code.
2. **How many levels of headings are there in HTML? -** 6
3. **What are some uses for the `<sup>` and `<sub>` elements? -** For marking up dates, math equations, or chemical formulas.
4. **When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term? -** the `title` attribute.

## Learn CSS

### How CSS Is Structured

Apply CSS three ways. With External stylesheets, internal stylesheets, and inline styles. Using inline styles should be avoided as it's the oposite of best practice. Inline styles are hard to maintain and makes code difficult to read.

A selector defines what the style will be applied to. Properties are the specific style that is being applied. When a property is paired with a value it is called a declaration.

Some values can be functions, like the `calc()` function as well as certain values for the `transform` property.

Some properties are called shorthand properties because they have several values in a single line.

CSS comments begin with `/*` and end with `*/`

### Learn CSS Answers

1. **What are ways we can apply CSS to our HTML? -** With an external stylesheet, and internal stylesheet, or with inline styles.
2. **Why should we avoid using inline styles? -** It's the oposite of best practice. It's hard to maintain and makes code hard to read.
3. **Review the block of code below and answer the following questions:**
   1. **What is representing the selector? -** the `h2`
   2. **Which components are the CSS declarations? -** Both lines inside the curley brackets. They are properties paired with values.
   3. **Which components are considered properties? -** `color` and `padding`

```css
  h2 {
     color: black;
     padding: 5px;
   }
```

## Learn JS

### JS Basics

Javascript comments can be implemented two different ways. `// comments out a line of code` where `/* will comment everything enclosed within */`.

An operator is a mathematical symbol that produces a result based on two values (variables).

Conditionals are code structures used to test if an expression returns true or not.

Functions are a way of packaging functionality that you wish to reuse.

Events are code strucures that listen for activity in the browswer, then run code in response.

### JS Basics Answers

1. **What data type is a sequence of text enclosed in single quote marks? -** A String
2. **List 4 types of Javascript operators. -** +, -, !, ===.
3. **Describe a real world problem you could solve with a function. -** You could use a function to calculate employee payroll by taking in variables such as employee pay, hours worked, and maybe their taxes and benefits to be deducted.

### Making decisions in your code - Conditionals

if/else statements will probably be the most used conditional statment used in JS. The basic syntax is:

```javascript
if (condition) {
    //Run if true.
} else {
    //Run other code
}
```

You can also make multiple checks with the `elseif` statement.

```javascript
if (condition) {
    //Run if true.
} elseif (condition) {
    //Run if first condition false and this condition true.
} else {
    //Run other code.
}
```
&&, ||, ! are very important logical operators. 
* && - All conditions must be true for conditional to evaluate to true.
* || - Only one condition must be true for conditional to evaluate to true.
* ! - inverts the logic of the condition, Makes a `true` condition evaluate to false and a `false` condition evaluate to true.

Switch statements can be a better option than if/else statements if you have a lot of cases or want to print out very specific things.

```javascript
switch (expression) {
  case choice1:
    // run this code
    break;

  case choice2:
    // run this code instead
    break;

  // include as many cases as you like

  default:
    // actually, just run this code
    break;
}
```

The ternary operator is a small bit of syntax that tests a condition and returns one value/expression if it is true, and another if it's false.

```
Condition ? run this code : run this code instead;
```

### Conditionals Answers

1. **An if statement checks a __ and if it evaluates to ___, then the code block will execute. -** Condition, True.
2. **What is the use of an `else if`? -** To make multiple checks in your if statement.
3. **List 3 different types of comparison operators. -** `>`, `==`, `!=`.
4. **What is the difference between the logical operator `&&` and `||`? -** `&&` requires all statements to be true while `||` only requires one of the satements to be true.

## Things I want to know more about

I didn't know about the `===` operator, so I would like to learn more about all the other kinds of operators.

Ternary operator looks really cool, look more into how to properly use this.