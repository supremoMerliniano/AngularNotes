
Is a structural directive in Angular that conditionally renders or removes elements from the DOM based on an expression's truthy or falsy value.

**Example of use:**

1. **Component File (app.component.ts)**:

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  isLoggedIn: boolean = false;
}
```

2. **HTML Template File (app.component.html)**:

```html
<div *ngIf="isLoggedIn">
  <p>Welcome, User!</p>
</div>

<div *ngIf="!isLoggedIn">
  <p>Please log in to continue.</p>
</div>
```
