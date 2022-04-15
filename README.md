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

## Angular Tour of Heroes
1. The Hero Editor
- You used the CLI to create a second HeroesComponent
- You displayed the HeroesComponent by adding it to the AppComponent shell
- You applied the UppercasePipe to format the name
- You used two-way data binding with the ngModel directive
- You learned about the AppModule
- You imported the FormsModule in the AppModule so that Angular would recognize and apply the ngModel directive
- You learned the importance of declaring components in the AppModule and appreciated that the CLI declared it for you

2. Display a List
- The Tour of Heroes application displays a list of heroes with a detail view
- The user can select a hero and see that hero's details
- You used *ngFor to display a list
- You used *ngIf to conditionally include or exclude a block of HTML
- You can toggle a CSS style class with a class binding.

3. Create a Feature Component
- You created a separate, reusable HeroDetailComponent.
- You used a property binding to give the parent HeroesComponent control over the child HeroDetailComponent.
- You used the @Input decorator to make the hero property available for binding by the external HeroesComponent.

4. Add Services
- You refactored data access to the HeroService class
- You registered the HeroService as the provider of its service at the root level so that it can be injected anywhere in the application
- You used Angular Dependency Injection to inject it into a component
- You gave the HeroService get data method an asynchronous signature
- You discovered Observable and the RxJS Observable library
- You used RxJS of() to return an observable of mock heroes (Observable<Hero[]>)
- The component's ngOnInit lifecycle hook calls the HeroService method, not the constructor
- You created a MessageService for loosely-coupled communication between classes
- The HeroService injected into a component is created with another injected service, MessageService

5. Add Navigation
- You added the Angular router to navigate among different components
- You turned the AppComponent into a navigation shell with <a> links and a <router-outlet>
- You configured the router in an AppRoutingModule
- You defined routes, a redirect route, and a parameterized route
- You used the routerLink directive in anchor elements
- You refactored a tightly-coupled master/detail view into a routed detail view
- You used router link parameters to navigate to the detail view of a user-selected hero
- You shared the HeroService among multiple components

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
