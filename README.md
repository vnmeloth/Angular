Here's a comprehensive README format with questions and answers about Angular, including examples for each question.

```markdown
# Angular FAQ

## Table of Contents
1. [How do you create a new Angular component?](#1-how-do-you-create-a-new-angular-component)
2. [How do you create a new Angular service?](#2-how-do-you-create-a-new-angular-service)
3. [What is Angular CLI and how do you install it?](#3-what-is-angular-cli-and-how-do-you-install-it)
4. [How do you generate a new Angular project using Angular CLI?](#4-how-do-you-generate-a-new-angular-project-using-angular-cli)
5. [How do you start the development server in an Angular project?](#5-how-do-you-start-the-development-server-in-an-angular-project)
6. [What is the purpose of `ng serve`?](#6-what-is-the-purpose-of-ng-serve)
7. [How do you add routing to an Angular application?](#7-how-do-you-add-routing-to-an-angular-application)
8. [How do you create a new route in Angular?](#8-how-do-you-create-a-new-route-in-angular)
9. [How do you navigate between routes in Angular?](#9-how-do-you-navigate-between-routes-in-angular)
10. [What is the purpose of the `RouterModule` in Angular?](#10-what-is-the-purpose-of-the-routermodule-in-angular)
11. [How do you pass data between components in Angular?](#11-how-do-you-pass-data-between-components-in-angular)
12. [What is an Angular module and how do you create one?](#12-what-is-an-angular-module-and-how-do-you-create-one)
13. [How do you use Angular services to share data between components?](#13-how-do-you-use-angular-services-to-share-data-between-components)
14. [What is dependency injection in Angular?](#14-what-is-dependency-injection-in-angular)
15. [How do you inject a service into a component in Angular?](#15-how-do-you-inject-a-service-into-a-component-in-angular)
16. [How do you use lifecycle hooks in Angular components?](#16-how-do-you-use-lifecycle-hooks-in-angular-components)
17. [What is the purpose of the `ngOnInit` lifecycle hook in Angular?](#17-what-is-the-purpose-of-the-ngoninit-lifecycle-hook-in-angular)
18. [How do you create a custom directive in Angular?](#18-how-do-you-create-a-custom-directive-in-angular)
19. [How do you use a custom directive in an Angular template?](#19-how-do-you-use-a-custom-directive-in-an-angular-template)
20. [What is the purpose of the `@Input` decorator in Angular?](#20-what-is-the-purpose-of-the-input-decorator-in-angular)
21. [How do you use the `@Output` decorator in Angular?](#21-how-do-you-use-the-output-decorator-in-angular)
22. [How do you bind a method to an event in an Angular template?](#22-how-do-you-bind-a-method-to-an-event-in-an-angular-template)
23. [What is two-way data binding in Angular?](#23-what-is-two-way-data-binding-in-angular)
24. [How do you implement two-way data binding in Angular?](#24-how-do-you-implement-two-way-data-binding-in-angular)
25. [What are Angular pipes and how do you use them?](#25-what-are-angular-pipes-and-how-do-you-use-them)
26. [How do you create a custom pipe in Angular?](#26-how-do-you-create-a-custom-pipe-in-angular)
27. [How do you chain pipes in Angular?](#27-how-do-you-chain-pipes-in-angular)
28. [What is a pure pipe in Angular?](#28-what-is-a-pure-pipe-in-angular)
29. [What is an impure pipe in Angular?](#29-what-is-an-impure-pipe-in-angular)
30. [How do you handle form validation in Angular?](#30-how-do-you-handle-form-validation-in-angular)
31. [How do you create a reactive form in Angular?](#31-how-do-you-create-a-reactive-form-in-angular)
32. [How do you create a template-driven form in Angular?](#32-how-do-you-create-a-template-driven-form-in-angular)
33. [How do you use form groups in Angular?](#33-how-do-you-use-form-groups-in-angular)
34. [How do you use form controls in Angular?](#34-how-do-you-use-form-controls-in-angular)
35. [How do you validate form controls in Angular?](#35-how-do-you-validate-form-controls-in-angular)
36. [How do you create a custom validator in Angular?](#36-how-do-you-create-a-custom-validator-in-angular)
37. [How do you use the `ngModel` directive in Angular?](#37-how-do-you-use-the-ngmodel-directive-in-angular)
38. [How do you handle form submission in Angular?](#38-how-do-you-handle-form-submission-in-angular)
39. [How do you reset a form in Angular?](#39-how-do-you-reset-a-form-in-angular)
40. [What is the purpose of the `HttpClient` module in Angular?](#40-what-is-the-purpose-of-the-httpclient-module-in-angular)
41. [How do you make HTTP requests in Angular?](#41-how-do-you-make-http-requests-in-angular)
42. [How do you handle HTTP errors in Angular?](#42-how-do-you-handle-http-errors-in-angular)
43. [How do you use interceptors in Angular?](#43-how-do-you-use-interceptors-in-angular)
44. [How do you implement authentication in an Angular application?](#44-how-do-you-implement-authentication-in-an-angular-application)
45. [How do you implement route guards in Angular?](#45-how-do-you-implement-route-guards-in-angular)
46. [How do you create a canActivate guard in Angular?](#46-how-do-you-create-a-canactivate-guard-in-angular)
47. [How do you use lazy loading in Angular?](#47-how-do-you-use-lazy-loading-in-angular)
48. [How do you optimize an Angular application for production?](#48-how-do-you-optimize-an-angular-application-for-production)
49. [What is Ahead-of-Time (AOT) compilation in Angular?](#49-what-is-ahead-of-time-aot-compilation-in-angular)
50. [How do you enable AOT compilation in Angular?](#50-how-do-you-enable-aot-compilation-in-angular)
51. [How do you use Angular animations?](#51-how-do-you-use-angular-animations)
52. [How do you create a simple animation in Angular?](#52-how-do-you-create-a-simple-animation-in-angular)
53. [How do you use the `ngStyle` directive in Angular?](#53-how-do-you-use-the-ngstyle-directive-in-angular)
54. [How do you use the `ngClass` directive in Angular?](#54-how-do-you-use-the-ngclass-directive-in-angular)
55. [What is content projection in Angular?](#55-what-is-content-projection-in-angular)
56. [How do you use content projection in Angular?](#56-how-do-you-use-content-projection-in-angular)
57. [What is a structural directive in Angular?](#57-what-is-a-structural-directive-in-angular)
58. [How do you create a structural directive in Angular?](#58-how-do-you-create-a-structural-directive-in-angular)
59. [How do you use the `*ngIf` directive in Angular?](#59-how-do-you-use-the-ngif-directive-in-angular)
60. [How do you use the `*ngFor` directive in Angular?](#60-how-do-you-use-the-ngfor-directive-in-angular)
61. [How do you track items in an `*ngFor` loop in Angular?](#61-how-do-you-track-items-in-an-ngfor-loop-in-angular)
62. [How do you use the `*ngSwitch` directive in Angular?](#62-how-do-you-use-the-ngswitch-directive-in-angular)
63. [How do you create an Angular library?](#63-how-do-you-create-an-angular-library)
64. [How do you publish an Angular library?](#64-how-do-you-publish-an-angular-library)
65. [How do you use Angular Material in your project?](#65-how-do-you-use-angular-material-in-your-project)
66. [How do you add Angular Material to an Angular project?](#66-how-do-you-add-angular-material-to-an-angular-project)
67. [How do you use Angular Material components in your project?](#67-how-do-you-use-angular-material-components-in-your-project)
68. [How do you customize Angular Material themes?](#68-how-do-you-customize-angular-material-themes)
69. [How do you use the Angular CDK?](#69-how-do-you-use-the-angular-cdk)
70. [How do you create a drag-and-drop interface with Angular CDK?](#70-how-do-you-create-a-drag-and-drop-interface-with-angular-cdk)
71. [How do you use the `async` pipe in Angular?](#71-how-do-you-use-the-async-pipe-in-angular)
72. [How do you handle asynchronous operations in Angular?](#72-how-do-you-handle-asynchronous-operations-in-angular)
73. [How do you use observables in Angular?](#73

-how-do-you-use-observables-in-angular)
74. [How do you use the `subscribe` method in Angular?](#74-how-do-you-use-the-subscribe-method-in-angular)
75. [How do you use the `map` operator in Angular?](#75-how-do-you-use-the-map-operator-in-angular)
76. [How do you use the `filter` operator in Angular?](#76-how-do-you-use-the-filter-operator-in-angular)
77. [How do you use the `mergeMap` operator in Angular?](#77-how-do-you-use-the-mergemap-operator-in-angular)
78. [How do you handle multiple observables in Angular?](#78-how-do-you-handle-multiple-observables-in-angular)
79. [How do you use the `combineLatest` function in Angular?](#79-how-do-you-use-the-combinelatest-function-in-angular)
80. [How do you use the `forkJoin` function in Angular?](#80-how-do-you-use-the-forkjoin-function-in-angular)
81. [How do you test Angular components?](#81-how-do-you-test-angular-components)
82. [How do you test Angular services?](#82-how-do-you-test-angular-services)
83. [How do you write unit tests in Angular?](#83-how-do-you-write-unit-tests-in-angular)
84. [How do you write end-to-end tests in Angular?](#84-how-do-you-write-end-to-end-tests-in-angular)
85. [How do you use the Angular testing utilities?](#85-how-do-you-use-the-angular-testing-utilities)
86. [How do you mock services in Angular tests?](#86-how-do-you-mock-services-in-angular-tests)
87. [How do you mock HTTP requests in Angular tests?](#87-how-do-you-mock-http-requests-in-angular-tests)
88. [How do you use the `TestBed` utility in Angular?](#88-how-do-you-use-the-testbed-utility-in-angular)
89. [How do you configure a test module in Angular?](#89-how-do-you-configure-a-test-module-in-angular)
90. [How do you use the `async` function in Angular tests?](#90-how-do-you-use-the-async-function-in-angular-tests)
91. [How do you use the `fakeAsync` function in Angular tests?](#91-how-do-you-use-the-fakeasync-function-in-angular-tests)
92. [How do you test Angular pipes?](#92-how-do-you-test-angular-pipes)
93. [How do you test Angular directives?](#93-how-do-you-test-angular-directives)
94. [How do you test Angular forms?](#94-how-do-you-test-angular-forms)
95. [How do you debug an Angular application?](#95-how-do-you-debug-an-angular-application)
96. [How do you use the Angular DevTools?](#96-how-do-you-use-the-angular-devtools)
97. [How do you enable strict mode in Angular?](#97-how-do-you-enable-strict-mode-in-angular)
98. [How do you handle global error handling in Angular?](#98-how-do-you-handle-global-error-handling-in-angular)
99. [How do you use the `catchError` operator in Angular?](#99-how-do-you-use-the-catcherror-operator-in-angular)
100. [How do you deploy an Angular application to a web server?](#100-how-do-you-deploy-an-angular-application-to-a-web-server)

### 1. How do you create a new Angular component?
Use the Angular CLI command:
```sh
ng generate component component-name
```
Example:
```sh
ng generate component hello-world
```
This creates a new component named `HelloWorldComponent`.

## 2. How do you create a new Angular service?
Use the Angular CLI command:
```sh
ng generate service service-name
```
Example:
```sh
ng generate service data
```
This creates a new service named `DataService`.

## 3. What is Angular CLI and how do you install it?
Angular CLI is a command-line interface for Angular that helps in creating, managing, and testing Angular applications. Install it using npm:
```sh
npm install -g @angular/cli
```

## 4. How do you generate a new Angular project using Angular CLI?
Use the Angular CLI command:
```sh
ng new project-name
```
Example:
```sh
ng new my-angular-app
```

## 5. How do you start the development server in an Angular project?
Use the Angular CLI command:
```sh
ng serve
```
This starts the development server at `http://localhost:4200`.

