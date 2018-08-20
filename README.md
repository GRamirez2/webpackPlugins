# WebpackTest
## Adding Bootstrap
1. make sure you have the latest cli
2. `npm install bootstrap font-awesome angular-font-awesome --save`
3. In the angular.json
   ```
    "styles": [
    "src/styles.css",
    "node_modules/bootstrap/dist/css/bootstrap.min.css",
    "node_modules/font-awesome/css/font-awesome.css"
    ],
  
4. In the main module
  ```
  import { AngularFontAwesomeModule } from 'angular-font-awesome';

  @NgModule({
    //...
    imports: [
      //...
      AngularFontAwesomeModule
    ],
  ```
5. Inside the src/styles.css file add:
   
  `@import "~bootstrap/dist/css/bootstrap.css";`

  `@import "~font-awesome/css/font-awesome.css";`

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.1.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
