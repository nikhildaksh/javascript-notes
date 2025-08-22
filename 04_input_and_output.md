# 4. Input & Output

## Theory
Input means taking data from the user. Output means showing data to the user or developer. In JavaScript, you can use different methods for input and output:
- `alert()`: Shows a popup message to the user.
- `prompt()`: Asks the user to enter some input.
- `confirm()`: Asks the user a Yes/No question.
- `console.log()`: Prints messages in the browser console (for developers).
- `console.error()`: Prints error messages in the console.
- `console.table()`: Shows data in a table format in the console.

---

## Practical Examples

### 1. alert(), prompt(), confirm()
```js
alert('Welcome to JavaScript!'); // Shows a popup message

let name = prompt('What is your name?'); // Asks for user input
alert('Hello, ' + name);

let isSure = confirm('Are you sure you want to continue?'); // Yes/No popup
alert('User clicked: ' + isSure); // true if Yes, false if No
```

### 2. console.log(), console.error(), console.table()
```js
console.log('This is a normal message');
console.error('This is an error message');

let students = [
  { name: 'Amit', age: 20 },
  { name: 'Sara', age: 22 }
];
console.table(students); // Shows data in table format
```

---

## Practice Questions
1. Use `alert()` to show your name in a popup.
2. Ask the user for their favorite color using `prompt()` and print it using `console.log()`.
3. Use `confirm()` to ask the user if they like JavaScript. Print the result in the console.
4. Create an array of 3 objects (each with name and age) and display it using `console.table()`.
5. Try using `console.error()` to print a custom error message.

---

**Tip:** Open your browser and press F12 to use the console for trying these examples! 