# Transforms, Transitions, and Animations

## CSS Transforms

Use vendor prefixes to ensure your code will work, and use the un-prefixed declaration so it overwrites the others if it's supported.

Transforms work on both 2D and 3D planes.

2D Transforms:

* Rotate
* Scale
* Translate
* Skew

Add multiple effects on the same fransform property, never make multiple transforms on one element or they will overwrite one another. `transform: scale(1.5) rotate(90deg);`.

`transform-origin` will change the center of the animation.

Setting the perspective will give your element a vanishing point. Setting `perspective-origin' will set the coordinates of your perspective.

3D Transforms:

* rotatex, rotatey, rotatez
* scalez
* translatez

`transform-style: preseve-3d;` on a parent 3D element will preserve its childrens 3D properties.

`backface-visibility: hidden;` will hide the element if it's facing away from the user.

## CSS Transforms Questions

1. **What does a CSS transform allow the developer to do to an element? -** It allows us alternative ways to size, position, and change elements.
2. **Provide an example of a transform and how you could see that being used on a website. -** On a site that sells software, or even cereal, you can create a product box that looks 3D by using transform. This can be used to make the user feel like they're purchasing a physical product even if they aren't.

## CSS Transitions and Animations

### Transitions

Transition let you alter the appearance and behavior of an element whenever a state change happens like hover, focus, active, or target.

Animations do the same over the course of multiple keyframes while transitions only provide a change from one state to another.

transition has 4 properties:

* transition-property
* transition-duration
* transition-timing-function
* transition-delay

It's suggested to use vendor prefixes.

Not all properties can be transitioned. Only ones with an obvious midpoint. like, opacity works but hidden does not.

Much like you can set multiple properties to transition, you can set multiple durations. one for each property. the same can be done with timing function, and the delay.

Shorthand;

```CSS
transition: property duration timing-function delay;
```

for multiple properties, seperate them with a comma:

```CSS
transition property duration timingfunction, property duration timingfunction delay;
```

### Animations

Animation properties are similar to transition. One called animation-name points to the @keyframes rule that defines the different steps of the animation. iteration-count tell the animation how many times to play, infinite is an option.

animation-direction will play in either normal, reverse, alternate, and alternate-reverse. Normal and reverse do as you would expect. alternate will alternate between the two. First playing normal, then playing in reverse.

play-state will allow you to pause the animation.

fill-mode identifies hwo an element should be styles before, after, or both, after the animation has been run. Arguments it takes are none, forwards, backwards, and both.

shorthand:

```CSS
animation: name duration timingFunction delay iterationCount direction fillMode playState;
```

## Transitions and Animations Questions

1. **What does a CSS transition allow the developer to do to an element? -** It let's you alter size, position and change an element over the course of multiple keyframes.
2. **How does a CSS animation differ from a CSS transition? -** It requires the use of keyframes and lets you change the element from one state to multiple other states over time.

## 3 Simple CSS3 Transitions

1. Fade in - opacity from 0.5 to 1
2. Change color
3. Grow and Shrink - use transform: scale
4. Rotate - transform: rotate
5. square to circle - border radius
6. 3D shadow - give box shadow then transform: translate X&Y
7. Swing - animate using transform: translate
8. inset border - create a ghost button by setting the border

## CSS3 Transition Questions

1. **What are some benefits to using CSS transitions on websites? -** They can excite your users, increase engagement, and increase conversation
2. **How this topic fit in with your long-term goals? -** Using some of these animations will ultimately help me create cleaner and more interactive websites!

## Things I Want To Know More About

* Cubic Bezier Curve and how to use it.
