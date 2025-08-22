# 15. JavaScript in Browser (DOM)

## Theory
The DOM (Document Object Model) is a way for JavaScript to interact with web pages. The browser makes a tree-like structure of your HTML, and you can use JavaScript to read or change anything on the page.
- **window:** The main browser object (represents the whole browser window).
- **document:** Represents the web page loaded in the browser.
- **DOM tree:** The structure of all elements on the page (like a family tree).
- **DOM selection:** You can select elements using methods like `getElementById` or `querySelector`.
- **Modifying elements/attributes:** You can change text, HTML, or attributes of elements.
- **Event handling:** You can run code when users click, type, or interact with the page (using `onclick`, `addEventListener`, etc.).

---

## Practical Examples

### 1. window and document
```js
console.log(window.innerWidth); // Width of the browser window
console.log(document.title); // Title of the web page
```

### 2. DOM Selection
```js
// HTML: <p id="demo">Hello</p>
let para = document.getElementById('demo');
console.log(para.textContent); // 'Hello'

// HTML: <div class="box"></div>
let box = document.querySelector('.box');
```

### 3. Modifying Elements and Attributes
```js
// Change text
para.textContent = 'Hi there!';

// Change HTML
box.innerHTML = '<b>Bold Text</b>';

// Change attribute
box.setAttribute('style', 'color: red;');
```

### 4. Event Handling
```js
// HTML: <button id="btn">Click me</button>
let btn = document.getElementById('btn');

// Method 1: onclick
btn.onclick = function() {
  alert('Button clicked!');
};

// Method 2: addEventListener
btn.addEventListener('click', function() {
  console.log('Button was clicked!');
});
```

### 5. Event Bubbling and Delegation
```js
// HTML: <ul id="list"><li>Item 1</li><li>Item 2</li></ul>
let list = document.getElementById('list');
list.addEventListener('click', function(event) {
  if (event.target.tagName === 'LI') {
    alert('You clicked: ' + event.target.textContent);
  }
});
```

---

## Practice Questions
1. Select a paragraph by its ID and change its text using JavaScript.
2. Use `querySelector` to select a div with class "container" and change its background color.
3. Add a click event to a button that shows an alert.
4. Change the value of an input field using JavaScript.
5. Use event delegation to handle clicks on all list items in a `<ul>`.
6. What is the difference between `onclick` and `addEventListener`?

---

**Tip:** Open your browser's console and try selecting and changing elements on any web page for practice! 