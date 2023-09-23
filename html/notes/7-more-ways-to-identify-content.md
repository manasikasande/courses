# More ways to identify content

### Supporting Languages

- ```lang``` attribute is used to specify the language of the content.
- Can be used with any element.

```html
<html lang="en-us">
    ...
</html>
```
- direction of the content can also be specified.
- Languages like Arabic and hebrew flow from right to left direction.
- ```dir``` attribute is used to specify direction.
- ```dir="ltr"``` and ```dir="rtl"``` are the two values.
- ```charset``` attribute - defines the alphabet or set of characters for the script language.

```html
<head>
    <meta charset="UTF-8>
</head>
```
### Generic elements: div and span

- Sometime we just need a way to wrap a group of elements or to mark a phrase.
- Sometimes we just need a way to target a part of the DOM with CSS or JavaScript.
- Two elements for this purpose:
  - ```<div>```
  - ```<span>```
- div is a block level element.
- span is an inline element.
- both elements can take all global attributes