## 6. What is the purpose of `ng serve`?
`ng serve` compiles the application and starts a web server to serve the application locally for development purposes.

## 7. How do you add routing to an Angular application?
Use the Angular CLI command when creating a new project:
```sh
ng new project-name --routing
```
Alternatively, add `RouterModule` to your app manually:
```typescript
import { RouterModule, Routes } from '@angular/router';

const routes: Routes = [
  { path: '', component: HomeComponent },
  { path: 'about', component: AboutComponent }
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```

## 8. How do you create a new route in Angular?
Define routes in your `AppRoutingModule`:
```typescript
const routes: Routes = [
  { path: 'home', component: HomeComponent },
  { path: 'about', component: AboutComponent }
];
```

## 9. How do you navigate between routes in Angular?
Use the `routerLink` directive in your templates:
```html
<a routerLink="/home">Home</a>
<a routerLink="/about">About</a>
```

## 10. What is the purpose of the `RouterModule` in Angular?
`RouterModule` provides the necessary services and directives to perform routing in Angular applications. It defines routes and sets up the navigation.

## 11. How do you pass data between components in Angular?
Use `@Input` and `@Output` decorators:
```typescript
// Parent Component
@Component({
  selector: 'app-parent',
  template: `<app-child [childData]="parentData" (childEvent)="handleChildEvent($event)"></app-child>`
})
export class ParentComponent {
  parentData = 'Data from Parent';
  handleChildEvent(event: any) {
    console.log(event);
  }
}

// Child Component
@Component({
  selector: 'app-child',
  template: `<button (click)="sendData()">Send Data</button>`
})
export class ChildComponent {
  @Input() childData: string;
  @Output() childEvent = new EventEmitter<string>();

  sendData() {
    this.childEvent.emit('Data from Child');
  }
}
```

