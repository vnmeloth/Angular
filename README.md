# Angular
Angular Interview Questions
## 1. What is the difference between pure and impure pipe?
In the context of Angular, pipes are used to transform data in templates. Pipes can be classified into two types: pure and impure. The primary difference between pure and impure pipes lies in how and when they trigger change detection and update their output.

### Pure Pipes

**Characteristics:**
1. **Deterministic Behavior:** Pure pipes return the same output for the same input.
2. **Change Detection:** Pure pipes are only re-evaluated when the input reference changes.
3. **Performance:** They are more efficient because they do not require frequent checks.
4. **Examples:** Built-in pipes like `DatePipe`, `UpperCasePipe`, and `CurrencyPipe` are pure pipes.

**Use Case:**
- Use pure pipes when the transformation logic is stateless and depends solely on the input value.

**Code Example:**
```typescript
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({
  name: 'purePipe'
})
export class PurePipe implements PipeTransform {
  transform(value: any, ...args: any[]): any {
    // Transformation logic here
    return value;
  }
}
```

### Impure Pipes

**Characteristics:**
1. **Non-Deterministic Behavior:** Impure pipes may return different outputs for the same input.
2. **Change Detection:** Impure pipes are re-evaluated on every change detection cycle, even if the input reference has not changed.
3. **Performance:** They are less efficient due to frequent re-evaluation.
4. **Examples:** Custom pipes that need to handle more complex logic, such as filtering arrays, may be impure.

**Use Case:**
- Use impure pipes when the transformation logic depends on external factors or when the input is a complex object that changes frequently.

**Code Example:**
```typescript
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({
  name: 'impurePipe',
  pure: false
})
export class ImpurePipe implements PipeTransform {
  transform(value: any, ...args: any[]): any {
    // Transformation logic here
    return value;
  }
}
```

**Key Difference:**
- **Pure Pipe:** Only re-evaluated when the input reference changes, leading to better performance.
- **Impure Pipe:** Re-evaluated on every change detection cycle, useful for more complex transformations but can impact performance.

## 2. Chaining Pipes
In Angular, you can chain pipes by applying multiple pipes in sequence within the template. Each pipe takes the output of the previous pipe as its input. This allows you to perform multiple transformations on the data in a readable and concise manner.

### Syntax
To chain pipes, you use the pipe character (`|`) between each pipe.

### Example
Let's say you have a string that you want to transform in several ways: convert it to uppercase, then slice a portion of it, and finally format it.

**Template:**
```html
<!-- Assuming 'message' is a string variable in your component -->
{{ message | uppercase | slice:0:5 }}
```

**Explanation:**
1. **Uppercase Pipe (`uppercase`):** Converts the entire string to uppercase.
2. **Slice Pipe (`slice:0:5`):** Extracts a substring from index 0 to 5.

### More Complex Example
Consider a scenario where you have a date that you want to format and then apply a custom pipe to further transform it.

**Component:**
```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  template: `
    <p>{{ today | date:'fullDate' | customDatePipe }}</p>
  `
})
export class AppComponent {
  today: number = Date.now();
}
```

**Custom Pipe:**
```typescript
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({
  name: 'customDatePipe'
})
export class CustomDatePipe implements PipeTransform {
  transform(value: string, ...args: any[]): string {
    // Custom transformation logic here
    return `Transformed Date: ${value}`;
  }
}
```

**Explanation:**
1. **Date Pipe (`date:'fullDate'`):** Formats the date to a full date string (e.g., "Wednesday, July 7, 2023").
2. **Custom Pipe (`customDatePipe`):** Further transforms the formatted date string as defined in the custom pipe logic.

### Summary
Chaining pipes in Angular is a powerful way to apply multiple transformations to data in a template. By separating concerns into individual pipes, you can create reusable and composable transformations that keep your templates clean and easy to understand.
