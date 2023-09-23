# Putting it all together

### The HTML Page

- HTML File - The first file that's returned in response to a request for a webpage.
- Every .html file has the following:
  - The doctype declaration. Declares which era the html file is from.
  - ```<html>``` element
  - Within the html element - ```<head>``` and the ```<body>``` element.
    - ```<head>``` element is used for metadata.
    - ```<body>``` element is for the content.

```html
<!doctype html>
<html lang="en-US" dir="ltr">
    <head>
        ...
    </head>
    <body>
        ...
    </body>
</html>
```

### Document Head

- Information about the website that should be known to the browser is mentioned in the document head.
- ```<meta>``` element for example, is only used inside the head.
  - conveys metadata of the page
- ```<title>``` is used to display the name of the webpage on the browser.
- Attributes to define a responsive website:

```html
<meta name="viewport" content="width-device-width, initial-scale=1">
```
- Add a descriptions about the site that will show up in search engine results:

```html
<meta name="description" content="A description that will show up in search engine results">
```
- ```<link>``` element links to a range of assets that we want to load.
- css files
- fonts
- favicons
- ```rel``` attribute tells the browser about the kind of asset
- ```href``` provides the url

```html
<link href="main.css" rel="stylesheet">
<link rel="icon" href="favicon.ico">
<link rel="preload" href="myFont.woff2" as="font" type="font/woff2" crossorigin="anonymous">
```
- ```<script>```  tag tells the browser to load a javascript file.
```html
<script src="my-javascript-file.js"></script>
```

### Structuring content

- ```main```
  - wraps around the main content of the page
  - used only once per page
- ```header```
  - used to wrap site header
- ```footer```
  - used to wrap the site header
  - also used to convey extra information
- ```article```
  - wrapped around any instance of an article
  - used to display unit of content
- ```section```
  - used to mark each segment of the content
- ```aside```
  - marks content that is not the main attraction