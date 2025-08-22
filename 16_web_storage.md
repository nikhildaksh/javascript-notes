# 16. Web Storage

## Theory
Web Storage lets you store data in the browser so it stays even if you refresh the page (localStorage) or until you close the tab (sessionStorage).
- **localStorage:** Stores data with no expiration. Data stays even after closing the browser.
- **sessionStorage:** Stores data for one tab. Data is lost when the tab is closed.
- Both use methods: `setItem` (save), `getItem` (read), `removeItem` (delete one), `clear` (delete all).

---

## Practical Examples

### 1. localStorage
```js
// Save data
localStorage.setItem('username', 'Amit');
// Get data
let user = localStorage.getItem('username');
console.log(user); // 'Amit'
// Remove data
localStorage.removeItem('username');
// Clear all data
localStorage.clear();
```

### 2. sessionStorage
```js
// Save data
sessionStorage.setItem('color', 'blue');
// Get data
let color = sessionStorage.getItem('color');
console.log(color); // 'blue'
// Remove data
sessionStorage.removeItem('color');
// Clear all data
sessionStorage.clear();
```

---

## Practice Questions
1. Save your name in localStorage and print it in the console.
2. Save your favorite color in sessionStorage and print it in the console.
3. Remove a value from localStorage and check if it is gone.
4. Use `clear()` to delete all data from sessionStorage.
5. What is the difference between localStorage and sessionStorage?

---

**Tip:** Web Storage is useful for saving user preferences or login info. Try using it in your own small projects! 