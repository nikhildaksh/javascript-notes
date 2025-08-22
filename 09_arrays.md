# 9. Arrays

## Theory
Arrays are special variables that can store multiple values in a single variable. Each value in an array has an index (position), starting from 0. Arrays help you manage lists of data easily.

You can add, remove, or change items in an array using different methods.

---

## Practical Examples

### 1. Declaration, Indexing, Iteration
```js
let fruits = ['apple', 'banana', 'mango'];
console.log(fruits[0]); // 'apple' (index 0)
console.log(fruits[2]); // 'mango' (index 2)

// Iteration
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}
```

### 2. Common Methods
```js
let nums = [1, 2, 3];
nums.push(4); // [1,2,3,4] (add at end)
nums.pop(); // [1,2,3] (remove last)
nums.shift(); // [2,3] (remove first)
nums.unshift(0); // [0,2,3] (add at start)

let arr = [10, 20, 30, 40];
arr.splice(1, 2); // [10,40] (remove 2 items from index 1)
let sliced = arr.slice(0, 2); // [10,40] (copy from index 0 to 2, not including 2)

let a = [1,2], b = [3,4];
let combined = a.concat(b); // [1,2,3,4]
```

### 3. Higher Order Methods
```js
let numbers = [1, 2, 3, 4, 5];
let doubled = numbers.map(n => n * 2); // [2,4,6,8,10]
let evens = numbers.filter(n => n % 2 === 0); // [2,4]
let sum = numbers.reduce((acc, n) => acc + n, 0); // 15

numbers.forEach(n => console.log(n)); // prints each number

let found = numbers.find(n => n > 3); // 4
let hasEven = numbers.some(n => n % 2 === 0); // true
let allPositive = numbers.every(n => n > 0); // true
let includesThree = numbers.includes(3); // true
```

---

## Practice Questions
1. Create an array of 5 colors and print the third color.
2. Add a new color to the end of the array using `push()`.
3. Remove the first color using `shift()` and print the array.
4. Use a loop to print all elements of an array.
5. Use `map()` to create a new array with each number doubled.
6. Use `filter()` to get all numbers greater than 10 from an array.
7. Use `reduce()` to find the sum of all numbers in an array.
8. Check if an array includes the value 7.
9. Use `find()` to get the first number greater than 100 in an array.
10. What is the difference between `forEach()` and `map()`?

---

**Tip:** Arrays are very useful for handling lists. Try using different methods and see how the array changes! 