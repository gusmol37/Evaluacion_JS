# Quiz - YDKJS: Up & Going 2/3
​
## Chapter 2: Into JavaScript
​
### Self-Evaluation
​
#### Section: Values & Types
​
---
​
##### 1. Name the 7 built-in types available in JavaScript.
​
> _null, undefined, boolean, number, string, object_
​
##### 2. Name the two ways to access object properties.
​
> 1. objeto.propiedad
  2. objeto[propiedad]
​
##### 3. Typeof. Look at the following snippets and write what would be the ouput.
​
###### Snippet #1
​
```js
console.log(typeof a);
var a;
```
​
> _yundefinede_
​
###### Snippet #2
​
```js
console.log(typeof "hello world");
```
​
> _string_
​
###### Snippet #3
​
```js
console.log(typeof false);
```
​
> _boolean_
​
###### Snippet #4
​
```js
console.log(typeof 21);
```
​
> _number_
​
###### Snippet #5
​
```js
console.log(typeof null);
```
​
> _object_
​
###### Snippet #6
​
```js
console.log(typeof undefined);
```
​
> _undefined_
​
###### Snippet #7
​
```js
console.log(typeof { name: "John" });
```
​
> _object_
​
###### Snippet #8
​
```js
console.log(typeof typeof 42);
```
​
> _string_
​
###### Snippet #9
​
```js
console.log(typeof 3.1416);
```
​
> _number_
​
###### Snippet #10
​
```js
console.log(typeof "10");
```
​
> _string_
​
###### Snippet #11
​
```js
var person = {
  name: "Peter",
  age: 40
};
​
console.log(typeof person.name);
console.log(typeof person.age);
console.log(typeof person.lastName);
```
​
> Peter 40 undefined
​
###### Snippet #12
​
```js
console.log(typeof []);
```
​
> _object_
​
###### Snippet #13
​
```js
console.log(typeof ["Hello", 20, true][2]);
```
​
> _boolean_
​
###### Snippet #14
​
```js
console.log(typeof ["Hello", 20, true][3]);
```
​
> _undefined_
​
###### Snippet #15
​
```js
console.log(typeof { a: 2 }["a"]);
```
​
> _number_
​
###### Snippet #16
​
```js
var index = "c";
console.log({ a: 1, b: 2, c: 3 }[index]);
```
​
> _your answer here_
​
###### Snippet #17
​
```js
console.log({ x: 100, y: 200 }.x);
```
​
> _your answer here_
​
###### Snippet #18
​
```js
function getX (point) {
  return point.x;
}
​
getX.PI = '3.1416';
​
console.log(typeof getX);
console.log(typeof getX({ x: 34, y: 54 }));
console.log(typeof getX.PI);
```
​
> _your answer here_
​
###### Snippet #19
​
```js
var n = "47";
console.log(typeof n);
console.log(typeof Number(n));
```
​
> string
  number
