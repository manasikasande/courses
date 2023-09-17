# Images and Graphics

- ```<img>``` is used to add images.
- 4 attributes that should be used along with the tag:
  - src
  - alt
  - width
  - height

### Image Formats

Four main file formats
- GIF
  - Does well compressing large areas of a single colour
  - Limited colour space of 256 Colours
  - Pixelation possible
  - Can have multiple frames, and make a little movie.
- SVG
  - Great for logos, icons
  - Vector file
  - No pixelation
- JPG
  - Image format for compressing photos
  - Size vs quality balance can be maintained
- PNG
  - Images that need transparency
  - Good at compression

### Responsive Images and Responsive Width

The below notes have been obtained from [this link]( https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images).

- Responsive images are images that work well on various screen sizes and devices.
- Ideally, multiple resolutions should be made available to the user's web browser. 
- The browser could then determine the optimal resolution to load based on the screen size of the user's device. 
- Some devices have high resolution screens that need larger images than you might expect to display nicely. 
- We can use two attributes — ```srcset``` and ```sizes``` — to provide several additional source images along with hints to help the browser pick the right one. 

```html
<img
  srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
  sizes="(max-width: 600px) 480px,
         800px"
  src="elva-fairy-800w.jpg"
  alt="Elva dressed as a fairy" />
```
```srcset``` attribute allows you to specify multiple files to be used based on either viewport width or mage pixel width. <br>
```srcset``` defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma. For each one, we write:
1. An image filename (elva-fairy-480w.jpg)
2. A space
3. The image's intrinsic width in pixels (480w)

```sizes``` defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true. In this case, before each comma we write:
1. A media condition ((max-width:600px)) — a media condition describes a possible state that the screen can be in. In this case, we are saying "when the viewport width is 600 pixels or less".
2. A space
3. The width of the slot the image will fill when the media condition is true (480px)

If you're supporting multiple display resolutions, but everyone sees your image at the same real-world size on the screen, you can allow the browser to choose an appropriate resolution image by using ```srcset``` with x-descriptors and without ```sizes```.

```html
<img
  srcset="elva-fairy-320w.jpg, elva-fairy-480w.jpg 1.5x, elva-fairy-640w.jpg 2x"
  src="elva-fairy-640w.jpg"
  alt="Elva dressed as a fairy" />
```
### Responsive Pictures

- Needed when we want to use different images altogether on different types of screens.
- ```picture``` and ```source``` element is used for this purpose.

```html
<picture>
    <source media="condition"
            srcset="path/of/file/when/it/matches/the/condition">
    <source srcset="path/of/the/other/file">
    <img src="img/path"
        width="480" height="360"
        alt="Description">
</picture>
```
### Figure and figcaption

- ```<figcaption>``` is used for providing captions to the image.
- ```<img>``` and ```<figcaption>``` together are then wrapped inside the ```<figure>``` element.
- ```<figure>``` is used for anything that appears as a figure and illustrates something.
