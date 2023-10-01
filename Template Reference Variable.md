
A template reference variable (often referred to as "ref" or "hash variable") is a way to get a reference to a DOM element or an Angular directive in your template. It allows you to access and manipulate the element or directive from your component code.

**Syntax**:
- The syntax to create a template reference variable is `#variableName`.
- You can add a template reference variable to almost any HTML element, including components, directives, and native HTML elements.

```html
<input #myInput type="text">
```