# 3. Type Conversion & Type Coercion

## Theory
In JavaScript, sometimes you need to change one type of value to another. This is called type conversion. There are two ways this happens:

- **Implicit Type Conversion (Type Coercion):** JavaScript automatically changes the type for you. For example, adding a number and a string will turn the number into a string.
- **Explicit Type Conversion (Type Casting):** You change the type yourself using functions like `String()`, `Number()`, or `Boolean()`.

This helps you work with different types of data easily, but you should know how and when these changes happen.

---

## Practical Examples

### 1. Implicit Type Conversion (Type Coercion)
```js
let result = '5' + 2; // '52' (number 2 becomes string)
let sum = '10' - 3;   // 7 (string '10' becomes number)
let boolTest = 'true' == true; // false (string is not converted to boolean)
```

### 2. Explicit Type Conversion (Type Casting)
```js
let num = '123';
let convertedNum = Number(num); // 123 (string to number)

let str = 456;
let convertedStr = String(str); // '456' (number to string)

let val = 0;
let boolVal = Boolean(val); // false (0 is false)
```

### 3. parseInt and parseFloat
```js
let n1 = '42';
let intVal = parseInt(n1); // 42

let n2 = '3.14';
let floatVal = parseFloat(n2); // 3.14

let n3 = '100px';
let parsed = parseInt(n3); // 100 (stops at non-number)
```

---

## Practice Questions
1. What will be the result of `'7' + 3` and `'7' - 3`?
2. Convert the string `'2024'` to a number and print its type.
3. Use `Boolean()` to check if an empty string `''` is true or false.
4. What does `parseInt('50.99')` return? Try it in the console.
5. Write code to convert the number `99` to a string and print its type.

---

**Tip:** Always check the type using `typeof` after conversion to avoid confusion! 