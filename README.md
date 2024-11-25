# Curated JS output based questions

###### Question 1

```javascript
function ab(a = 100, b = 20) {
  console.log(a + b)
}

ab(null, 200)

ab(undefined, 200)
```
<details>
<summary>Answer</summary>
  <span>200</span> | <span>300</span>
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

```
<details>
<summary>Answer</summary>
  <span> ... </span>
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







