# Angular - The Complete Guide [2023 Edition]

## Course Structure

- Getting Started
- The Basics
- Components and Databinding
- Directives
- Services and Dependency Injection
- Routing
- Observables
- Forms
- Pipes
- Http
- Authentication
- Optimizations & NgModules
- Deployment

## Getting Started

### Angular is

- JavaScript Framework
- can create reactive Single-Page-Applications (SPAs)

### Reactive Single Page Applications

- web application that dynamically rewrites a current web page
- web browser doesn't load entirely new pages
- no page refresh
- HTML code and DOM is changed by JavaScript during runtime

### Angular Versioning

- AngularJS - Angular 1
- Angular 2 (totally different than Angular 1)
- Angular 4
- Angular 10,11,12,...
- New major version is released every 6 months
- From Angular 2 onwards -> small, incremental, backwards-compatible changes

### Installation Steps

1. Install node js
2. Open terminal as administrator
```
npm install -g @angular/cli@latest
```
### How to create and run application

**Steps to create a simple app with no routing:**
1. Open terminal as administrator
2. navigate to project directory
3. Run the below command.
```
ng new project-name --no-strict

Press N when asked about routing
default styling - CSS
```
When you run this command, the CLI installs the necessary Angular npm packages and other dependencies in a new workspace, with a root-level application named project-name. The workspace root folder contains various support and configuration files, and a README file with generated descriptive text that you can customize.

By default, ng new creates an initial skeleton application at the root level of the workspace.

Ref - [Angular Documentation](https://angular.io/guide/file-structure)

**Command to run the app:**

```
ng serve
```
### What is TypeScript ?

- Super set to JavaScript
- More features than vanilla JS (e.g Types, Classes, Interfaces,..)
- TypeScript is compiled to JavaScript in the end