## 12. What is an Angular module and how do you create one?
An Angular module is a container for a cohesive block of code dedicated to an application domain, a workflow, or a closely related set of capabilities. Use the Angular CLI to create a module:
```sh
ng generate module module-name
```
Example:
```sh
ng generate module user
```

## 13. How do you use Angular services to share data between components?
Create a service and inject it into the components:
```typescript
// Data Service
@Injectable({
  providedIn: 'root'
})
export class DataService {
  private data = new BehaviorSubject<string>('Initial Data');
  currentData = this.data.asObservable();

  changeData(newData: string) {
    this.data.next(newData);
  }
}

// Component A
@Component({
  selector: 'app-component-a',
  template: `<button (click)="changeData()">Change Data</button>`
})
export class ComponentA {
  constructor(private dataService: DataService) {}
  
  changeData() {
    this.dataService.changeData('Data from Component A');
  }
}

// Component B
@Component({
  selector: 'app-component-b',
  template: `{{data}}`
})
export class ComponentB {
  data: string;
  constructor(private dataService: DataService) {
    this.dataService.currentData.subscribe(data => this.data = data);
  }
}
```

## 14. What is dependency injection in Angular?
Dependency Injection (DI) is a design pattern in which a class receives its dependencies from an external source rather than creating them itself. Angular's DI system allows you to define providers and inject them into your classes.

