# Formatting Text

### Syntax of HTML elements

- Opening tag - content - closing tag
- These three together form an element.
- Not every element has a closing tag, but most HTML elements have an opening and closing tag.

**Document Object Model (DOM)**

- Represents the structure of a web page or a web document with the help of a tree.
- Often used for targeting elements in CSS and JavaScript.

### Paragraphs

Syntax
```html
<p> Content of your paragraph </p>
```
### Headlines

- H1 - biggest, H6 - smallest
- Syntax
- H1 is usually used for main title

```html
<h1> Heading 1 </h1>
<h2> Heading 2 </h2>
<h3> Heading 3 </h3>
<h4> Heading 4 </h4>
<h5> Heading 5 </h5>
<h6> Heading 6 </h6>
```

### Bold and Italics

```html
<i> - visual only italics
<em> - emphasized italics
<strong> - conveys importance, seriousness and urgency
<b> - bold
```
### Lists

Unordered lists
- used most often

```html
<ul>
    <li> item1 </li>
    <li> item2 </li>
    <li> item3 </li>
</ul>
```

Ordered lists
- contains numbers

```html
<ol>
    <li> item1 </li>
    <li> item2 </li>
    <li> item3 </li>
</ol>
```

Definition lists
- A description list, with terms and descriptions

```html
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```
### Quotes

- Blockquote element
- Block level element

```html
<blockquote>
<p> "Sample Quote" </p>
<cite>- Author</cite>
</blockquote>
```

- Instead of typing the quotes manually we can use this structure and let the browser provide the quote marks for us.

- ```<q>``` element is an inline element.

- It is wrapped around phrases of text.

```html
<p> Sentence <q>Your quote</q> Sentence<p>
```
 
### Dates and Times

- ```<time>``` element is used to format date and time.
- Any human understandable format can be used for the phrase of text that is displayed in the tags.
- Attributes are used to provide more details.

```html
<time datetime="2025-05-08"> May 8, 2025 </time>
```

- Machine readable formats for datetime attribute: 
  - YYYY-MM-DD
  - HH:MM (24 hour format)
  - HH-MM-SS.DDD
  - HH-MM-SS.DDD+-hh:mm (timezone)
  - Date and time can also be used together (date followed by time)

### Code, pre, and br

- ```<code>``` element is used to indicate a block of code.
- Inline element.

```html
<p> your content 
  <code> block of code <code> 
    remaining content
</p>
```
- To write about html elements on the webpage:
  - &lt is equivalent to <
  - &gt is quivalent to >
- ```<br>``` is used for line breaks.
- no opening and closing tags
- ```<pre>``` is used for indentation
- Opening and closing tags are used.

### Superscripts, subscripts, and small text

- Subscripts - Characters that are set below the text baseline.
  - ```<sub>``` element is used.
  - Has an opening and closing tag.
- Superscripts - Characters that are set above the text baseline.
  - ```<sup>``` element is used.
  - Has an opening and closing tag.
- Fine print is needed at times. Smaller than usual text size.
  - ```<small>``` tag can be used.
  - Has an opening and closing tag.
- These 3 elements are mainly used in typography.