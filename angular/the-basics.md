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