## 15. How do you inject a service into a component in Angular?
Inject a service in the component's constructor:
```typescript
@Component({
  selector: 'app-my-component',
  template: `<p>My Component</p>`
})
export class MyComponent {
  constructor(private myService: MyService) {}
}
```

## 16. How do you use lifecycle hooks in Angular components?
Implement lifecycle hooks in your component class:
```typescript
@Component({
  selector: 'app-lifecycle',
  template: `<p>Lifecycle Hooks</p>`
})
export class LifecycleComponent implements OnInit, OnDestroy {
  ngOnInit() {
    console.log('ngOnInit called');
  }

  ngOnDestroy() {
    console.log('ngOnDestroy called');
  }
}
```

## 17. What is the purpose of the `ngOnInit` lifecycle hook in Angular?
`ngOnInit` is called once after the component's data-bound properties have been initialized. It's used for component initialization and fetching initial data.

## 18. How do you create a custom directive in Angular?


Create a directive using Angular CLI:
```sh
ng generate directive directive-name
```
Example:
```sh
ng generate directive highlight
```
Define the directive:
```typescript
@Directive({
  selector: '[appHighlight]'
})
export class HighlightDirective {
  @HostListener('mouseenter') onMouseEnter() {
    this.highlight('yellow');
  }

  @HostListener('mouseleave') onMouseLeave() {
    this.highlight(null);
  }

  private highlight(color: string) {
    this.el.nativeElement.style.backgroundColor = color;
  }

  constructor(private el: ElementRef) {}
}
```

## 19. How do you use a custom directive in an Angular template?
Apply the directive to an element in your template:
```html
<p appHighlight>Hover over this text to see the highlight effect.</p>
```

## 20. What is the purpose of the `@Input` decorator in Angular?
`@Input` decorator is used to pass data from a parent component to a child component.

## 21. How do you use the `@Output` decorator in Angular?
`@Output` decorator is used to emit an event from a child component to a parent component.
```typescript
@Output() childEvent = new EventEmitter<string>();

sendData() {
  this.childEvent.emit('Data from Child');
}
```

## 22. How do you bind a method to an event in an Angular template?
Use the event binding syntax:
```html
<button (click)="myMethod()">Click Me</button>
```
In the component class:
```typescript
myMethod() {
  console.log('Button clicked');
}
```

## 23. What is two-way data binding in Angular?
Two-way data binding allows you to synchronize data between the model and the view. It combines property binding and event binding.

## 24. How do you implement two-way data binding in Angular?
Use the `ngModel` directive:
```html
<input [(ngModel)]="myData">
```
In the component class:
```typescript
myData: string;
```

## 25. What are Angular pipes and how do you use them?
Pipes transform data in templates. Use them with the pipe (`|`) operator:
```html
<p>{{ myDate | date }}</p>
```

## 26. How do you create a custom pipe in Angular?
Create a pipe using Angular CLI:
```sh
ng generate pipe pipe-name
```
Example:
```sh
ng generate pipe exponentialStrength
```
Define the pipe:
```typescript
@Pipe({ name: 'exponentialStrength' })
export class ExponentialStrengthPipe implements PipeTransform {
  transform(value: number, exponent: string): number {
    let exp = parseFloat(exponent);
    return Math.pow(value, isNaN(exp) ? 1 : exp);
  }
}
```
Use the pipe in a template:
```html
<p>{{ 2 | exponentialStrength: 10 }}</p>
```

## 27. How do you chain pipes in Angular?
Use multiple pipes in sequence:
```html
<p>{{ myDate | date: 'short' | uppercase }}</p>
```

## 28. What is a pure pipe in Angular?
A pure pipe is only called when Angular detects a change in the input value.

## 29. What is an impure pipe in Angular?
An impure pipe is called on every change detection cycle, regardless of whether the input value changes.

## 30. How do you handle form validation in Angular?
Use built-in validators and custom validators with reactive forms or template-driven forms.

