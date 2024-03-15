JavaScript/TypeScript: General
================================

## Contents

  - [Apply an array as function arguments](general.md#apply-an-array-as-function-arguments)
  - [Extend a class](general.md#extend-a-class)
  - [Add a method](general.md#add-a-method)

## Apply an array as function arguments

Apply an array as function arguments.<br />
Example:

```js
fn(...args);
```
Source: [interval-cancellation](https://github.com/easai/interval-cancellation/blob/main/index.js)

Or use apply().
```js
const fn = (x) => x * 2;
const args = [4];

var res=fn.apply(args);
console.log(res);
```

## Extend a class

Extend (Inherit) a class.<br />
Example:

```js
class ArrayWrapper extends Array {
  constructor(nums) {
    super();
    for (var i = 0; i < nums.length; i++) {
      this.push(nums[i]);
    }
  }
}
```
Source: [array-wrapper](https://github.com/easai/array-wrapper/blob/main/script.js)


## Add a method

Add a method to an existing class.<br />
Example:

```js
Array.prototype.last = function () {
  var res = -1;
  var nLen = this.length;
  if (nLen > 0) {
    res = this.at(nLen - 1);
  }
  return res;
};
```
Source: [array-prototype-last](https://github.com/easai/array-prototype-last/blob/main/index.js)