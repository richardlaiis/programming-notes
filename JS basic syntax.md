# Javascript basic syntax
## array

`slice`: 取出陣列 \[n, m) 區間的內容

```js
var arr = [1, 3, 5, 7, 8];
var arr1 = arr.slice(2, 4);
console.log(arr1); // [5, 7]
```

`splice`: 插入/刪除第 i 項的元素

```js
var ary = arr.splice(n, m, a, b, c, ...);
// n: starting index
// m: 刪除個數，若為 0 就是插入
// a, b, c: 欲插入的元素
```

## function

#### callback

```js
function calc(x, y, callback) {
	return callback(x, y);
};
function foo(x, y) {
	return (x == y);
};
console.log(calc(5, 6, foo));
```

callback function 可以避免 javascript asynchronous 導致的一些問題。
## Object