## 31. How do you create a reactive form in Angular?
Import `ReactiveFormsModule` and create a form group:
```typescript
import { FormBuilder, FormGroup } from '@angular/forms';

@Component({
  selector: 'app-reactive-form',
  template: `
    <form [formGroup]="form" (ngSubmit)="onSubmit()">
      <input formControlName="name">
      <button type="submit">Submit</button>
    </form>
  `
})
export class ReactiveFormComponent {
  form: FormGroup;

  constructor(private fb: FormBuilder) {
    this.form = this.fb.group({
      name: ['']
    });
  }

  onSubmit() {
    console.log(this.form.value);
  }
}
```

## 32. How do you create a template-driven form in Angular?
Import `FormsModule` and use the `ngModel` directive:
```html
<form #form="ngForm" (ngSubmit)="onSubmit(form)">
  <input name="name" ngModel>
  <button type="submit">Submit</button>
</form>
```
In the component class:
```typescript
onSubmit(form: NgForm) {
  console.log(form.value);
}
```

## 33. How do you use form groups in Angular?
Create a form group using `FormBuilder`:
```typescript
this.form = this.fb.group({
  name: [''],
  email: ['']
});
```

## 34. How do you use form controls in Angular?
Create form controls using `FormBuilder` or manually:
```typescript
this.name = new FormControl('');
```

## 35. How do you validate form controls in Angular?
Use built-in validators:
```typescript
this.form = this.fb.group({
  name: ['', Validators.required],
  email: ['', [Validators.required, Validators.email]]
});
```

## 36. How do you create a custom validator in Angular?
Create a function that returns a validation function:
```typescript
function forbiddenNameValidator(nameRe: RegExp): ValidatorFn {
  return (control: AbstractControl): { [key: string]: any } | null => {
    const forbidden = nameRe.test(control.value);
    return forbidden ? { forbiddenName: { value: control.value } } : null;
  };
}

this.form = this.fb.group({
  name: ['', [forbiddenNameValidator(/bob/i)]]
});
```

## 37. How do you use the `ngModel` directive in Angular?
Bind `ngModel` to an input:
```html
<input [(ngModel)]="myData">
```

## 38. How do you handle form submission in Angular?
Bind a method to the form's submit event:
```html
<form (ngSubmit)="onSubmit()">
  <!-- form controls -->
  <button type="submit">Submit</button>
</form>
```
In the component class:
```typescript
onSubmit() {
  console.log(this.form.value);
}
```

## 39. How do you reset a form in Angular?
Use the `reset` method:
```typescript
this.form.reset();
```

## 40. What is the purpose of the `HttpClient` module in Angular?
`HttpClient` is used to make HTTP requests to a backend service.

## 41. How do you make HTTP requests in Angular?
Inject `HttpClient` and use its methods:
```typescript
constructor(private http: HttpClient) {}

getData() {
  this.http.get('url').subscribe(data => console.log(data));
}
```

## 42. How do you handle HTTP errors in Angular?
Use `catchError` operator:
```typescript
import { catchError } from 'rxjs/operators';

this.http.get('url').pipe(
  catchError(error => {
    console.error('Error occurred:', error);
    return throwError(error);
  })
);
```

## 43. How do you use interceptors in Angular?
Create an interceptor service:
```typescript
@Injectable()
export class MyInterceptor implements HttpInterceptor {
  intercept(req: HttpRequest<any>, next: HttpHandler): Observable<HttpEvent<any>> {
    const modifiedReq = req.clone({ headers: req.headers.set('Authorization', 'Bearer token') });
    return next.handle(modifiedReq);
  }
}
```
Provide the interceptor:
```typescript
providers: [
  { provide: HTTP_INTERCEPTORS, useClass: MyInterceptor, multi: true }
]
```

## 44. How do you implement authentication in an Angular application?
Use a combination of services, route guards, and interceptors.

## 45. How do you implement route guards in Angular?
Create a guard service:
```typescript
@Injectable({
  providedIn: 'root'
})
export class AuthGuard implements CanActivate {
  canActivate(): boolean {
    // logic to determine if route can be activated
    return true;
  }
}
```
Apply the guard to routes:
```typescript
const routes: Routes = [
  { path: 'protected', component: ProtectedComponent, canActivate: [AuthGuard] }
];
```

## 46. How do you create a canActivate guard in Angular?
Create a service that implements `CanActivate`:
```typescript
@Injectable({
  providedIn: 'root'
})
export class AuthGuard implements CanActivate {
  canActivate(route: ActivatedRouteSnapshot, state: RouterStateSnapshot): boolean {
    // logic to determine if route can be activated
    return true;
  }
}
```

## 47. How do you use lazy loading in Angular?
Define routes with the `loadChildren` property:
```typescript
const routes: Routes = [
  { path: 'feature', loadChildren: () => import('./feature/feature.module').then(m => m.FeatureModule) }
];
```

## 48. How do you optimize an Angular application for production?
Use the Angular CLI to build the application with the `--prod` flag:
```sh
ng build --prod
```

