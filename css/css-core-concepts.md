# CSS Core concepts

### CSS Syntax and terminology

- Declaration blocks in css - contains one or more style rules enclosed in curly braces.
- Here, ```body``` is the selector which specifies the HTML element being styled.
- ```background: blue;``` is a declaration which tells the browser more about the styling to be applied.
- Each declaration is made in the format ```property: value;```.

```css
body {
    background: blue;
}
```

### CSS Properties, Values and Units

- Each property is given a specific value and values can be given in various units.
- Values are also known as data types.

**Numeric Data Types**

- Number based values
- Used with or without units to define different styles

```css

width: 80%;
height: 1vh;
border-width: 2px;
animation-iteration-count: 2;
```
- Different numeric data types:
  - integer - negative or positive whole number
  - number - whole number or a fraction with decimals
  - percentage - A fraction of another value (usually a parent or ancestor element) that uses a number with a percentage unit
  - dimension - number value with a unit like ```ms, dppx, vw,``` etc. Represents data types such as time, resolution, length and more
  - length - used to define a distance value. Example ```width``` or ```font-size```.
- number values are used with absolute or relative units.
- absolute units - fixed units based on physical measurements
  - px: pixels
  - cm: centimeters
  - mm: millimeters
  - Q: quarter-millimeters
  - in: inches
  - pt: points
- relative units - define a length based on another length
- ```em``` is relative to the font size of an ancestor element
- ```rem``` is relative to the root element
- Viewport based units are relative to the size of the browser viewport
- ```vw``` is relative to the viewport width, ```vh``` to the viewport height

**Keywords**

- textual data types
- pre defined values that vary depending on the property

**Functions**

- function values can include more complex values.
- Start with the name of the function, followed by parentheses
- includes one or more arguments that are used to compute a value

### The color property and values

- The ```color``` property changes an element's text color and text decorations (such as underline or strikethrough).
- It is defined with different types of color values.
- Keywords are one way to define the values

RGB Function values

```css
/* syntax */
rgb([red] [green] [blue])

color: rgb(0 0 0); /* black */
color: rgb(255 255 255); /* white */
color: rgb(255 0 0); /* a shade of red */
color: rgb(0 255 0); /* a shade of green */
color: rgb(0 0 255); /* a shade of blue */
```
To add transparency an optional fourth value can be added which uses a value between 0 and 1 or a percentage between 0 and 100.

```css
color: rgba(0 0 0/ 0.5); /* black with 50% opacity */
color: rgba(0 0 255/ 25%) /* blue with 25% opacity */
```
**RGB Hexadecimal values**

```css
/* syntax */
#rrggbb or #RRGGBB

color: #000000; /* black */
color: #ffffff; /* white */
color: #ff0000; /* A shade of red */
color: #008000; /* A shade of green */
color: #0000ff; /* A shade of blue */
```
To add transparency

```css
/* syntax */

#rrggbba or #rrggbbaa

color: #9ACD320; /* yellow green with no opacity (full transparency) */

color: #9ACD32FF; /* yellow green with full opacity (no transparency) */
```
### Type and Universal Selectors

- CSS selectors - used to select specific HTML elements and apply styles to them
- Different types of selectors are used to determine which element the style should be applied to.

**Type Selectors**

- Also known as element selectors
- Matches the element name but without the angular brackets

```css
/* this style will apply to all <h2> elements */

h2 {
    color: red;
}
```
**Universal selector**

- Selects all elements on the HTML page using an asterisk (*)
- May cause performance issues and should be used sparingly

```css
/* this style will be applied to all elements */
* {
    border: 1px solid black;
}
```
