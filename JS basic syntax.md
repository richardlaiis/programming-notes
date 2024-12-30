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

```js
function College(name, rank, loc) {
	this.name = name;
	this.rank = rank;
	this.loc = loc;
	this.print = function() {
		console.log(this.name + "is ranked as" + this.rank);
	}
};
var a = new College("NTU", 69, "Taiwan");
console.log(a);
a.print();
delete a.loc; // delete a property
a["tmp"] = 123; // add a property
console.log(a);
```

JSON 物件的基礎操作
```js
var json1 = {"year": 2025, "location": "Taiwan", "party": "DPP"};
console.log(json1);
json1 = JSON.stringify(json1); // convert a json object to a string
console.log(json1);

json1 = JSON.parse(json1); // parse a string into a json object
console.log(json1);
```

## time

```js
var i = 0;
var timer = setInterval(
    function clock() {
        console.log(i);
        i++;
        if(i == 3) {
            clearInterval(timer); // stop the loop
        }
    },
    1000 // (ms)
); // execute specific function forever on a regular frequency

var timer2 = setTimeout(
    function clock() {
        console.log("Hello NTU CSIE");
    },
    1000
); // only execute one time
//clearTimeout(timer2); // clear timer for timeout
```