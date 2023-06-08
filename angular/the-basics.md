# Chapter 2: The Basics

## Loading and starting an angular application

- `main.ts` file is the first file that is executes when `ng serve` is run
- Angular application is bootstrapped and module is passed as argument
- index.html file is served by the server
- `<body>` tag of index.html file contains the `<app-root>` tag which is not a default html element
- `<app-root>` is the selector of the root component of angular project created by the CLI
- files under `app` folder are related to the component
- the file `app.component.ts` contains the name of the selector inside its decorator
- Once the CLI detects the `<app-root>` tag in index.html, it replaces it with the template of the root component, which is written in `app.component.html`

## Components

- Key feature of Angular
- Each component has its own:
  - template
  - html code
  - styling
  - business logic
- separate folder for each new component
- all folders created under `app/` directory
- component is simply a TS class

**Steps to create a component**
Method 1: Manual

- Create a new folder under `app/` directory with the component name
- Under the folder, create its corresponding .ts and .html file.
- .ts file should contain the relevent imports, decorator and class
- .html file contains the template of the component
- In `app.module.ts` file add component name to declarations and import the component
- Use the component's tag (same as selector) inside `app.component.html` file to render it

Method 2: Using CLI

```
ng generate component component-name

or

ng g c component-name
```