## 49. What is Ahead-of-Time (AOT) compilation in Angular?
AOT compilation compiles Angular templates and components at build time instead of runtime, resulting in faster rendering.

## 50. How do you enable AOT compilation in Angular?
Use the Angular CLI to build the application with the `--aot` flag:
```sh
ng

 build --aot
```

## 51. How do you use environment variables in Angular?
Define environment variables in the `src/environments` folder:
```typescript
export const environment = {
  production: false,
  apiUrl: 'http://localhost:3000'
};
```
Access them in your application:
```typescript
import { environment } from '../environments/environment';

const apiUrl = environment.apiUrl;
```

## 52. How do you create a custom environment in Angular?
Create a new environment file in the `src/environments` folder:
```typescript
export const environment = {
  production: false,
  apiUrl: 'http://localhost:3000'
};
```
Add the environment to the `angular.json` file:
```json
"configurations": {
  "custom": {
    "fileReplacements": [{
      "replace": "src/environments/environment.ts",
      "with": "src/environments/environment.custom.ts"
    }]
  }
}
```

## 53. How do you use Angular animations?
Import `BrowserAnimationsModule` and define animations in your component:
```typescript
import { trigger, state, style, transition, animate } from '@angular/animations';

@Component({
  selector: 'app-animations',
  template: `<div [@myAnimation]="state" (click)="toggleState()">Animate me</div>`,
  animations: [
    trigger('myAnimation', [
      state('state1', style({ backgroundColor: 'red' })),
      state('state2', style({ backgroundColor: 'blue' })),
      transition('state1 <=> state2', [animate('0.5s')])
    ])
  ]
})
export class AnimationsComponent {
  state = 'state1';

  toggleState() {
    this.state = this.state === 'state1' ? 'state2' : 'state1';
  }
}
```

## 54. How do you create a custom Angular animation?
Define a custom animation using `trigger`, `state`, `style`, `transition`, and `animate`:
```typescript
trigger('customAnimation', [
  state('start', style({ opacity: 1 })),
  state('end', style({ opacity: 0 })),
  transition('start => end', [animate('1s')]),
  transition('end => start', [animate('1s')])
]);
```

## 55. How do you handle user input in Angular?
Use event binding and template reference variables:
```html
<input #inputElement (input)="onInput(inputElement.value)">
```
In the component class:
```typescript
onInput(value: string) {
  console.log(value);
}
```

## 56. How do you use the `@ViewChild` decorator in Angular?
Use `@ViewChild` to get a reference to a child component or directive:
```typescript
@ViewChild('inputElement') inputElement: ElementRef;

ngAfterViewInit() {
  console.log(this.inputElement.nativeElement.value);
}
```

## 57. How do you use the `@ContentChild` decorator in Angular?
Use `@ContentChild` to get a reference to projected content:
```typescript
@ContentChild('contentElement') contentElement: ElementRef;

ngAfterContentInit() {
  console.log(this.contentElement.nativeElement.textContent);
}
```

## 58. How do you use the `Renderer2` service in Angular?
Use `Renderer2` to safely manipulate the DOM:
```typescript
constructor(private renderer: Renderer2, private el: ElementRef) {}

ngOnInit() {
  this.renderer.setStyle(this.el.nativeElement, 'color', 'blue');
}
```

## 59. How do you create a custom event in Angular?
Use `@Output` and `EventEmitter` to create custom events:
```typescript
@Output() customEvent = new EventEmitter<string>();

triggerEvent() {
  this.customEvent.emit('Custom event triggered');
}
```

## 60. How do you handle file uploads in Angular?
Use the `FormData` API and `HttpClient` to upload files:
```typescript
onFileSelected(event: Event) {
  const file = (event.target as HTMLInputElement).files[0];
  const formData = new FormData();
  formData.append('file', file);
  
  this.http.post('upload-url', formData).subscribe(response => {
    console.log(response);
  });
}
```

## 61. How do you implement internationalization (i18n) in Angular?
Use Angular's `@angular/localize` package and translation files.

## 62. How do you set up Angular Material in an Angular project?
Install Angular Material:
```sh
ng add @angular/material
```
Import Angular Material modules in your application module:
```typescript
import { MatButtonModule } from '@angular/material/button';

@NgModule({
  imports: [
    MatButtonModule
  ]
})
export class AppModule { }
```

## 63. How do you use Angular Material components?
Use Angular Material components in your templates:
```html
<button mat-button>Click me!</button>
```

## 64. How do you customize Angular Material themes?
Create a custom theme in your styles file:
```scss
@import '~@angular/material/theming';
@include mat-core();

$custom-primary: mat-palette($mat-indigo);
$custom-accent: mat-palette($mat-pink, A200, A100, A400);
$custom-theme: mat-light-theme($custom-primary, $custom-accent);

@include angular-material-theme($custom-theme);
```

