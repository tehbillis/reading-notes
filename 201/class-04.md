# Links, Layouts, and Functions

## HTML

### Creating Hyperlinks

A basic link is created by wrapping text or content in the `<a>` tag and using the `href` attribute that contains the web address.

```html
<a href="www.site.com">Go to site.com</a>
```

You can even link to a specific location in an HTML document, this is known as a _document Fragment_.

```html
<a href="www.site.com/webpage.html#elementID">Go To element with ID of X on webpage.html</a>
```

Or go to an element on the current page.

```html
<a href="#elementID">Go To element with ID of X</a>
```

### HTML Questions

1. **To create a basic link, we wrap text or other content inside what element? -** the `<a>` element.
2. **The `href` attribute contains what information? -** The location that the link points to.
3. **What are some ways we can ensure links on our pages are accessible to all readers? -** Keep the link text descriptive. Don't include URLs in the text. Minimize instances where the same text is linked to different locations.

## CSS

### CSS Layout: Normal Flow

Normal flow is the way that webpage elements lay themselves out if you haven't changed their layout.

Margin collapsing: Only relevent in the vertical direction, If 2 vertically adjacent elements both have a margin set on them and the margins touch, the larger of the two will remain and the smaller one will dissapear.

### CSS Layout: Positioning

Positioning allows you to take elements out of the normal flow and make them behave differently.

* **Static -** The default position.
* **Relative -** Similar to static, but once the element is in its place in normal flow, you can modify its position.
* **Absolute -** The element is removed entirely from the normal flow and positioned based on the containing element.
* **Fixed -** Works similar to absolute, but fixes the position to the viewport, not the containing element.
* **Sticky -** Works like a mix of `relative` and `fixed` positions. The element will behave relatively unitll its scrolled to a certain threshold, then it becomes fixed.

### CSS Questions

1. **What is meant by “normal flow”? -** Normal flow is the way that webpage elements lay themselves o9ut if you haven't changed their layout.
2. **What are a few differences between `block-level` and `inline` elements? -** Block elements expand to fill the existing space where inline only take up the space of its content.
3. **___ positioning is the default for every html element. -** Static positioning.
4. **Name a few advantages to using absolute positioning on an element. -** Good for creating unique elements that don't interfere with the flow of the rest of the page. Greate for making popups and tooltips. And is a great way to work with animations on your page.
5. **What is a key difference between fixed positioning and absolute positioning? -** The fixed position is based off of the viewport, and not the containing element.

## JS

### Functions - Reusable Blocks of Code

Functions allow you to store a piece of code that does a single task and call it whenever you want.

Functions that are part of objects are called methods.

### JS Questions

1. **Describe the difference between a function declaration and a function invocation. -** Declaring a function is what you do when a function is created. Invoking a function is what we do when we use or run the function.
2. **What is the difference between a parameter and an argument? -** A parameter is the placeholder for the argument. And the argument is the actual data that is passed along.

## Miscellaneous

### 6 Reasons for Pair Programming

**Driver** - The person who is doing the typing.

**Navigator** - Uses words to guide the driver but doesn't input anything into the computer.

Paired programming in codefellows provides:

1. Greateer efficiency.
2. Engaged collaboration.
3. Learning from your peers.
4. Social skills.
5. Job interview readiness.
6. Work environment readiness.

### Misc Questions

1. **Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey. -** 
   * Social Skills: I think the social skills gained from this will greatly help me be a better coworker and overall employee at any company. 
   * Learning From your Peers: I typically like to know the ins and outs of the tools that i'm working with, and i've found that working with others and getting their help is a great way for me to learn something fast.

## Things I Want To Learn More About

**Scrolling Index** - working with sticky positioning, look into making projects like a scrolling index.

**Anonymous Functions** - Find out more uses of the anonymous function.

**Arrow Functon** - This thing looks like it can allow you to do some awesome stuff. Get familiar with it.
