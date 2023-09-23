# Forms and interactive elements

### HTML form basics

```html

<form action="suucess.html" method="get">
    <label for="name"> Name </label>
    <input name="name" id="name">
    <label for="email"> Email </label>
    <input name="email" id="email">
    <button> Sign Up </button>
</form>
```
- An HTML form is used to collect user input. The user input is most often sent to a server for processing.
- The ```<label>``` tag defines a label for many form elements.
- The ```<input>``` tag is used to take user input.
- Default input type is text.
- Other input types can be specified using ```type``` attribute
- ```<input type="text">```	Displays a single-line text input field
- ```<input type="radio">```	Displays a radio button (for selecting one of many choices)
- ```<input type="checkbox">```	Displays a checkbox (for selecting zero or more of many choices)
- ```<input type="submit">```	Displays a submit button (for submitting the form)
- ```<input type="button">```	Displays a clickable button
- Full list of the types can be viewed [here](https://www.w3schools.com/html/html_form_input_types.asp).
