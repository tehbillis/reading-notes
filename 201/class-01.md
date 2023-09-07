# Setting up the developer toolbelt

There will be lots of reading this first class so some things to help make the most of my time.

* Manage your reading time, this isn't an exercise in memorizing what you read.
* 15-30 minutes should be enough time to skim through the article and spend the appropriate time on the most important parts.
* Keep in mind that the ability to read and apply documentation is a core skill for developers. There’s always new technologies to learn, and you typically learn them by reading the documentation and then playing around with code samples.

## Getting Started

### How the web works

Computers that are connected to the internet are called clients and servers. Clients are typically your average user, someone who visits a website. Servers are the computers that host the websites, web apps, images, and information. Clients get websites and their information from the servers.

Other things needed in internet communication:

* An internet connection.
* TCP/IP: Transmission control protocol / Internet protocol, defines how data should travel across the internet.
* DNS: Domain Name System, like and address book for websites.
* HTTP: Hypertext Transfer Protocol, how clients and servers talk to each other.
* Component files
  * Code files: HTML, CSS, JS.
  * Assets: Images, videos, ect.

How the browser gets a web page:

1. Browser goes to DNS for site address.
2. Browser sends HTTP request to server for site files.
3. If approved, server sends "200 OK" message and site files.
4. Browser assembles the website.

Order that components are parsed:

1. HTML first.
2. CSS & JS.
3. Generate DOM, CSSOM, compile and execute JS.
4. Paint site to screen.

### Website design and process

To begin you need to answer:

* What is your website about?
* What information are you presenting?
* What will it look like, put in simple high-level terms?

Then sketch out the design, either on paper or a wireframe tool.

Choose your assets:

* Text
* Theme color
* Images
* Font

### Javascript basics

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

### Getting Started Answers

1. **Compose a short poem describing how HTTP sends data between computers. -** Consider my haiku:

    >The client requests.</br>
    >The server will then respond</br>
    >They form the world web

    Or perhaps this poem that was generated in the style of Shel Silverstein:

    >In the world of ones and zeros, oh so neat,</br>
    >HTTP dances to its web-slinging beat.</br>
    >With a click and a clack, it's on its way,</br>
    >Sharing data 'cross the digital bay.
    >
    >It's the bridge between sites, the info's guide,</br>
    >Like a digital ferry on a web-wide ride.</br>
    >From the server's den to your browser's home,</br>
    >HTTP, the web's tale, starts to roam.

2. **Describe how HTML, CSS, and JS files are “parsed” in the browser. -** The browser parses the HTML first, then it goes through it to see what CSS needs to be parsed from any `<link>` elements, then it goes and parses any Javascript from any `<script>` elements. 
3. **How can you find images to add to a Website? -** Google Images, be sure to set your search settings to open source images.
4. **How do you create a `String` vs a `Number` in JavaScript? -** A string is declared with the value wrapped in quotes such as `let string = '45'`, while a number is declared without such as `let number = 45`.
5. **What is a `Variable` and why are they important in JavaScript? -** Variables are containers that store data. They allow us to store, retrieve and manipulate data in our code.

## Introduction to HTML

### Getting started with HTML

Semantic html is a way to use your code to represent that data contained within it. It makes it easier to see what the different parts of the web page are. There are many other benefits as well such as influencing search engines, accessibility for the disabled, finding meaningful code instead of searching through endless div tags, suggesting what type of data should be there, and semantic naming mirrors proper sumo element/component naming standards.

Here are just some of the roughly 100 semantic elements available

* `<article>`
* `<aside>`
* `<details>`
* `<figcaption>`
* `<figure>`
* `<footer>`
* `<form>`
* `<header>`
* `<main>`
* `<mark>`
* `<nav>`
* `<section>`
* `<summary>`
* `<time>`

### HTML Document structure

Basic sections:

* Header
* Navigation bar
* Main content
* Sidebar
* Footer

Steps for planning a simple website.

1. Find out and write down what will be common to all pages.
2. Draw a rough sketch of how you want your pages to look.
3. Brainstorm all other (Not common to all pages) content that you want on the site.
4. Try to sort these content items into groups to see what might live together.
5. Try to sketh a rough sitemap.

### Metadata in HTML

The heads (`<head>`) content is not displayed on the webpage. Its job is to contain metadata about the document.

Metadat is data that describes data. Author and Description are very useful items to define as they can help you be found easier in web searches.

### Introduction to HTML Answers

1. **What is an HTML attribute? -** It is a selector that lets you define more details about the element.
2. **Describe the Anatomy of an HTMl element. -** you have the opening tag that defines what the element is, the content between the tags, and a closing tag.
3. **What is the Difference between `<article>` and `<section>` element tags? -** They are similar and can sometimes be used interchangeably. but an article usually groups content, while a section usually groups a standalone part of the page or components.
4. **What Elements does a “typical” website include? -**

   * Header
   * Navigation bar
   * Main content
   * Sidebar
   * Footer

5. **How does metadata influence Search Engine Optimization? -** Search engines look for certain keywords in your description and other meta elements on your page. ironically the meta keywords element that was designed for search engines is no longer used by them.
6. **How is the `<meta>` HTML tag used when specifying metadata? -** it can be used to define a variety of metadata such as `<meta name="twitter:title" content="content" />` or `<meta name="author" content="Will Green" />` or even do define character encoding for the site like `<meta charset="utf-8" />`

## Miscellaneous

### How to start designing a website

Questions to ask:

1. What exactly do I want to accomplish?
2. How will a website help me reach my goals?
3. What needs to be done, in what order, to reach my goals?

Write out your goals and prioritize them. Asking if a website can help with these goals will help you save effort by trimming goals that can't be helped by a website. Then turn each goal into actionable steps.

### Miscellaneous Answers

1. **What is the first step to designing a website? -** Define what you want to accomplish with it.
2. **What is the most important question to answer when designing a website? -** What exactly do I want to accomplish?

### Semantics

Semantics refers to the meaning of a piece of code, like what is the effect or purpose or role of this code. It helps us better understand and read our code.

HTML should be coded to represent the data it will be pupulated with, and not based on its default presentation styling. Presentation is handled by the CSS.

### Semantics Answers

1. **Why should you use an `<h1>` element over a `<span>` element to display a top level heading? -** It is more semantically correct and adds understandable structure to our code.
2. **What are the benefits of using semantic tags in our HTML? -** It helps us to better understand our code and makes it easier to read. In the case of HTML it can also boost search rankings or help screen readers.

### What is Javascript?

JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved.

### What is JS Answers

1. **Describe 2 things that *require* Javascript in the browser? -** Dynamic content, such as changing information on the page. And asynchronous content, such as retrieving or updating information in a database without reloading the web page.
2. **How can you add Javascript to an HTML document? -** Either internally or externally with the `<script>` tag.
