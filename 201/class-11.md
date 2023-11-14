# Audio, Video, Images

## Video and Audio Content

The `<video>` element lets you embed a video on your page. `src` points to the bideo, like the `src` you find in the img element. The controls attribute displays the default browser controls. You don't have to use them and can use custom controls but you need to have play/pause and volume controls at the minimum. The content within the `<video>` tags is called fallback content and is used or displayed if the browser doesn't support the initial source.

Formats like mp3, mp4, and WebM are called container formats. They hold more information that just audio and video. Since support for these formats can't be garunteed, it's good to try and have a few options available for total support.

and example of using fallback content:

```html
<video controls>
  <source src="source1.mp4" type="video/mp4" />
  <source src="source2.webm" type="video/webm" />
  <p>
    Your browswer doesn't support this video.
  </p>
</video>
```

Other video features include:

* `width/height`
* `autoplay`
* `loop`
* `muted`
* `poster`
* `preload`

The `<audio>` element works just liek the `<video>` element with jsut a few small differences.

* Doesn't support width/height.
* Doesn't support poster.

WebvTT is a format used to provide text taht accompanies a video. It is made up of cues. The most common ones are:

* subtitles
* captions
* timed descriptions

## Video and Audio Questions

1. **Explain how the ability to use video and audio on the web has evolved since the early 2000s. -** You once needed specialized software like flash or silverlite to embed media on your site. But now you can achieve this much more easily and securely with native HTML elements while interacting with them in javascript.
2. **Describe the use of the `src` and `controls` attributes in the `<video>` element. -** `src` will point to where your video resides and `controls` tells the browser whether or not to display the play/pause/skip/volume controls or not.
3. **Why is it important to have *fallback content* inside the `<video>` element? -** Media formats are not garunteed to be covered by each individual browser. So it's important to have other options just in case your initial format isn't supported.
4. **Write a very short story where `<audio>` and `<video>` are characters. -** There once were two twin brothers, one named audio and one named video. They were not identical twins but were fraternal twins. They looked very much alike, and could do almost all of the same things. But video was a little bit taller, maybe a little bit wider, and was a little bit of a showoff. Audio didn't mind, he knew they were their own people, just doing what they did best. Besides, Audio didn't like being noticed too much, he very much prefered to be heard than seen.

## A Complete Guide To Grid

Grid is a page layout tool amde to solve the issues that came with laying pages out with tables or floats or inline block. It also works well when paired with flexbox.

Grid Terminology:

* Grid Container - Direct parent of all grid items.
* Grid Item - The children of grid container. The children of these elements are not themselves grid items.
* Grid Line - Lines that make up the structure of the grid.
* Grid Cell - Space between 2 adjeacent row and column lines.
* Grid Track - Space between 2 adjacent grid lines. AKA columns or rows.
* Grid Area - Total space surrounded by 4 grid lines.

## Grid Questions

1. **How does Grid layout differ from Flex? -** Grid layout is two dimension, you can lay out items up or down, as well as left or right at the same time. Flex only lays items out in a single direction. You can explicitly place items on a grid in a specific location where as you aren't able to do that with flex.
2. **Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences. -** The grid container is the direct parent of all the grid items, and those grid items live inside of that grid container. the grid lines are what seperates the content and makes up the structure of the grid.

## Responsive Images

`srcset` defines the set of image the browser can choose from.

`sizes` are the conditions that browser uses to choose what image to use.

**Art Direction** is when you want to serve cropped images for different layouts.

**Resolution Switching** is where you want to serve smaller images to narrower screens & different resolution pictures to high/low density screens.

## Responsive Images Questions

1. **Besides making a site visually appealing across different screen sizes, why should developers make images responsive? -** It can actually cut back on bandwidth because you're sending less data to the user overall.
2. **Define the following `<img>` attributes `srcset` and `sizes`. Write an example of how they are used. -** `srcset` defines the set of images the browser can use, `sizes` are the conditions that the browsers uses to choose an image from that set. For example you can have an image for desktop users and different sized image for mobile users, In the `sizes` you would specify how big the viewport should be for each image to be displayed. that way the browser knows which image to serve to the user.
3. **How is `srcset` more helpful for responsive images than CSS or JavaScript? -** since the `<img>` part of the HTML it's processed before the CSS or Javascript, so the browser knows exactly which image to use and loads it in before it even starts to pull the CSS and JS files in.

## Things I Want To Know More About
