# CSS Layout

## Flexbox

The flexbox layout model is a layout model designed for one dimenstional content. Picture a plot graph with an x and y axis. Flexbox models data that is layout on on a single axis, so either up and down or left and right. but not both.

Your main axis is the one set by your `flex-direction` property. Either `row` or `column` can be applied. the cross axis runs oposite of your main axis.

Flexbox initial values:

* items display as a row.
* They do not wrap.
* They do not grow to fill the container.
* They line up at the start of the container.

`flex-direction` properties:

* row
* row-reverse
* column
* column-reverse

`flex-flow` is shorthand to control direction and wrap in one property. `flex-flow: column wrap;`

Control space inside flex items with `flex-grow`, `flex-shrink`, and `flex-basis`. The shorthand property for this is just `flex` and the key values are `initial`, `auto`, and `1`.

In flexbox alignment you have properties that distriburte space: `justify-content`, `align-content`, and `place-content`. You also have properties for alignment: `align-self`, and `align-items`. `justify-` works on the main axis while `align-` works on the cross axis.

To distribute space along the main axis, use the `justify-content` property on the flex container. For this to work on items set to `column`, you need to give the container a `height` or `block-size`. Use `align-content` to distribute space on the cross axis. The shorthand property for this is `place-content` with one or two values, a single value will apply to both the main and cross axis.

To align items on the cross axis use `align-items` and `align-self`.

## Flexbox Questions

1. **Flexbox is designed for one-dimensional content. Explain what this means. -** Imagine a plot graph that has an x and y axis. flexbox is designed for data that flows along one of those two axis'. Either up and down, or left and right. because of this, you can't control if things line up exactly in all 4 directions.
2. **Explain the difference between the main axis and cross axis. -** Your main axis is set by the `flex-direction` property. The cross axis runs oposite of whatever that property is set to.
3. **How can using certain properties of flexbox negatively impact accessibility? -** Reordering things only happens on a visual level, not a logical level, so accessibility features may not match what is displayed.

## Flexbox Layout

## Flexbox Layout Questions

1. **What are some advantages to using flexbox over float? -**
2. **How does this topic connect with your long term goals? -**

## Things I Want To Know More About
