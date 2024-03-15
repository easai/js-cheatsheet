JavaScript/TypeScript: Testing
================================

## Contents

  - [Detect exceptions](testing.md#detect-exceptions)

## Detect exceptions

Test if the function emits an exception.<br />
Example:

```sql
    expect(()=>{c.divide(0)}).toThrow(Error);
    expect(()=>{c.divide(0)}).toThrow("Division by zero is not allowed");
```
Source: [method-chaining](https://github.com/easai/method-chaining)
