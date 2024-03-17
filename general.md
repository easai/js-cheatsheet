JavaScript/TypeScript: General
================================

## Contents

  - [Array as arguments](general.md#array-as-arguments)
  - [Extend a class](general.md#extend-a-class)
  - [Add a method](general.md#add-a-method)
  - [Custom sort](general.md#custom-sort)
  - [Process each element](general.md#process-each-element)

## Array as arguments

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


## Custom sort

Define the customized sort function.<br />
Example:

```js
    sortedArray=arr.sort((a,b)=>fn(a)-fn(b));
```
Source: [sort-by](https://github.com/easai/sort-by/blob/main/index.js)


## Process each element

Process each element of an array.<br />
Example:

```js
    arr.forEach((x,i)=>{
        if(fn(x,i)){
            newArray.push(x);
        }
    });
```
Source: [filter-elements-js](https://github.com/easai/filter-elements-js/blob/main/script.js)