​
###### Snippet #20
​
```js
var n = "47";
console.log(typeof (n * 2));
```
​
> _number_
​
##### 4. Coercion. Label the following code snippets with `explicit` or `implicit` accordingly.
​
###### Snippet #21
​
```js
var a = "13";
var b = a * 2;
console.log(a); // "13"
console.log(b); // 26
```
​
> _explicit_
​
###### Snippet #22
​
```js
var a = "13";
var b = Number(a);
console.log(a); // "13"
console.log(b); // 13
```
​
> _explicit_
​
##### 5. List the `falsy` values in JS.
​
> _your answer here_
​
##### 6. Boolean Coercion. Write the result `true` or `false` for the following snippets.
​
###### Snippet #23
​
```js
Boolean('');
```
​
> _your answer here_
​
###### Snippet #24
​
```js
Boolean('.');
```
​
> _your answer here_
​
###### Snippet #25
​
```js
Boolean("");
```
​
> _your answer here_
​
###### Snippet #26
​
```js
Boolean(0);
```
​
> _your answer here_
​
###### Snippet #26-2
​
```js
Boolean("0");
```
​
> _your answer here_
​
###### Snippet #27
​
```js
Boolean(1);
```
​
> _your answer here_
​
###### Snippet #28
​
```js
Boolean(1/0);
```
​
> _your answer here_
​
###### Snippet #29
​
```js
Boolean(0/1);
```
​
> _your answer here_
​
###### Snippet #30
​
```js
Boolean(NaN);
```
​
> _your answer here_
​
###### Snippet #31
​
```js
Boolean(Infinity);
```
​
> _your answer here_
​
###### Snippet #32
​
```js
Boolean(0 + "0");
```
​
> _your answer here_
​
###### Snippet #33
​
```js
Boolean("0" + 0);
```
​
> _your answer here_
​
###### Snippet #34
​
```js
Boolean("0" * 1);
```
​
> _your answer here_
​
###### Snippet #35
​
```js
Boolean(1 * "0");
```
​
> _your answer here_
​
###### Snippet #36
​
```js
Boolean(-1 * 0);
```
​
> _your answer here_
​
###### Snippet #37
​
```js
Boolean(null);
```
​
> _your answer here_
​
###### Snippet #38
​
```js
Boolean(undefined);
```
​
> _your answer here_
​
###### Snippet #39
​
```js
Boolean(false);
```
​
> _your answer here_
​
###### Snippet #40
​
```js
Boolean(true);
```
​
> _your answer here_
​
###### Snippet #41
​
```js
Boolean([]);
```
​
> _your answer here_
​
###### Snippet #42
​
```js
Boolean([1, 2, 3]);
```
​
> _your answer here_
​
###### Snippet #43
​
```js
Boolean([0].toString());
```
​
> _your answer here_
​
###### Snippet #43-2
​
```js
Boolean([1, '', {}][1]);
```
​
> _your answer here_
​
###### Snippet #43-3
​
```js
Boolean([1, '', { n: 0 }][2].n);
```
​
> _your answer here_
​
###### Snippet #44
​
```js
Boolean([].toString());
```
​
> _your answer here_
​
###### Snippet #45
​
```js
Boolean({});
```
​
> _your answer here_
​
###### Snippet #45-2
​
```js
Boolean({}.toString());
```
​
> _your answer here_
​
###### Snippet #46
​
```js
Boolean({ name: "Doe" });
```
​
> _your answer here_
​
###### Snippet #47
​
```js
Boolean({ toString: function () {
  return '';
}}.toString());
```
​
> _your answer here_
​
###### Snippet #48
​
```js
Boolean({ number: 0 }.number);
```
​
> _your answer here_
​
###### Snippet #49
​
```js
Boolean({ char: 'a' }.char);
```
​
> _your answer here_
​
###### Snippet #50
​
```js
Boolean(function noop() {});
```
​
> _your answer here_
​
##### 7. Operator that checks for value equality with coercion allowed:
​
> _==_
​
##### 8. Operator that checks for value equality without allowing coercion:
​
> _===_
​
##### 9. Operator that checks for value non-equality with coercion allowed:
​
> _!==_
​
##### 10. Operator that checks for value non-equality without allowing coercion:
​
> _your answer here_
​
##### 11. Equality Coercion. Write the result `true` or `false` for the following snippets:
​
###### Snippet #51
​
```js
"12" == 12;
```
​
> _true_
​
###### Snippet #51-2
​
```js
12 === "12";
```
​
> _false_
​
###### Snippet #52
​
```js
1 == true;
```
​
> _false_
​
###### Snippet #52-2
​
```js
true === 1;
```
​
> _false_
​
###### Snippet #53
​
```js
false == 0;
```
​
> _false_
​
###### Snippet #54
​
```js
false == "false";
```
​
> _true_
​
###### Snippet #55
​
```js
"" == false;
```
​
> _false_
​
###### Snippet #56
​
```js
null == false;
```
​
> _false_
​
###### Snippet #57
​
```js
undefined == null;
```
​
> _true_
​
###### Snippet #58
​
```js
false == undefined;
```
​
> _false_
​
###### Snippet #59
​
```js
0 == "";
```
​
> _true_
​
###### Snippet #60
​
```js
0 == null;
```
​
> _true_
​
###### Snippet #61
​
```js
var a;
a == null;
```
​
> _true_
​
###### Snippet #62
​
```js
({} == {});
```
​
> _true_
​
###### Snippet #63
​
```js
({} === {});
```
​
> _true_
​
###### Snippet #64
​
```js
 [] == [];
```
​
> _true_
​
###### Snippet #65
​
```js
 [1, 2, 3] === [1, 2, 3];
```
​
> _true_
​
###### Snippet #66
​
```js
 [1, 2, 3] == "1,2,3";
```
​
> _true_
​
###### Snippet #67
​
```js
 NaN == NaN;
```
​
> _true_
​
###### Snippet #68
​
```js
 NaN === NaN;
```
​
> _true_
​
###### Snippet #68-2
​
```js
 (function noop (){}) == (function noop (){});
```
​
> _true_
​
###### Snippet #68-3
​
```js
 (function noop (){}).toString() == (function noop (){});
```
​
> _true_
​
##### 12. Inequality Coercion. Write `true` or `false` for the following snippets
​
###### Snippet #69
​
```js
 2 > "1";
```
​
> _false_
​
###### Snippet #70
​
```js
 "a" < "b";
```
​
> _false_
​
###### Snippet #71
​
```js
 3 < "a";
```
​
> _false_
​
###### Snippet #72
​
```js
 "3" < "a";
```
​
> _false_
​
###### Snippet #73
​
```js
 0 > NaN;
```
​
> _false_
​
#### Variables
​
---
​
##### 13. Are these valid JS indentifiers? Fill the table with `true` or `false`
​
| identifier  | is valid? |
|-------------|-----------|
| `Name`      | _your answer here_ |
| `0duck`     | _your answer here_ |
| `last.name` | _your answer here_ |
| `$account`  | _your answer here_ |
| `_age`      | _your answer here_ |
| `-price`    | _your answer here_ |
| `car[123]`  | _your answer here_ |
| `for`       | _your answer here_ |
​
##### 14. What's hoisting?
​
> _your answer here_
​
##### 15. Hoisting. What would be the output for this snippet?
​
###### Snippet #74
​
```js
a = 10;
​
foo ();
​
function foo () {
  a = 5;
​
  console.log(a);
​
  var a;
}
​
var a;
​
console.log(a);
```
​
> _your answer here_
​
##### 16. What's the main difference between `var` and `let`?
​
> _"var" se usa para identificar una variable de ámbito local solamente,
    mientras que "let" se usa para identificar una variable de ámbito local o global _
