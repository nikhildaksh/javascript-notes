# 17. Timers

## Theory
Timers let you run code after a delay or again and again at regular intervals. JavaScript gives you special functions for this:
- **setTimeout:** Runs code once after a set time (in milliseconds).
- **setInterval:** Runs code again and again after every set time.
- **clearTimeout:** Stops a timeout before it runs.
- **clearInterval:** Stops an interval from repeating.

---

## Practical Examples

### 1. setTimeout
```js
setTimeout(function() {
  console.log('This runs after 2 seconds');
}, 2000); // 2000 ms = 2 seconds
```

### 2. setInterval
```js
let count = 1;
let intervalId = setInterval(function() {
  console.log('Count:', count);
  count++;
  if (count > 5) {
    clearInterval(intervalId); // Stop after 5 times
  }
}, 1000); // Runs every 1 second
```

### 3. clearTimeout
```js
let timeoutId = setTimeout(function() {
  console.log('You will not see this');
}, 3000);
clearTimeout(timeoutId); // Cancels the timeout
```

---

## Practice Questions
1. Use `setTimeout` to print "Hello after 3 seconds" in the console.
2. Use `setInterval` to print numbers from 1 to 5, one every second.
3. How do you stop a repeating interval? Try it in code.
4. Set a timeout and then cancel it before it runs.
5. What is the difference between `setTimeout` and `setInterval`?

---

**Tip:** Timers are useful for animations, reminders, and repeating tasks. Try changing the time values and see what happens! 