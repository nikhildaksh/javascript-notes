# 12. Advanced Objects

## Theory
Objects can have other objects or arrays inside them. These are called nested objects or nested arrays. You can loop through object properties using special loops. JSON (JavaScript Object Notation) is a way to store and send data. You can convert objects to JSON strings and back using `JSON.stringify()` and `JSON.parse()`.

---

## Practical Examples

### 1. Nested Objects & Arrays
```js
let student = {
  name: 'Amit',
  marks: {
    math: 90,
    science: 85
  },
  hobbies: ['reading', 'cricket']
};
console.log(student.marks.math); // 90
console.log(student.hobbies[1]); // 'cricket'
```

### 2. Looping Through Objects
```js
let car = { brand: 'Honda', model: 'Civic', year: 2020 };
for (let key in car) {
  console.log(key, car[key]);
}
```

### 3. JSON.stringify() and JSON.parse()
```js
let obj = { name: 'Sara', age: 21 };
let jsonStr = JSON.stringify(obj); // Convert object to JSON string
console.log(jsonStr); // '{"name":"Sara","age":21}'

let newObj = JSON.parse(jsonStr); // Convert JSON string back to object
console.log(newObj.name); // 'Sara'
```

---

## Practice Questions
1. Create an object with a nested object and a nested array. Print one value from each.
2. Loop through all properties of an object and print their keys and values.
3. Convert an object to a JSON string using `JSON.stringify()`.
4. Convert a JSON string back to an object using `JSON.parse()`.
5. What is the difference between an object and a JSON string?

---

**Tip:** Nested objects and JSON are very useful for working with complex data. Practice converting and accessing nested values! 