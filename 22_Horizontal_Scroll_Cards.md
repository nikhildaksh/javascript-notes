
# Horizontal Scroll Cards with Button Click

This document explains how to create a horizontally scrolling set of cards, where clicking a button scrolls two cards at a time.

---

## HTML Code

```html
<div class="scroll-buttons">
  <button onclick="scrollLeft()">⬅ Close</button>
  <button onclick="scrollRight()">➡ Close</button>
</div>

<div id="cardContainer" class="scroll-container">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
  <div class="card">Card 4</div>
  <div class="card">Card 5</div>
  <div class="card">Card 6</div>
  <div class="card">Card 7</div>
</div>
```

---

## CSS Code

```css
.scroll-container {
  display: flex;
  overflow-x: auto;
  scroll-behavior: smooth;
  gap: 16px;
  padding: 10px;
  max-width: 100%;
}

.card {
  min-width: 200px;
  height: 120px;
  background: #4f46e5;
  color: white;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
}

.scroll-buttons {
  margin: 10px 0;
}

button {
  margin-right: 10px;
  padding: 6px 12px;
}
```

---

## JavaScript Code

```javascript
const container = document.getElementById('cardContainer');

// Card width + gap = 200 + 16 = 216
const cardWidth = 200;
const gap = 16;
const scrollAmount = (cardWidth + gap) * 2; // Scroll 2 cards at a time

function scrollLeft() {
  container.scrollLeft -= scrollAmount;
}

function scrollRight() {
  container.scrollLeft += scrollAmount;
}
```
