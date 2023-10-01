Is a structural directive in Angular that allows you to conditionally render elements based on a specified value.

Here's an example of how to use ngSwitch in Angular:

1. Component File (`app.component.ts`):

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  fruit: string = 'banana';
}
```


2. HTML Template File (`app.component.html`):

```html
<div [ngSwitch]="fruit">
  <div *ngSwitchCase="'apple'">You selected an apple.</div>
  <div *ngSwitchCase="'banana'">You selected a banana.</div>
  <div *ngSwitchCase="'cherry'">You selected a cherry.</div>
  <div *ngSwitchDefault>Select a fruit.</div>
</div>
```
