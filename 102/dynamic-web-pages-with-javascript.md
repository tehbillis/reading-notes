# Dynamic Web Pages With JavaScript

Javascript is a lightweight interpreted, or just in time (JIT), compiled language with first-class funtions. It's a language used for web & non web applications. It is a prototype-based, multi-paradigm, single threaded, dynamic language, supporting object-oriented imperative and declarative styles. It may be tempting to think Java and JavaScript are related, but they are not. The only thing they have in common is the fact that they are registered trademarks of Oracle.

JS was tlypically run on the clients machine, but lately it has been run on the server as well, with things like Node.js or io.js.

3 major parts we usually call JS are:

1. The language itself. Fairly standard on back & front end.
2. The DOM API. How JS interacts with various parts of the web page.
3. Server API, or just API. Provided by Node.js, io.js, ect.

JS can be included as a seperagte file, or embeded in the web page using `<script>` tags. `document.write();` is a simple way to write content on the page. `console.log();` is a common call used for debugging.

**Prompt** is one way to revieve input.

```html
    <script>
        var name = prompt("Your Name:", ""); // The secend set of parenthesis can be used to pre-populate the input.
        document.write("Hello ", name);
    </script>
```

The **Confirm** function is a way for the user to input true or false

```html
    <script>
        if (confirm("Print Hello?")) {
            document.write("Hello!");
        } else {
            document.write("Nevermind");
        }
    </script>
```

**Variables** are containers for storing data. There are 4 ways to declare variables:
1. Automatically
2. Using `var`
3. Using `let`
4. Using `const`

> **_NOTE_** `var` was used in all JS from 1995 to 2015. `let` and `const` were added in 2015. `var` should only be used in code for older browswers as it's not used any longer.

When to use `var`, `let`, or `const`?
* Always declare your variables.
* Always use `const` if the values shouldn't change or if the types shouldn't change. (arrays & objects)
* Only use `let` if you can't use `const`.
* only use `var` if you must support old browswers.

One thing to remember is that variables must be identified with unique names. The general rules for contructing names are:

* Names can contain letters, digits, underscores & dollar signs.
* Names must begin with a letter.
* Names can also begin with $ and _.
* Names are case sensitive.
* Reserved words (like JS keywords) can't be used as names.

**=** is the assignment operator, and **==** is the compare operator.

**=** means "This variable is".

**==** means "This variable is equal to".

## Answer

1. **What are variables in JavaScript? -** Variables are containers for storing data.
2. **What does it mean to `declare` a variable? -** To create a variable. more specifically, it tells the compiler that the variable exists, and may also have a value and data type.
3. **What is an “assignment” operator, and what does it do? -** It is a symbol that assigns a value to a variable. In JavaScript the assignment operator is the equals ( = ) symbol.
4. **What is information received from the user called? -** It is called Input. 
