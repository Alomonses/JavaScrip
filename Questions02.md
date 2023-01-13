###### Question 1: What's the output?

```js
function greeting() {
console.log(name);
console.log(age);
var name = "Hana";
let age = 21;
}

greeting();
// A: Hana and undefined
// B: Hana and ReferenceError
// C: ReferenceError and 21
// D: undefined and ReferenceError

// Ans: D: undefined and ReferenceError
// Short explanation:They are not accessible before the line we declare
###### Question 2: What's the output?

```js
+true;
!"Lydia";

// A: 1 and false
// B: false and NaN
// C: false and false

// Ans:  A: 1 and false
// Short explanation: the unary plus tries to convert an operand to a number. true is 1, and false is 0.


```
###### Question 3: What's the output?

```js
function sum(a, b) {
return a + b;
}

sum(1, "2");

// A: NaN
// B: TypeError
// C: "12"
// D: 3

// Ans: C: "12"
// Short explanation: JS take both values as a string so they just are concatenated
```
###### Question 4: What's the output?

```js
let number = 0;
console.log(number++);
console.log(++number);
console.log(number);

// A: 1 1 2
// B: 1 2 2
// C: 0 2 2
// D: 0 1 2

// Ans: C: 0 2 2
// Short explanation: In the first console.log the increment is AFTER the variable so it would show in the next opportunity. In the second the incremnet is BEFORE the  variable so it will increce the value before show it.
```

###### Question 5: What's the output?

```js
!!null;
!!"";
!!1;

// A: false true false
// B: false false true
// C: false true true
// D: true true false

// Ans:B: false false true
// Short explanation: Null, Space, 0 are consider as a false and the others elemnts as true

```
###### Question 6: What's the output?

```js
console.log(3 + 4 + "5");

// A: "345"
// B: "75"
// C: 12
// D: "12"

// Ans: B: "75"
// Short explanation: 3 AND 4 are the same type of value (number) so js add them but 5 is String so this value is only concatenated with the result of the addittion
```
###### Question 7: What's the value of num?

```js
const num = parseInt("7*6", 10);

// A: 42
// B: "42"
// C: 7
// D: NaN

// Ans: C: 7
// Short explanation:
```

###### Question 8:

Write a function indexOfIgnoreCase taking two strings
and determining the first occurrence of the second
string in the first string. The function should be
case insensitive.

Example: indexOfIgnoreCase('bit','it') and
indexOfIgnoreCase('bit','IT') should return 1.

```js
//Hint
function indexOfIgnoreCase(s1, s2) {
// Change s1 and s2
// first to lowercase.
// Then use the
// indexOf method.
}

```

###### Question 9:
Write a function firstChar, which returns the
first character that is not a space when a string
is passed.

Example: firstChar(' Rosa Parks ') should return 'R'.

```js
//Hint:
function firstChar(text) {
// Trim first.
// Then use the
// charAt method.
}
```
function firstChar(text) {
    var input = text;
    if (input.charAt(0) == " ") {
        return input.charAt(1);
    }
    else {
        return input.charAt(0);
    }

}
console.log(firstChar(' Rosa Parks '));


###### Question 10:
Write a function normalize, that replaces '-'
with '/' in a date string.

Example: normalize('20-05-2017') should return
'20/05/2017'.


function normalize(date) {

    let newdate = date.replace(/-/g, "/");

}

console.log(normalize('20/05/2017'));