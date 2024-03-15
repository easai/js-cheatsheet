JavaScript/TypeScript: General
================================

## Contents

  - [Apply an array as function arguments](general.md#apply-an-array-as-function-arguments)

## Apply an array as function arguments

Apply an array as function arguments.<br />
Example:

```sql
fn(...args);
```
Source: [interval-cancellation](https://github.com/easai/interval-cancellation/blob/main/index.js)

Or use apply().
```sql
const fn = (x) => x * 2;
const args = [4];

var res=fn.apply(args);
console.log(res);
```