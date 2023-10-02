# Getting started

## Referencing CSS

**Method 1: Inline**

- ```style ``` attribute is added to the opening html tag.
- CSS style rules are added as the value of the attribute.
```html
<p style="color:red;"> Red text </p>
```
- As the styles are applied directly to each element, they are not reusable. Each style declaration must be added to each element even if it is the same style.
- Multiple styles must be added to the same style attribute which can make it difficult to read and manage.

```html
<p style="color:red;font-size:12px;background#333;">Multiple Styles </p>
```
- Overrides style rules added by other methods potentially leading to conflicts.
- Should be used sparingly, if at all.
- Not flexible, can be difficult to maintain.

**Method 2: Internal**

- CSS is added to the head section of the HTML document.
- All the CSS style rules are enclosed between the style tags.
- CSS selectors are then used to apply the styles to the matched elements.
- To apply the same style to multiple html pages the style blocks must be added to each page.
- More flexible than inline css but not useful for multipage websites or longer blocks of CSS.

**Method 3: External**

- Most used and flexible method for bigger projects.
- Involves use of separate css file which is referenced in the html file using the link tag,

```html
<head>
    <title> page title </title>
    <link rel="stylesheet" href="css/styles.css">
</head>
```
- Can be shared among multiple html files in the same project by linking to the same CSS file.
- Separates CSS from HTML