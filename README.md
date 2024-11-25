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





