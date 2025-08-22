# 5. Operators

## Theory
Operators are special symbols or keywords that help you perform actions on values or variables. JavaScript has many types of operators:
- **Arithmetic Operators:** For math (like +, -, *, /)
- **Assignment Operators:** To assign values (=, +=, -=, etc.)
- **Comparison Operators:** To compare values (==, ===, !=, >, <, etc.)
- **Logical Operators:** For logic (&& for AND, || for OR, ! for NOT)
- **Ternary Operator:** Short way to write if-else (`condition ? value1 : value2`)
- **Nullish Coalescing (`??`):** Gives a default value if the first is null or undefined
- **Optional Chaining (`?.`):** Safely access nested object properties

---

## Practical Examples

### 1. Arithmetic, Assignment, Comparison
```js
let a = 10, b = 3;
console.log(a + b); // 13
console.log(a - b); // 7
console.log(a * b); // 30
console.log(a / b); // 3.333...
console.log(a % b); // 1

a += 2; // a = a + 2
console.log(a); // 12

console.log(a == 12); // true
console.log(a === '12'); // false (strict equality)
console.log(a > b); // true
```

### 2. Logical Operators
```js
let x = 5, y = 10;
console.log(x > 0 && y > 0); // true (both true)
console.log(x > 10 || y > 0); // true (one is true)
console.log(!(x == 5)); // false (not true)
```

### 3. Ternary Operator
```js
let age = 18;
let canVote = (age >= 18) ? 'Yes' : 'No';
console.log(canVote); // 'Yes'
```

### 4. Nullish Coalescing (??)
```js
let userName = null;
let defaultName = userName ?? 'Guest';
console.log(defaultName); // 'Guest'
```

### 5. Optional Chaining (?.)
```js
let user = { profile: { name: 'Amit' } };
console.log(user.profile?.name); // 'Amit'
console.log(user.address?.city); // undefined (no error)
```

---

## Practice Questions
1. Write code to add, subtract, multiply, and divide two numbers.
2. Use assignment operators to increase a variable by 5 and then decrease it by 2.
3. Compare two numbers using `==` and `===`. What is the difference?
4. Use logical operators to check if a number is between 10 and 20 (inclusive).
5. Use the ternary operator to print "Adult" if age is 18 or more, otherwise print "Minor".
6. Use `??` to give a default value if a variable is undefined.
7. Use optional chaining to safely access a nested property in an object.

---

**Tip:** Try all examples and questions in your browser console to see how operators work! 