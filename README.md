
-[array](#array)

### array-js

```js
  // Array Declaration

const arr1 = [1, 2, 3, 4, 5, 6];

const arr2 = ['css', 'javascript', 'phython'];

const arr3 = new Array(2, 'babu', 8, 'bootstrap', true);

// Methods of Array

arr1.push(8, 10); // push method add items into end of the array
arr1.pop();  // pop method remove last item from the array
// console.log(arr1);

arr2.unshift('abc', 'html'); // add items into start of the array
arr2.shift(); // remove first item from the array
// console.log(arr2);

const sArr = [1, 2, 3, 4, 5, 6];
console.log(sArr);

const sliceArr = sArr.slice(1, 4); // slice method will create new array but orginial will remain same
console.log(sliceArr);
console.log(sArr);

const spliceArr =  sArr.splice(1, 3);  // splice method Will create new array and items are also remove from the original array
console.log(spliceArr);
console.log(sArr);

```
