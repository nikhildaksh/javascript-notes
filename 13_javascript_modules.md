# 13. JavaScript Modules

## Theory
Modules help you organize your code by splitting it into different files. You can export (share) code from one file and import (use) it in another. This makes your code cleaner and easier to manage.
- **export:** Use to share variables, functions, or classes from a file.
- **import:** Use to bring exported code into another file.
- **Default export:** Only one per file, imported without curly braces.
- **Named export:** Many per file, imported with curly braces.

---

## Practical Examples

### 1. Named Export and Import
```js
// math.js
export function add(a, b) {
  return a + b;
}
export function subtract(a, b) {
  return a - b;
}

// main.js
import { add, subtract } from './math.js';
console.log(add(2, 3)); // 5
```

### 2. Default Export and Import
```js
// greet.js
export default function greet(name) {
  console.log('Hello, ' + name);
}

// main.js
import greet from './greet.js';
greet('Amit'); // Hello, Amit
```

---

## Practice Questions
1. Create a file that exports two functions: one for addition and one for multiplication. Import and use them in another file.
2. What is the difference between default and named exports?
3. Try exporting a variable and importing it in another file.
4. Can you have more than one default export in a file? Why or why not?
5. Write a default export for a function that prints "Welcome to Modules!" and import it in another file.

---

**Tip:** Modules make your code organized and reusable. Practice splitting your code into different files and using import/export! 