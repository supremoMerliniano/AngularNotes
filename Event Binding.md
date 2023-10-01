
**Event binding** in _Angular_ allows you to listen for and respond to events triggered by user interactions or by the application itself. It's a way to capture user input, such as clicks, keystrokes, mouse movements, and more.

You use parentheses `()` to bind an event in the template to a method in your component.

## Commonly used events

Here are some of the most commonly used events in Angular:

1. **`Click Event:`** This event is triggered when a user clicks on an element.
2. **`Input Event:`** This event is triggered when the value of an input element changes.
3. **`Mouse Events (e.g., mouseover, mouseout, mouseenter, mouseleave):`** These events are triggered by mouse actions.
4. **`Key Events (e.g., keyup, keydown, keypress):`** These events are triggered by keyboard actions.
5. **`Form Events (e.g., submit, reset):`** These events are triggered when a form is submitted or reset.
6. **`Change Event:`** This event is triggered when the value of a select element changes.
7. **`Focus and Blur Events (e.g., focus, blur):`** These events are triggered when an element gains or loses focus.
8. **`Custom Events:`** You can create and trigger your own custom events for communication between components

### Click event

1. `app.component.ts`:
```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  handleInputChange(event: any) {
    console.log('Input value:', event.target.value);
  }
}
```

2. `app.component.html`:
```html
<input (input)="handleInputChange($event)" placeholder="Type something">
```

## Input Events

1. Component File (app.component.ts):
```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  handleInputChange(event: any) {
    console.log('Input value:', event.target.value);
  }
}
```

2. HTML Template File (app.component.html):
```typescript
<input (input)="handleInputChange($event)" placeholder="Type something">
```

### Mouse events

1. `app.component.ts`:
```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  handleInputChange(event: any) {
    console.log('Input value:', event.target.value);
  }
}
```

2. `app.component.html`:
```html
<input (input)="handleInputChange($event)" placeholder="Type something">
```
