# Images, Color, Text

## HTML

### Using Images In HTML

The `<img>` element is a void element, it can have no children and has no end tag. It requires two attributes to be useful. `src` and `alt`.

Absolute URL's aren't ideal when it comes to the `src` attribute. But they can be used.

`alt` is supposed to be a textual description of the image, for when the image can't be seen or displayed.

### Common Image Types

* **APNG** (.apng) - Animated Portable Network Graphics is like a higher quality GIF.
* **AVIF** (.avif) - AV1 Image File format is a good choice for still and animated images. Not entirely supported by all browsers.
* **GIF** (.gif) - Graphics Interchange Format is a widely supported format for simple images and animations.
* **JPEG** (.jpg / .jpeg) - Joint Photographic Expert Group image is the most popular format on the web, but not as detailed as PNG.
* **PNG** (.png) - Portable Network Graphics, Good for precise reproductions of source images.
* **SVG** (.svg) - Selectable Vector Graphic, Great for UI elements, icons, and diagrams. Acurate drawings that can be scaled.
* **WebP** (.webp) - Web Picture Format, grat choice for both still and animated images. Great compression and widely supported.

### Choosing Image Formats

**Photos**, JPEG and WebP are both good choices with WebP being the best choice and JPEG being the most popular. Consider providing both with a failover to JPEG.

**Icons**, SVG is best if the icon allows it, otherwise PNG would be good. You can use a fallback image here as well.

**Screenshots**, Best to use a lossless format like Lossless WebP or PNG to preserve details and text clarity.

**Diagrams, Drawings & Charts**, Anyt of these that can be represented with SVG probably should.

**Providing Fallbacks**, `<img>` does not allow you to fallback on another image, but the `<picture>` element does by wrapping around multiple `<source>` elements as well as an `<img>` element that describes how the image is to be displayed.

```html
<picture>
  <source srcset="diagram.svg" type="image/svg+xml" />
  <source srcset="diagram.png" type="image/png" />
  <img
    src="diagram.gif"
    width="620"
    height="540"
    alt="Diagram showing the data channels" />
</picture>
```

### HTML Questions

1. **What is a real world use case for the `alt` attribute being used in a website? -** If a user is visually impaired it can be very helpful for them to understand what the image is, and the alt text helps with that.
2. **How can you improve accessibility of images in an HTML document? -** be sure to include the alt text, and try not to use the title attribute. instead try to include that information in the main text of the article.
3. **Provide an example of when the `figure` element would be useful in an HTML document. -** It's a great solution to combine an image and a textual caption of that image together, Like if you have an image of a celebrity at a charity event in your article, you can use the `<figure>` element to combine the image and description of the event.
4. **Describe the difference between a `gif` image and an `svg` image, pretend you are explaining to an elder in your community. -** A gif is like a short movie clip without sound, and an svg is a picture made up of a bunch of shapes or strokes layered on one another like a collage or painting.
5. **What image type would you use to display a screenshot on your website and why? -** Either a Lossless WebP or PNG filetype would be best so you can preserve the image details.

## CSS

### Using Color In CSS

The color property defines the foreground color of an elements content and background-color defines the elements background color.

### Styling HTML Text Elements

Font styling in css usually falls in 2 categories. 

- Font styles: properties that affect the texts font, which font is applied, its size, and if it's bold, italic, ect.
- Text layout: Properties that affect spacing and other layout features.

When setting your font, you can add fallbacks in case the first is not supported. You can wrap a font with a space in its name with quotes so there are no issues.

```css
p {
    font-family: "Trebuchet MS", Verdana, Sans-Serif;
}
```

### CSS Questions

1. **Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge. -** The foreground pretty much covers the text of the element, where the background covers what's behind the text.
2. **Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character? -** I would start with whatever the theme of the blog is and find out if there is a color that is associated with it, if there is no color or theme, then i would ask for his favorite color or some emotion he would like to convey. then use tools to find complimentary colors to go with the main color chosen.
3. **What should you consider when choosing fonts for an HTML document? -**
4. **What do `font-size`, `font-weight`, and `font-style` do to HTML text elements? -** they each respectively deal with the size of the text, whether it's bold or not, and wheter it's italic or not.
5. **Describe two ways you could add spacing around the characters displayed in an `h1` element. -** `line-height` to add space above and below and `letter-spacing` to add space to the sides of each character.
