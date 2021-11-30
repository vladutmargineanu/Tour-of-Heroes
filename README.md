# Tour-of-Heroes
Application from the ground up, providing experience with the typical development process, as well as an introduction to basic app-design concepts, tools, and terminology.

---
## Index

### The Hero Editor

Summary
- You used the CLI to create a second HeroesComponent.
- You displayed the HeroesComponent by adding it to the AppComponent shell.
- You applied the UppercasePipe to format the name.
- You used two-way data binding with the ngModel directive.
- You learned about the AppModule.
- You imported the FormsModule in the AppModule so that Angular would recognize and apply the ngModel directive.
- You learned the importance of declaring components in the AppModule and appreciated that the CLI declared it for you.

```
ng new angular-tour-of-heroes

cd angular-tour-of-heroes
ng serve --open

ng generate component heroes

ng generate component heroes

```
---

### Display a list

Summary
- The Tour of Heroes application displays a list of heroes with a detail view.
- The user can select a hero and see that hero's details.
- You used *ngFor to display a list.
- You used *ngIf to conditionally include or exclude a block of HTML.
- You can toggle a CSS style class with a class binding.

---

### Create a Feature Component

Summary
- You created a separate, reusable HeroDetailComponent.
- You used a property binding to give the parent HeroesComponent control over the child HeroDetailComponent.
- You used the @Input decorator to make the hero property available for binding by the external HeroesComponent.

```
ng generate component hero-detail
```

### Add Services

Summary
- You refactored data access to the HeroService class.
- You registered the HeroService as the provider of its service at the root level so that it can be injected anywhere in the application.
- You used Angular Dependency Injection to inject it into a component.
- You gave the HeroService get data method an asynchronous signature.
- You discovered Observable and the RxJS Observable library.
- You used RxJS of() to return an observable of mock heroes (Observable<Hero[]>).
- The component's ngOnInit lifecycle hook calls the HeroService method, not the constructor.
- You created a MessageService for loosely-coupled communication between classes.
- The HeroService injected into a component is created with another injected service, MessageService.

```
ng generate service hero

ng generate component messages

ng generate service message

```
