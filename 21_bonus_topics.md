# 21. Bonus (Recommended for Projects)

## Theory
These advanced topics help you write better, faster, and more efficient JavaScript code. They are very useful in real-world projects and interviews.
- **Closures & Lexical Scope:** Functions can remember variables from where they were created.
- **Debouncing & Throttling:** Control how often a function runs (useful for search, scroll, resize events).
- **Hoisting:** JavaScript moves declarations to the top before running code.
- **Event Loop & Call Stack:** How JavaScript handles tasks and runs code.
- **Memory Management Basics:** How JavaScript stores and cleans up data.
- **Currying:** Breaking a function with many arguments into many functions with one argument each.
- **Memoization:** Remembering results of expensive function calls to speed up code.
- **Deep vs Shallow Copy:** Copying objects/arrays by value or by reference.
- **Polyfills:** Code that adds missing features to old browsers.
- **Code Splitting:** Breaking code into smaller files to load faster.

---

## Practical Examples

### 1. Closures & Lexical Scope
```js
function outer() {
  let count = 0;
  function inner() {
    count++;
    return count;
  }
  return inner;
}
let counter = outer();
console.log(counter()); // 1
console.log(counter()); // 2
```

### 2. Debouncing & Throttling (Simple Example)
```js
// Debounce: Only run after user stops typing for 500ms
function debounce(fn, delay) {
  let timer;
  return function(...args) {
    clearTimeout(timer);
    timer = setTimeout(() => fn(...args), delay);
  };
}

// Throttle: Only run once every 1 second
function throttle(fn, limit) {
  let lastCall = 0;
  return function(...args) {
    const now = Date.now();
    if (now - lastCall >= limit) {
      lastCall = now;
      fn(...args);
    }
  };
}
```

### 3. Hoisting
```js
console.log(a); // undefined (not error)
var a = 5;
// Function hoisting
hoisted(); // 'I am hoisted!'
function hoisted() {
  console.log('I am hoisted!');
}
```

### 4. Event Loop & Call Stack
```js
console.log('Start');
setTimeout(() => console.log('Timeout'), 0);
console.log('End');
// Output: Start, End, Timeout
```

### 5. Currying
```js
function add(a) {
  return function(b) {
    return a + b;
  };
}
console.log(add(2)(3)); // 5
```

### 6. Memoization
```js
function memoize(fn) {
  const cache = {};
  return function(x) {
    if (cache[x]) return cache[x];
    cache[x] = fn(x);
    return cache[x];
  };
}
const square = memoize(x => x * x);
console.log(square(4)); // 16
console.log(square(4)); // 16 (from cache)
```

### 7. Deep vs Shallow Copy
```js
let arr1 = [1, 2, 3];
let arr2 = arr1; // Shallow copy (same reference)
let arr3 = [...arr1]; // Deep copy (new array)
arr2[0] = 99;
console.log(arr1[0]); // 99
console.log(arr3[0]); // 1
```

### 8. Polyfills (Simple Example)
```js
if (!Array.prototype.myMap) {
  Array.prototype.myMap = function(callback) {
    let result = [];
    for (let i = 0; i < this.length; i++) {
      result.push(callback(this[i], i, this));
    }
    return result;
  };
}
```

### 9. Code Splitting (Concept)
```js
// In modern frameworks (like React), code splitting is done automatically.
// Example: import('./module.js').then(...)
```

---

## Practice Questions
1. Write a closure that remembers a value and increases it every time you call it.
2. What is hoisting? Give an example with a variable and a function.
3. Explain the difference between deep and shallow copy with code.
4. Write a simple debounce function.
5. What is memoization? Try memoizing a function that returns the square of a number.
6. How does the event loop work? Try using setTimeout and see the order of output.
7. What is a polyfill? Write a polyfill for Array.prototype.filter.
8. What is code splitting and why is it useful?

---

**Tip:** These topics are important for interviews and real-world projects. Try to understand and use them in your code! 