## 65. How do you use Angular Material dialogs?
Import `MatDialogModule` and create a dialog component:
```typescript
@Component({
  selector: 'app-dialog',
  template: `<h1 mat-dialog-title>Dialog</h1>`
})
export class DialogComponent {}

openDialog() {
  this.dialog.open(DialogComponent);
}
```

## 66. How do you use Angular Material tabs?
Import `MatTabsModule` and use the `mat-tab` component:
```html
<mat-tab-group>
  <mat-tab label="Tab 1">Content 1</mat-tab>
  <mat-tab label="Tab 2">Content 2</mat-tab>
</mat-tab-group>
```

## 67. How do you use Angular Material table?
Import `MatTableModule` and use the `mat-table` component:
```html
<table mat-table [dataSource]="dataSource">
  <ng-container matColumnDef="name">
    <th mat-header-cell *matHeaderCellDef> Name </th>
    <td mat-cell *matCellDef="let element"> {{element.name}} </td>
  </ng-container>
  <!-- other columns -->
</table>
```

## 68. How do you create a custom Angular Material component?
Create a custom component and style it using Angular Material theming.

## 69. How do you use the Angular Material `mat-icon` component?
Import `MatIconModule` and use the `mat-icon` component:
```html
<mat-icon>home</mat-icon>
```

## 70. How do you use Angular Flex Layout?
Install Angular Flex Layout:
```sh
npm install @angular/flex-layout
```
Use the layout directives in your templates:
```html
<div fxLayout="row" fxLayoutAlign="space-around center">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

## 71. How do you set up Angular Universal for server-side rendering (SSR)?
Use the Angular CLI to generate a Universal app:
```sh
ng add @nguniversal/express-engine
```
Build and serve the application:
```sh
npm run build:ssr
npm run serve:ssr
```

## 72. How do you use observables in Angular?
Use `HttpClient` methods, which return observables:
```typescript
this.http.get('url').subscribe(data => console.log(data));
```

## 73. How do you use the `subscribe` method in Angular?
Call `subscribe` on an observable to execute it:
```typescript
this.http.get('url').subscribe(
  data => console.log('Success', data),
  error => console.error('Error', error)
);
```

## 74. How do you use the `map` operator in Angular?
Use `map` to transform the response:
```typescript
this.http.get('url').pipe(
  map(response => response['data'])
).subscribe(data => console.log(data));
```

## 75. How do you use the `filter` operator in Angular?
Use `filter` to filter the response:
```typescript
this.http.get('url').pipe(
  filter(response => response['status'] === 'success')
).subscribe(data => console.log(data));
```

## 76. How do you use the `mergeMap` operator in Angular?
Use `mergeMap` to flatten higher-order observables:
```typescript
this.http.get('url1').pipe(
  mergeMap(response1 => this.http.get(`url2/${response1['id']}`))
).subscribe(data => console.log(data));
```

## 77. How do you handle multiple observables in Angular?
Use `forkJoin`, `combineLatest`, or `zip` to handle multiple observables:
```typescript
forkJoin([
  this.http.get('url1'),
  this.http.get('url2')
]).subscribe(([response1, response2]) => {
  console.log(response1, response2);
});
```

## 78. How do you use the `combineLatest` function in Angular?
Combine multiple observables and emit the latest values:
```typescript
combineLatest([
  this.http.get('url1'),
  this.http.get('url2')
]).subscribe(([response1

, response2]) => {
  console.log(response1, response2);
});
```

## 79. How do you use the `switchMap` operator in Angular?
Use `switchMap` to switch to a new observable:
```typescript
this.http.get('url1').pipe(
  switchMap(response1 => this.http.get(`url2/${response1['id']}`))
).subscribe(data => console.log(data));
```

## 80. How do you unsubscribe from an observable in Angular?
Call the `unsubscribe` method on the subscription:
```typescript
const subscription = this.http.get('url').subscribe(data => console.log(data));

subscription.unsubscribe();
```

## 81. How do you use the `take` operator in Angular?
Use `take` to complete the observable after a number of emissions:
```typescript
this.http.get('url').pipe(
  take(1)
).subscribe(data => console.log(data));
```

## 82. How do you use the `debounceTime` operator in Angular?
Use `debounceTime` to delay emissions:
```typescript
fromEvent(this.input.nativeElement, 'input').pipe(
  debounceTime(300)
).subscribe(event => console.log(event));
```

## 83. How do you use the `distinctUntilChanged` operator in Angular?
Use `distinctUntilChanged` to ignore duplicate values:
```typescript
fromEvent(this.input.nativeElement, 'input').pipe(
  distinctUntilChanged()
).subscribe(event => console.log(event));
```

## 84. How do you use the `share` operator in Angular?
Use `share` to share the observable among multiple subscribers:
```typescript
const sharedObservable = this.http.get('url').pipe(
  share()
);

