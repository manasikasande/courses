# Understanding the Power of HTML

### Debugging HTML

- Right click -> Insepct Element
- Lot of information available
- DOM created by the browser can be seen
- Developer tools of any browser can be used
- Can be also used to debug mistakes

### HTML Attributes

- Global Attributes
  - Attributes in HTMl that can be applied to any element.
- ```class``` attribute
  - Gives us a way to target all elements with that class in our CSS of JavaScript.
- ```id``` attribute
  - Similar to class
  - Allows us to target a unique element with that id in our CSS of JavaScript
  - Can be used once in a page
- ```contenteditable``` attribute
  - Lets the visitor of the webpage edit that content
- ```lang``` attribute
  - Used to specify the language
- ```dir``` attribute
  - Used to specify direction of the text
- Many more such global attributes can be used.

### ARIA Roles

- HTML attributes that provide accessible information about that specific element.
- attribute name: ```aria-label```

### Weird Characters

Characters which are part of the code that is used to write html pages: <,>,&
When we want to use these characters in our content, use character entities.
For example:
```html
&lt - <
&gt - >
&amp; - &
&nbsp; - non breaking space
```


