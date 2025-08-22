# 7. Loops / Iteration

## Theory
Loops help you run the same block of code multiple times. This is useful when you want to repeat something, like printing numbers from 1 to 10. JavaScript has different types of loops:
- **for:** Runs code a set number of times.
- **while:** Runs code while a condition is true.
- **do...while:** Runs code at least once, then repeats while a condition is true.
- **break:** Stops the loop early.
- **continue:** Skips the current loop step and goes to the next.
- **for...in:** Loops through object properties.
- **for...of:** Loops through values in arrays or strings.

---

## Practical Examples

### 1. for loop
```js
for (let i = 1; i <= 5; i++) {
  console.log('Number:', i);
}
```

### 2. while loop
```js
let count = 1;
while (count <= 3) {
  console.log('Count:', count);
  count++;
}
```

### 3. do...while loop
```js
let num = 1;
do {
  console.log('Num:', num);
  num++;
} while (num <= 2);
```

### 4. break and continue
```js
for (let i = 1; i <= 5; i++) {
  if (i === 3) break; // stops loop when i is 3
  console.log(i);
}

for (let i = 1; i <= 5; i++) {
  if (i === 3) continue; // skips 3
  console.log(i);
}
```

### 5. for...in vs for...of
```js
let person = { name: 'Amit', age: 21 };
for (let key in person) {
  console.log(key, person[key]); // keys and values
}

let colors = ['red', 'green', 'blue'];
for (let color of colors) {
  console.log(color); // values
}
```

---

## Practice Questions
1. Print numbers from 1 to 10 using a for loop.
2. Use a while loop to print even numbers from 2 to 10.
3. Use a do...while loop to print numbers from 5 to 1 (reverse order).
4. Write a loop that stops when it finds the number 7 in an array.
5. Use continue to skip printing the number 5 in a loop from 1 to 7.
6. Use for...in to print all properties of an object.
7. Use for...of to print all elements of an array.

---

**Tip:** Loops make it easy to repeat tasks. Try changing the loop conditions and see what happens! 