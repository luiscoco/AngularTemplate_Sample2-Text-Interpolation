# interpolation

In Angular, interpolation refers to a way of binding data from the component to the HTML template. It allows you to display dynamic values in the template by embedding them within curly braces ({{ }}).

Here's a simple example to illustrate interpolation in Angular:

In your component TypeScript file (e.g., app.component.ts), define a variable named name with a value:

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  template: `
    <h1>Welcome, {{ name }}!</h1>
  `
})
export class AppComponent {
  name = 'John';
}
```

In the above code, we have a component named AppComponent with a property name set to 'John'.

In the associated HTML template (e.g., app.component.html), you can use interpolation to display the name property:

```typescript
<h1>Welcome, {{ name }}!</h1>
```

When the application runs, the template will be rendered with the value of name interpolated within the double curly braces. In this case, the output will be:

Welcome, John!

You can also perform basic expressions and calculations within interpolation. Here's an example that demonstrates this:

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  template: `
    <p>The sum of 2 and 3 is {{ 2 + 3 }}</p>
    <p>The length of the word "Angular" is {{ 'Angular'.length }}</p>
  `
})
export class AppComponent { }
```

In the above code, we directly perform addition and access the length property of a string within the interpolation.

When the application runs, the template will be rendered as follows:

The sum of 2 and 3 is 5
The length of the word "Angular" is 7

These are some basic examples of how interpolation works in Angular. It allows you to display dynamic data and perform simple expressions within your templates.



