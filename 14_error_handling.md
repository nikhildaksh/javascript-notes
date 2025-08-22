# 14. Error Handling

## Theory
Error handling means managing mistakes in your code so your program doesn't crash. JavaScript gives you special keywords to catch and handle errors:
- **try:** Code that might cause an error goes here.
- **catch:** Runs if there is an error in try.
- **finally:** Runs after try/catch, no matter what (used for cleanup).
- **throw:** Lets you create your own (custom) errors.

Custom errors help you show meaningful messages when something goes wrong.

---

## Practical Examples

### 1. try, catch, finally
```js
try {
  let result = 10 / 0;
  console.log(result);
  // let x = y; // Uncomment to see a ReferenceError
} catch (error) {
  console.error('Error caught:', error.message);
} finally {
  console.log('This always runs.');
}
```

### 2. throw and Custom Errors
```js
function divide(a, b) {
  if (b === 0) {
    throw new Error('Cannot divide by zero!');
  }
  return a / b;
}

try {
  console.log(divide(10, 0));
} catch (err) {
  console.error('Custom Error:', err.message);
}
```

---

## Practice Questions
1. Write code that tries to access an undefined variable and catches the error.
2. Use try-catch-finally to handle an error and print a custom message.
3. Create a function that throws an error if the input is not a number.
4. What does the finally block do? Try removing it and see the difference.
5. Write a custom error message for dividing by zero.

---

**Tip:** Good error handling makes your code safe and user-friendly. Always handle possible errors in your programs! 