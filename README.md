# Curated JS output based questions

###### Question 1

```javascript
function ab(a = 100, b = 20) {
  console.log(a + b)
}

ab(null, 200)
ab(NaN, 200)

ab(undefined, 200)
```
<details>
<summary>Answer</summary>
  <span>200</span> | <span>NaN</span> <span>300</span>
</details>

---

###### Question 2

```javascript
const obj = Object.freeze({
  name: "Alice",
  info: {
    age: 25
  }
});

try {
  obj.name = "Bob";
  obj.info.age = 30;
} catch (e) {
  console.log("Error:", e.message);
}

console.log(obj.name, obj.info.age);
```
<details>
<summary>Answer</summary>
  <span>Alice</span> | <span>30</span>
</details>

---

###### Question 3

```javascript
var a = 10;
let a = 20;
console.log(a)
```
<details>
<summary>Answer</summary>
  <span> Output : SyntaxError: Identifier 'a' has already been declared
Reason : In Javascript, we cannot redeclare a variable with let if it has already been declared in the same scope. </span>
</details>

---

###### Question 4

```javascript
let a = 3;
let b = new Number(3);
let c = 3;

console.log(a == b);
console.log(a === b);
console.log(b === c);
```
<details>
<summary>Answer</summary>
  <span> true | false | false </span>

  <p>new Number() is a built-in function constructor. Although it looks like a number, it's not really a number: it has a bunch of extra features and is an object.

When we use the == operator (Equality operator), it only checks whether it has the same value. They both have the value of 3, so it returns true.

However, when we use the === operator (Strict equality operator), both value and type should be the same. It's not: new Number() is not a number, it's an object. Both return false.</p>
</details>

---

###### Question 5

```javascript
const target = { a: 'toy' , b: 'boy' };
const source = { b: 'car', c: 'pot' };

const returnedTarget = Object.assign(target, source);

console.log(target);

console.log(returnedTarget);
 
console.log(source);
```
<details>
<summary>Answer</summary>
  <span> {
  a: "toy",
  b: "car",
  c: "pot"
} </span>
  <a href='https://javascript.plainenglish.io/difference-between-object-assign-and-object-create-in-javascript-6f3ee100f99d'>Article</a>
</details>

---
###### Question 6

```javascript
const user = { 
name: "Surbhi dighe", 
country: "India" 
};
const { name: fullname, country } = user;
console.log(fullname);
console.log(name);

```
<details>
<summary>Answer</summary>
  <span> Surbhi dighe </span>
  <span> ReferenceError: name is not defined. it gives an error because name was assigned to a local variable fullname and therefore name is not directly accessible.</span>
</details>

---

#### Question 7
```javascript
const arr = [11, 0, '', false, 2, 1];
const filtered = arr.filter(Boolean);
console.log(filtered);
```
<details>
<summary>Answer</summary>
  <span> [11,2,1] </span>
  <span> Reason : filter(Boolean) removes all falsy values (0, "" (empty string), false, null, undefined, and NaN) from the array and keeps truthy ones.</span>

</details>

---

### Question 8

```javascript
console.log(10 - "5");
console.log("5" - 10);

```

<details>
  <summary>Answer</summary>
  <span> 5, -5 </span>
</details>

---

###### Question template

```javascript

```
<details>
<summary>Answer</summary>
  <span>  </span>
</details>

---










