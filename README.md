# AngularTourOfHeroes
View tutorial here: [https://angular.io/tutorial/](https://angular.io/tutorial/)

#### Overall Angular Workflow
- App Module imports every component
- HTML component file can call imported components using their CSS element selector
- TypeScript component file calls service functions for data and lifecycle methods are here
- Service retrieves data asynchronously using Observer library RxJS - updates are done through publish/subscribe design pattern

## Notes
- Angular CLI to generate component, services
- Generate heroes component and use in app.component.html
- Generate hero-detail component and use in heroes.component.html
- Annotate class with decorator that specifies Angular metadata - eg: @Component
- Angular event binding syntax - ```<button type="button" (click)="onSelect(hero)"``` and ```<input id="hero-name" [(ngModel)]="selectedHero.name" placeholder="name">```
- Angular conditional rendering - ```<div *ngIf="selectedHero">```
- Annotate data member with decorator - eg: @Input - The input property is bound to a DOM property in the template. During change detection, Angular automatically updates the data property with the DOM property's value.
- Service handles retrieval of data and passes to component

## Angular CLI README
This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
