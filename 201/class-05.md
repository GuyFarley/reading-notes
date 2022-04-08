# Code 201 - Class 05 - HTML Images; CSS Color & Text

## HTML Chapter 5: “Images” (pp.94-125)

- Images can be added to your page using the `<img>` tag:

```
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2e/Salmo_trutta.jpg/1280px-Salmo_trutta.jpg" alt="photo of a trout" />
```

- In the code example above, the `<img>` element is an empty element (no closing tag). `src=" "` notes the source location of the image. And  `alt=" "` provides a text description in case the image is not visible, or for accessibility purposes
- It is best to save your images at the size you will be using on the web page
- As a rule of thumb, photos = JPGs and illustrations/logos = GIFs

## HTML Chapter 11: “Color” (pp.246-263)

- You can use 3 different methods to specify color in CSS
>
>- RGB (Red, Green, Blue)
>- hex (RGB represented in hexadecimal code)
>- color names
>
- With CSS3, there is now an additional method that is used to indicate opacity: RGBA
- Additionally, CSS3 lets you specify colors as HSL (Hue, Saturation, Lightness) values + optional opacity (Alpha): HSLA

## HTML Chapter 12: “Text” (pp.264-299)

- It's important to remember that typefaces will only display on a browser if they're stored on a user's computer. For this reason, most sites use a small set of typfaces that already exist on most computers. For instance:

```
font-family: Georgia, Times, serif;
```

- CSS allows you to control the space between lines of text, letters, and words
- Pseudo-classes can be used to change the style of text when it is hovered over or clicked on:
>
>- `:hover`
>- `:active`
>- `:focus`
>
- A few properties that can be used to alter the appearance of text on the page:
>
>- `font-weight`
>- `font-style`
>- `text-transform`
>- `text-decoration`
>- `line-height`
>- `letter-spacing`
>- `word-spacing`
>- `text-align`
>- `vertical-align`

## [Blog Post: JPEG vs PNG vs GIF](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

There are hundreds of digital image formats, but the 3 that make up 95% of images on the web are: **JPEG**, **PNG**, and **GIF**. When is it best to use each format?

### JPEGs are best used for

- Photos or natural scenes where variation in color is smooth, due to its **lossy** compression. Using it for these types of images will reduce artifacts (visual imperfections) when the file is compressed for the web
- JPEGS are also great for these types of images because they can support around 16 million colors

### PNGs are best used for

- Images with text, logos, graphics with sharp edges due to it's **lossless** compression
- Images where transparency is required

### GIFs are best used for

- Animations

[Back to Home](../README.md)
