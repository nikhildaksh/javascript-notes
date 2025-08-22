# 2. Variables and Data Types

## Theory
Variables are like boxes in which you can store information (data) in your program. In JavaScript, you can create variables using `var`, `let`, or `const`:
- `var` is the old way, works in the whole function.
- `let` is the modern way, works only inside the block where you define it.
- `const` is for values that should not change.

JavaScript supports different types of data:
- **Number:** For all numbers (integers and decimals)
- **String:** For text (written in quotes)
- **Boolean:** true or false values
- **Undefined:** When a variable is declared but not given a value
- **Null:** Special value meaning "nothing"
- **BigInt:** For very large numbers
- **Symbol:** For unique values

JavaScript is a loosely typed language, so you can change the type of value stored in a variable anytime.

---

## Practical Examples

### 1. What is a Variable?
```js
let name = 'Rahul'; // string
typeof name; // 'string'

let age = 25; // number
typeof age; // 'number'
```

### 2. var, let, const
```js
var city = 'Delhi'; // function-scoped, can be changed
let country = 'India'; // block-scoped, can be changed
const pi = 3.14; // block-scoped, cannot be changed

city = 'Mumbai'; // OK
country = 'Nepal'; // OK
// pi = 3.15; // Error: Assignment to constant variable
```

### 3. Primitive Data Types
```js
let num = 10; // Number
let str = 'Hello'; // String
let isActive = true; // Boolean
let nothing = null; // Null
let notDefined; // Undefined
let bigNum = 12345678901234567890n; // BigInt
let sym = Symbol('id'); // Symbol
```

### 4. Dynamic Typing
```js
let data = 100; // number
data = 'Now I am a string'; // string
```

---

## Practice Questions
1. Create a variable to store your favorite movie name. Print its value and type.
2. Change a variable's value from a number to a string. Print both values and their types.
3. What happens if you try to change a `const` variable?
4. Create variables for your name, age, and if you like coding (true/false). Print all.
5. Try using `typeof` on `null` and `undefined`. What do you get?

---

**Tip:** Try all examples and questions in your browser console for better understanding! 