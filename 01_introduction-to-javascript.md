# Introduction to JavaScript

## What is JavaScript?

JavaScript is a high-level, versatile programming language that is
mainly used to make web pages interactive. It can manipulate HTML, CSS,
and handle events, making websites dynamic and user-friendly.

## History & Use in Web Development

-   JavaScript was created in **1995** by Brendan Eich while working at
    Netscape.
-   Originally designed for adding interactivity to websites.
-   Over time, it became one of the core technologies of the web, along
    with HTML and CSS.
-   Today, JavaScript is used in:
    -   Frontend development (in browsers)
    -   Backend development (with Node.js)
    -   Mobile apps, desktop apps, and even game development.

## JavaScript in Browser vs Node.js

-   **In Browser**:\
    JavaScript is mainly used for manipulating the DOM, handling user
    interactions, making network requests (AJAX/fetch), and adding
    animations or effects.

-   **In Node.js**:\
    JavaScript can be executed outside the browser. Node.js allows
    developers to build server-side applications, work with databases,
    file systems, and create APIs.

## How JS Code Runs (Execution Context)

-   JavaScript runs inside an **Execution Context**.\
-   The **Global Execution Context (GEC)** is created when the program
    starts.
-   Every function call creates its own **Function Execution Context
    (FEC)**.
-   Execution happens in two phases:
    1.  **Creation Phase** → Memory is allocated for variables and
        functions.
    2.  **Execution Phase** → Code is executed line by line.
-   The **Call Stack** manages the order of execution of these contexts.


## JavaScript Implementation Methods

There are three main ways to use JavaScript in a web page:

1. **Inline JavaScript**  
   JavaScript is written directly inside an HTML element’s attribute.

   ```html
   <button onclick="alert('Hello World!')">Click Me</button>
   ```

2. **Internal JavaScript**  
   JavaScript is written inside the `<script>` tag in the HTML file.

   ```html
   <script>
     console.log("Hello from Internal JavaScript!");
   </script>
   ```

3. **External JavaScript**  
   JavaScript code is written in a separate `.js` file and linked to the HTML.

   ```html
   <script src="app.js"></script>
   ```

---

## JavaScript Comments

Comments are used to make code more readable and to explain what the code does. They are ignored by the JavaScript engine.

1. **Single-line Comment**

   ```javascript
   // This is a single-line comment
   let x = 10; // Variable x stores the value 10
   ```

2. **Multi-line Comment**

   ```javascript
   /*
     This is a multi-line comment.
     It can span multiple lines.
   */
   let y = 20;
   ```
