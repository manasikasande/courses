# Media

### Audio

- ```<audio>``` element is used to put audio files on a webpage.
- Has both opening and closing tag.
- Attributes that can be used
  - controls - to show playback controls
  - loop - to loop the audio
  - autoplay - set autoplay to true

```html
<audio controls loop autoplay src="audio.mp3"></audio>
```
- We can use multiple formats for a single audio file by using the ```<source>``` element.
- The browser will execute the first format that it understands.

```html
<audio controls loop autoplay>
    <source src="birds.ogg"
            type="audio.ogg; codec=opus">
    <source src="birds.mp3"
            type="audio/mpeg">
    Sorry your browser doesn't support the audio file
```
- .mp3 is supported by most browsers. 

### Video

- H.264 codec currently has the widest support across browsers.
  - Not open source
  - Fees to use
- Other codecs
  - WebM
  - AV1
- Syntax similar to ```<audio>``` element

```html
<video controls>
    <source src="path.webm"
            type="video/webm">
    <source src="path.h264.mp4"
            type="video/mp4">
</video>
```
### Captions and subtitles

- ```<track>``` element provides subtitles and captions to a video.
- It points to a text file.
- File format - webvtt

```html
<video controls>
    <source src="path.webm"
            type="video/webm">
    <source src="path.h264.mp4"
            type="video/mp4">
    <track src="captions/path.webvtt"
            kind="captions"
            label="english"
            srclang="en"
            default>
    <track src="subtitles/path.webvtt"
            kind="subtitles"
            label="Spanish"
            srclang="es"
            default>
</video>
```
### Embedding other media through iframes

- Embedding - placing content from one site into the body of a page of another site.
- HTML code required to embed is present on the source website. For example - the share option in YouTube.