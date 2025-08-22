# 10. Strings

## Theory
Strings are used to store text in JavaScript. You can write strings inside single quotes (' '), double quotes (" "), or backticks (` `). Strings have many useful methods to work with text, like finding length, changing case, or extracting parts of the string.

Template literals (using backticks) let you easily add variables inside strings.

---

## Practical Examples

### 1. Basic String and Length
```js
let message = 'Hello, World!';
console.log(message.length); // 13
```

### 2. charAt(), slice(), substring()
```js
let str = 'JavaScript';
console.log(str.charAt(0)); // 'J'
console.log(str.slice(1, 4)); // 'ava'
console.log(str.substring(4, 10)); // 'Script'
```

### 3. split(), replace(), toLowerCase(), toUpperCase(), trim()
```js
let text = '  Learn JavaScript!  ';
console.log(text.split(' ')); // ['','', 'Learn', 'JavaScript!','', '']
console.log(text.replace('JavaScript', 'JS')); // '  Learn JS!  '
console.log(text.toLowerCase()); // '  learn javascript!  '
console.log(text.toUpperCase()); // '  LEARN JAVASCRIPT!  '
console.log(text.trim()); // 'Learn JavaScript!'
```

### 4. Template Literals
```js
let name = 'Amit';
let age = 21;
let info = `My name is ${name} and I am ${age} years old.`;
console.log(info); // 'My name is Amit and I am 21 years old.'
```

---

## Practice Questions
1. Create a string with your favorite quote and print its length.
2. Use `charAt()` to print the first character of a string.
3. Use `slice()` to get the last 3 characters of a string.
4. Replace the word 'bad' with 'good' in the string 'JavaScript is not bad!'.
5. Convert a string to uppercase and lowercase.
6. Remove extra spaces from the string '  Hello JS  '.
7. Split a sentence into words using `split()`.
8. Use a template literal to print your name and city in one sentence.

---

**Tip:** Strings are everywhere in programming. Try using different methods to see how they change your text! 