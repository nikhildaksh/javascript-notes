# 20. ES6+ Modern JavaScript Features

## Theory
ES6 (ECMAScript 2015) and later versions added many new features to JavaScript. These features make your code shorter, easier, and more powerful. Here are some of the most useful ones:
- **let, const:** New ways to declare variables.
- **Arrow functions:** Shorter way to write functions.
- **Default parameters:** Give default values to function parameters.
- **Template literals:** Use backticks and `${}` for easy string building.
- **Destructuring:** Quickly extract values from arrays or objects.
- **Spread & Rest operators (`...`):** Copy, combine, or collect values.
- **Enhanced object literals:** Easier way to write objects.
- **Optional chaining (`?.`):** Safely access nested properties.
- **Nullish coalescing (`??`):** Use a default value if something is null or undefined.
- **Modules:** Split code into files using `import` and `export`.
- **Classes:** Easier way to create objects with methods.

---

## Practical Examples

### 1. let, const
```js
let age = 20;
const pi = 3.14;
```

### 2. Arrow Functions
```js
const add = (a, b) => a + b;
```

### 3. Default Parameters
```js
function greet(name = 'Guest') {
  console.log('Hello, ' + name);
}
greet(); // Hello, Guest
```

### 4. Template Literals
```js
let name = 'Amit';
console.log(`Welcome, ${name}!`);
```

### 5. Destructuring
```js
let person = { name: 'Sara', age: 22 };
let { name, age } = person;
console.log(name, age);

let arr = [1, 2, 3];
let [x, y] = arr;
console.log(x, y);
```

### 6. Spread & Rest Operators
```js
let nums = [1, 2, 3];
let more = [...nums, 4, 5]; // Spread

function sum(...args) { // Rest
  return args.reduce((a, b) => a + b, 0);
}
console.log(sum(1, 2, 3));
```

### 7. Enhanced Object Literals
```js
let color = 'red';
let car = {
  color,
  drive() {
    console.log('Driving');
  }
};
```

### 8. Optional Chaining & Nullish Coalescing
```js
let user = {};
console.log(user.profile?.name); // undefined, no error
let username = user.name ?? 'Guest';
console.log(username); // 'Guest'
```

### 9. Modules (see module section for more)
```js
// export const value = 10;
// import { value } from './file.js';
```

### 10. Classes
```js
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(this.name + ' makes a sound');
  }
}
let dog = new Animal('Dog');
dog.speak();
```

---

## Practice Questions
1. Use `let` and `const` to declare two variables.
2. Write an arrow function to multiply two numbers.
3. Create a function with a default parameter and call it without passing the argument.
4. Use template literals to print your name and age.
5. Destructure an object to get its properties.
6. Use the spread operator to combine two arrays.
7. Write a function using the rest operator to add any number of numbers.
8. Use optional chaining to safely access a nested property.
9. Use nullish coalescing to give a default value if a variable is undefined.
10. Create a simple class for a Student with a method to print their name.

---

**Tip:** Modern JavaScript features make your code cleaner and easier. Try using them in your projects! 