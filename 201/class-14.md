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

## Transitions and Animations Questions

1. **What does a CSS transition allow the developer to do to an element? -**
2. **How does a CSS animation differ from a CSS transition? -**

## 3 Simple CSS3 Transitions

## CSS3 Transition Questions

1. **What are some benefits to using CSS transitions on websites? -**
2. **How this topic fit in with your long-term goals? -**

## Things I Want To Know More About
