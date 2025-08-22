# 19. Fetch API

## Theory
The Fetch API lets you get data from servers (like APIs) using JavaScript. It is used to make HTTP requests (like GET, POST). Fetch returns a promise, so you can use `.then()` or `async/await` to handle the response. You often need to convert the response to JSON. Always handle errors in case something goes wrong.

---

## Practical Examples

### 1. Basic fetch() with .then()
```js
fetch('https://jsonplaceholder.typicode.com/posts/1')
  .then(response => response.json())
  .then(data => {
    console.log(data); // The fetched data
  })
  .catch(error => {
    console.error('Error:', error);
  });
```

### 2. fetch() with async/await
```js
async function getPost() {
  try {
    let response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Fetch error:', error);
  }
}
getPost();
```

### 3. Handling HTTP Errors
```js
async function fetchData() {
  try {
    let response = await fetch('https://jsonplaceholder.typicode.com/invalid-url');
    if (!response.ok) {
      throw new Error('HTTP error! Status: ' + response.status);
    }
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error.message);
  }
}
fetchData();
```

---

## Practice Questions
1. Use `fetch()` to get data from any public API and print it in the console.
2. Rewrite a fetch example using `async/await`.
3. How do you handle errors when using fetch?
4. What does `response.json()` do?
5. Try fetching from an invalid URL and handle the error.

---

**Tip:** Fetch is very useful for working with APIs. Always handle errors to make your app reliable! 