sharedObservable.subscribe(data => console.log('Subscriber 1', data));
sharedObservable.subscribe(data => console.log('Subscriber 2', data));
```

## 85. How do you create a custom observable in Angular?
Use the `Observable` constructor to create a custom observable:
```typescript
const customObservable = new Observable(observer => {
  observer.next('Hello');
  observer.complete();
});

customObservable.subscribe(data => console.log(data));
```

## 86. How do you use the `Subject` class in Angular?
Use `Subject` to multicast to multiple observers:
```typescript
const subject = new Subject<string>();

subject.subscribe(data => console.log('Subscriber 1', data));
subject.subscribe(data => console.log('Subscriber 2', data));

subject.next('Hello');
```

## 87. How do you use the `BehaviorSubject` class in Angular?
Use `BehaviorSubject` to emit the latest value to new subscribers:
```typescript
const behaviorSubject = new BehaviorSubject<string>('Initial value');

behaviorSubject.subscribe(data => console.log('Subscriber 1', data));
behaviorSubject.next('Updated value');
behaviorSubject.subscribe(data => console.log('Subscriber 2', data));
```

## 88. How do you use the `ReplaySubject` class in Angular?
Use `ReplaySubject` to replay the specified number of emitted values to new subscribers:
```typescript
const replaySubject = new ReplaySubject<string>(2);

replaySubject.next('Value 1');
replaySubject.next('Value 2');
replaySubject.next('Value 3');

replaySubject.subscribe(data => console.log('Subscriber', data));
```

## 89. How do you use the `AsyncSubject` class in Angular?
Use `AsyncSubject` to emit the last value only when the observable completes:
```typescript
const asyncSubject = new AsyncSubject<string>();

asyncSubject.subscribe(data => console.log('Subscriber 1', data));
asyncSubject.next('Value 1');
asyncSubject.next('Value 2');
asyncSubject.complete();
asyncSubject.subscribe(data => console.log('Subscriber 2', data));
```

## 90. How do you handle state management in Angular?
Use services, `BehaviorSubject`, or state management libraries like NgRx.

## 91. How do you set up NgRx in an Angular project?
Install NgRx:
```sh
ng add @ngrx/store
```
Create a feature state:
```typescript
interface AppState {
  count: number;
}

const initialState: AppState = {
  count: 0
};

const countReducer = createReducer(
  initialState,
  on(increment, state => ({ ...state, count: state.count + 1 })),
  on(decrement, state => ({ ...state, count: state.count - 1 }))
);

@NgModule({
  imports: [
    StoreModule.forRoot({ count: countReducer })
  ]
})
export class AppModule { }
```

## 92. How do you use the `Store` service in Angular?
Inject `Store` and dispatch actions or select state:
```typescript
constructor(private store: Store<{ count: number }>) {}

increment() {
  this.store.dispatch(increment());
}

decrement() {
  this.store.dispatch(decrement());
}

ngOnInit() {
  this.store.select('count').subscribe(count => console.log(count));
}
```

## 93. How do you use NgRx effects in Angular?
Install NgRx Effects:
```sh
ng add @ngrx/effects
```
Create an effect:
```typescript
@Injectable()
export class MyEffects {
  loadItems$ = createEffect(() =>
    this.actions$.pipe(
      ofType(loadItems),
      mergeMap(() => this.myService.getItems().pipe(
        map(items => loadItemsSuccess({ items })),
        catchError(() => of(loadItemsFailure()))
      ))
    )
  );

  constructor(private actions$: Actions, private myService: MyService) {}
}
```
Provide the effect:
```typescript
@NgModule({
  imports: [
    EffectsModule.forRoot([MyEffects])
  ]
})
export class AppModule { }
```

## 94. How do you use the NgRx router store?
Install NgRx Router Store:
```sh
ng add @ngrx/router-store
```
Import `StoreRouterConnectingModule`:
```typescript
@NgModule({
  imports: [
    StoreRouterConnectingModule.forRoot()
  ]
})
export class AppModule { }
```

## 95. How do you debug NgRx applications?
Use the Redux DevTools extension and log actions or state changes.

## 96. How do you use Angular CLI to create a new Angular project?
Use the `ng new` command:
```sh
ng new project-name
```

## 97. How do you serve an Angular application locally?
Use the `ng serve` command:
```sh
ng serve
```

## 98. How do you build an Angular application for production?
Use the `ng build` command with the `--prod` flag:
```sh
ng build --prod
```

## 99. How do you generate a new component using Angular CLI?
Use the `ng generate component` command:
```sh
ng generate component component-name
```

## 100. How do you generate a new service using Angular CLI?
Use the `ng generate service` command:
```sh
ng generate service service-name
```
