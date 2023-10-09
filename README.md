
- [Array-js](#ArrayDeclaraton)
  - [ArrayDeclaraton](#ArrayDeclaraton)
- [MethodsofArray](#MethodsofArray)
  - [PushPop](#PushPop)
  - [ShiftUshift](#ShiftUshift)
  - [SlicSplice](#SlicSplice)
  - [ConcatRestOperator](#ConcatRestOperator)
  - [Flat](#Flat)
  - [Map](#Map)
  - [Filter](#Filter)
  - [ArrayOf](#ArrayOf)


### ArrayDeclaration

```js
  
const arr1 = [1, 2, 3, 4, 5, 6];

const arr2 = ['css', 'javascript', 'phython'];

const arr3 = new Array(2, 'babu', 8, 'bootstrap', true);

```

### MethodsofArray

## PushPop
```js
arr1.push(8, 10); // push method add items into end of the array
arr1.pop();  // pop method remove last item from the array
 console.log(arr1);
```

## ShiftUshift
```js

arr2.unshift('abc', 'html'); // add items into start of the array
arr2.shift(); // remove first item from the array
 console.log(arr2);
```
## SlicSplice

```js
const sArr = [1, 2, 3, 4, 5, 6];
console.log(sArr);

const sliceArr = sArr.slice(1, 4); // slice method will create new array but orginial will remain same
console.log(sliceArr);
console.log(sArr);

const spliceArr =  sArr.splice(1, 3);  // splice method Will create new array and items are also remove from the original array
console.log(spliceArr);
console.log(sArr);

```

## ConcatRestOperator

```js
const batter = ['Shakib', 'Tamim', 'Mushfiq', 'Mahmudullah', 'Liton'];
const bowler = ['Fizz', 'Miraz', 'Taskin', 'Shoriful'];

const fullTeam = batter.concat(bowler);
const fullTeam = [...batter, ...bowler];

// console.log(fullTeam);  // ['Shakib', 'Tamim', 'Mushfiq', 'Mahmudullah', 'Liton', 'Fizz', 'Miraz', 'Taskin', 'Shoriful']
```
## Flat

```js
const flatArr1 = [1, 2, 3,[4, 5, 6]];
console.log(flatArr1.flat());

const flatArr2 = [1, 2, [3, 4, [5, 6, [7, 8, [9, 10]]]]];

console.log(flatArr2.flat()); // [ 1, 2, 3, 4, [ 5, 6, [ 7, 8, [Array] ] ] ]
console.log(flatArr2.flat(2));  // [ 1, 2, 3, 4, 5, 6, [ 7, 8, [ 9, 10 ] ] ]
console.log(flatArr2.flat(3));  // [ 1, 2, 3, 4, 5, 6, 7, 8, [ 9, 10 ] ]
console.log(flatArr2.flat(Infinity)); // [ 1, 2, 3, 4,  5, 6, 7, 8, 9, 10 ]
```
## Map

```js
const ranNum = [2, 4, 7, 9];
let total = 0;

const addRanNum = ranNum.map(num => 
    total += num 
 );
console.log(addRanNum); // [ 2, 6, 13, 22 ]
console.log(total); // 22

const multiRanNum = ranNum.map(num => num * num);
console.log(multiRanNum); //[ 4, 16, 49, 81 ]
```
## Filter
```js
const filterArr = [-3, -2, -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13];

const fitteredArr = filterArr.filter(num => num > 8);
console.log(fitteredArr); // [ 9, 10, 11, 12, 13 ]

```
## ArrayOf

```js
const score1 = 9;
const score2 = 99;
const score3 = 999;
const score4 = 9999;

const createArr = Array.of(score1,score2, score3, score4);
console.log(createArr);  // [ 9, 99, 999, 9999 ]

```


