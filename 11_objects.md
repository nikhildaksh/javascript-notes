# 11. Objects

## Theory
Objects are used to store data in key-value pairs. Each value (property) has a name (key). Objects help you group related data and functions together.
- You can access properties using dot (.) or bracket ([]) notation.
- Objects can also have methods (functions inside objects).
- The `this` keyword refers to the object itself inside its methods.
- Object destructuring lets you easily extract values from objects.
- Spread (`...`) and rest (`...`) operators help you copy or collect properties.

---

## Practical Examples

### 1. Object Creation & Accessing Properties
```js
let person = {
  name: 'Amit',
  age: 22,
  city: 'Delhi'
};
console.log(person.name); // 'Amit' (dot notation)
console.log(person['city']); // 'Delhi' (bracket notation)
```

### 2. Methods Inside Objects & this Keyword
```js
let user = {
  name: 'Sara',
  greet: function() {
    console.log('Hello, ' + this.name);
  }
};
user.greet(); // 'Hello, Sara'
```

### 3. Object Destructuring
```js
let car = { brand: 'Honda', model: 'Civic', year: 2020 };
let { brand, year } = car;
console.log(brand); // 'Honda'
console.log(year); // 2020
```

### 4. Spread and Rest Operator
```js
let obj1 = { a: 1, b: 2 };
let obj2 = { ...obj1, c: 3 };
console.log(obj2); // { a: 1, b: 2, c: 3 }

function showAll(...args) {
  console.log(args);
}
showAll(1, 2, 3); // [1, 2, 3]
```

---

## Practice Questions
1. Create an object for a student with properties: name, age, and grade. Print all properties.
2. Add a method to the object that prints "Hi, I am [name]".
3. Access a property using bracket notation.
4. Use object destructuring to get the 'age' from the student object.
5. Use the spread operator to copy all properties from one object to another and add a new property.
6. Write a function using the rest operator that takes any number of numbers and prints them as an array.
7. What does the `this` keyword refer to inside an object method?

---

**Tip:** Objects are very useful for grouping related data. Try creating your own objects and using different features! 