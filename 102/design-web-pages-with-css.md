# Design Web Pages With CSS

What is Css? Css is a language for specifying how documents are presented to users. such as their styles and how they're laid out.

> **_NOTE:_**  User Agent typically means the web browser.

### Css Syntax

```css
    h1 {
        color: red;
        padding: 10px;
    }
```

The h1 would be what's known as the selector. It could just as well be a class, or element ID. What resides within the brackets are the declarations.

A few good things to keep note of:

* CSS properties have different allowable values depending on what property you are working with.
* CSS is grouped into different modules so that information is easier to locate.
* CSS Specs are what browsers use to interpret CSS, it's not something that devs truly need to know.
* Not all browsers support all CSS properties, it's a good idea to know what browser supports what you want to use.

### Adding CSS

There are 3 ways to add css to your project.

1. External CSS
2. Internal CSS
3. Inline CSS

**External** CSS are styles that live in an external document seperate from the HTML called a style sheet. You include these style sheets in the `<head>` section of your HTML page in a `<link>` element.

**Internal CSS** styles are saved in the `<style>` element in the `<head>` section of the HTML page. These are styles that would be unique to that specific page.

**Inline CSS** are styles that are unique to an individual element on the page. They are applied to the style attribute of the element.

**Cascading Order** defines which styles are applied to the element, and what styles are not. In order of greatest priority they are:

1. Inline Styles, applied over all others.
2. External and Internal styles, applied if there are no inline styles.
3. Browser defualts, applied if no style is defined.

### Multiple Style Sheets

If more than one style sheet defines the same selector, the value from the last read style sheet will be used.

**_Example 1_**

```html
    <head>
        <link rel="stylesheet" href="mystyle.css">
        <style>
            p {
                color: blue;
            }
        </style>
    </head>
```

In this example the color blue from the `<style>` element will be applied because it was the last one to be read.

**_Example 2_**

```html
    <head>
        <style>
            p {
                color: cerulean;
            }
        </style>
        <link rel="stylesheet" href="mystyle.css">
    </head>
```

In this example the style from the `<link>` element will be applied because it was the last one to be read.

### CSS Color

> **_NOTE_** The color property defines the color of text.

Examples of css color:

```css
    color: red;
    color: #00ff00;
    color: rgb(0, 0, 255);
    color: rgba(201, 76, 76, 0.6);
    color: hsl(89, 43%, 51%);
    color: hsla(89, 43%, 51%, 0.6);
```

## Answer

1. **What is the purpose of CSS? -** It is how we specify how documents are presented to the user, like how they're styled and laid out.
2. **What are the three ways to insert CSS into your project? -**
   * Externaly
   * Internaly
   * Inline
3. **Write an example of a CSS rule that would give all `<p>` elements red text. -**

```css
p { 
    color: red; 
}
```