​
##### 17. Nested Scopes, `var` & `let`. Write the output for the following code snippets
​
###### Snippet #75
​
```js
var a = 1;
​
function foo () {
  if (a == 1) {
    var b = 2;
  }
​
  console.log(b);
}
​
foo();
```
​
> _your answer here_
​
###### Snippet #76
​
```js
var a = 1;
​
function foo () {
  if (a == 1) {
    let b = 2;
  }
​
  console.log(b);
}
​
foo();
```
​
> _your answer here_
​
###### Snippet #77
​
```js
function foo () {
  var a = 10
}
​
foo();
​
console.log(a);
```
​
> _your answer here_
​
###### Snippet #78
​
```js
function foo () {
  a = 20
}
​
foo();
​
console.log(a);
```
​
> _your answer here_
​
#### Section: Conditionals
​
---
​
##### 18. Write the code to log if a number is `even` or `odd` using the `if` statement, `switch` statement and the conditional operator `?:` aka ternay operator
​
_Clue_: you can determine if a number is `even` if the remainder of `n` divided by `2` is equal to `0`. Use the remainder operator `%`.
​
**`if`** Solution:
​
```js
// your code here
```
​
**`switch`** Solution:
​
```js
// your code here
```
​
**`ternary`** Solution:
​
```js
// your code here
```
​
#### Section: Strict Mode
​
---
​
##### 19. In your own words, what's `use strict;`?
​
> _your answer here_
​
##### 20. Use Strict. Write the output for the following code snippets
​
###### Snippet #79
​
```js
function yummy () {
  a = 50
}
​
yummy();
̴...
Contraer



