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
