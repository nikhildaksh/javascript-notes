# 8. Functions

## Theory
Functions are blocks of code that do a specific task. You can use them again and again by calling their name. Functions help you organize and reuse your code easily.
- **Function Declaration:** The normal way to define a function.
- **Function Expression:** Store a function in a variable.
- **Arrow Function:** A shorter way to write functions (introduced in ES6).
- **Parameters:** Placeholders for values you pass to a function.
- **Arguments:** Actual values you give to the function when calling it.
- **Return Statement:** Sends a value back from the function.
- **Callback Function:** A function passed as an argument to another function.
- **IIFE:** A function that runs immediately after it is defined.

---

## Practical Examples

### 1. Function Declaration

Example 01:
```js
function fun1(){
  console.log("function one")
}
fun1(); // call the function
```

Example 02:
```js
function greet(name) {
  console.log('Hello, ' + name + '!');
}
greet('Amit'); // Hello, Amit!
```

### 2. Function Expression
```js
const add = function(a, b) {
  return a + b;
};
console.log(add(2, 3)); // 5
```

### 3. Arrow Function

Example 01:
```js

let sum2Numbers = ()=>{
  let num1 = Number(prompt("Enter First Number: "));
  let num2 = Number(Prompt("Enter Second Number: "));
  let sum = num1+num2;
  console.log(sum);
}

```

Example 02:
```js
const multiply = (x, y) => x * y;
console.log(multiply(4, 5)); // 20
```

### 4. Parameters vs Arguments
```js
function showMessage(message) { // 'message' is a parameter
  console.log(message);
}
showMessage('Welcome!'); // 'Welcome!' is an argument
```

### 5. Return Statement
Example 01:
```js
function square(n) {
  return n * n;
}
let result = square(6);
console.log(result); // 36
```

Example 02: if our function return a statement then we can write the function like:
```js
const square = (n) => n*n
let output = square(3)
console.log(output)
```

### 6. Callback Function
```js
function process(num, callback) {
  callback(num);
}
process(10, function(n) {
  console.log('Number is', n);
});
```

### 7. IIFE (Immediately Invoked Function Expression)
```js
(function() {
  console.log('I run immediately!');
})();
```

---

## Practice Questions
1. Write a function to add two numbers and return the result.
2. Create an arrow function to multiply three numbers.
3. What is the difference between parameters and arguments? Give an example.
4. Write a function that takes a name and prints "Hello, [name]!".
5. Use a callback function to print the square of a number.
6. Write an IIFE that prints "JavaScript is fun!".

---

**Tip:** Functions make your code reusable and organized. Try writing your own functions for different tasks! 