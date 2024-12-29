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

