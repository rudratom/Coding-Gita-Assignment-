# Assignment: Introduction to JavaScript

## Section A: Short Answer Questions

### Q1. What is JavaScript?

JavaScript is a programming language used to make websites interactive and dynamic. For example, it can be used for buttons, forms, animations, and other interactive features on a website.

### Q2. Who created JavaScript and in which year?

JavaScript was created by **Brendan Eich in 1995** while he was working at Netscape.

### Q3. What was the original name of JavaScript?

The original name of JavaScript was **Mocha**. Later, it was changed to **LiveScript** and then to JavaScript.

### Q4. Is JavaScript the same as Java? Give one major difference.

No, JavaScript and Java are two different programming languages. Java is mainly used for general-purpose applications, while JavaScript is widely used to make websites interactive.

### Q5. What does it mean when we say JavaScript is a high-level programming language?

It means JavaScript is easy for humans to read and write. We don't have to deal directly with complicated computer hardware or memory details while writing JavaScript code.

### Q6. Is JavaScript a compiled language or an interpreted language? Explain briefly.

JavaScript is generally considered an **interpreted language** because the code can be executed by the JavaScript engine without first creating a separate executable file. Modern JavaScript engines also use **JIT compilation** to make the code run faster.

### Q7. Name the JavaScript engines used by the following browsers:

* **Google Chrome:** V8
* **Mozilla Firefox:** SpiderMonkey
* **Apple Safari:** JavaScriptCore

### Q8. What is Dynamic Typing in JavaScript?

Dynamic typing means that a variable in JavaScript does not have to be of only one data type. The same variable can store different types of values.

For example:

```javascript
let x = 10;
x = "Hello";
```

Here, `x` first stores a number and later stores a string.

### Q9. What is the main difference between a static website and a dynamic website?

A **static website** mostly shows fixed content that does not change often.

A **dynamic website** can change its content depending on the user, data, or user actions. For example, a social media website is dynamic.

### Q10. Name the three pillars of Front-end Web Development and write one line about each.

The three main pillars are:

1. **HTML:** It is used to create the structure of a webpage.
2. **CSS:** It is used to add styling and make the webpage look better.
3. **JavaScript:** It is used to add interaction and functionality to the webpage.

### Q11. What is the difference between Frontend and Backend?

**Frontend** is the part of a website that we can see and interact with, like buttons, text, images, and forms.

**Backend** is the part that works behind the website. It handles things like servers, databases, and processing data.

### Q12. What is Node.js?

Node.js is a runtime environment that allows us to run JavaScript outside of a web browser. It is commonly used to create backend applications and servers.

### Q13. Explain ECMAScript. What is its relation with JavaScript?

ECMAScript is a standard that defines how scripting languages should work. JavaScript follows the ECMAScript standard. In simple words, **ECMAScript is the standard, and JavaScript is one of the languages that follows that standard.**
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Section B: True or False

### 1. JavaScript is a statically typed language.

**False.** JavaScript is a **dynamically typed language**.

### 2. JavaScript can only run inside the browser.

**False.** JavaScript can run inside browsers as well as outside browsers using environments like **Node.js**.

### 3. HTML is responsible for the behaviour of a webpage.

**False.** HTML is mainly responsible for the **structure and content** of a webpage. JavaScript is mainly used to add behaviour and interaction.

### 4. Node.js allows JavaScript to run outside the browser.

**True.**

### 5. JavaScript is case-insensitive.

**False.** JavaScript is **case-sensitive**, which means uppercase and lowercase letters are treated differently.

### 6. `let name` and `let Name` are the same variable.

**False.** `name` and `Name` are **different variables** because JavaScript is case-sensitive.

### 7. ECMAScript is a programming language.

**False.** ECMAScript is a **standard/specification** that defines the rules and features followed by JavaScript and other implementations.

### 8. React, Angular, and Vue.js are used for Backend development.

**False.** React, Angular, and Vue.js are mainly used for **Frontend development**.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Section C: Fill in the Blanks

1. JavaScript was created by **Brendan Eich** in the year **1995**.

2. The three technologies used in Front-end development are **HTML, CSS, and JavaScript**.

3. JavaScript engines: Chrome uses **V8**, Firefox uses **SpiderMonkey**.

4. In the restaurant analogy: Customer = **Frontend/User**, Waiter = **Backend/API**, Chef = **Server**.

5. JavaScript file extension is **`.js`**.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Section D: Conceptual Questions (2 Marks each)

**Q14.** Differentiate between a **static website** and a **dynamic website**. Give one real-world example of each.

**Q15.** Explain any two features of JavaScript that make it suitable for creating interactive web pages.

**Q16.** List any four areas (apart from web browsers) where JavaScript is used today. Mention one popular framework/library for each (if applicable).

**Q17.** What is the difference between writing JavaScript code:
- Inside an HTML file using `<script>` tag, and
- In an external `.js` file?  
Mention two advantages of using an external JavaScript file.

**Q18.** Explain the difference between Frontend and Backend using the **restaurant analogy** in your own words.

**Q19.** Why should a beginner learn JavaScript? Write at least 4 points.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Section E: Code-Based Questions

## Q20. Predict the output of the following code and explain why:

```javascript
let value = 25;
console.log(typeof value);

value = "JavaScript";
console.log(typeof value);

value = false;
console.log(typeof value);
```

### Output:
<img width="961" height="191" alt="image" src="https://github.com/user-attachments/assets/c015a315-79c9-435e-8da4-2a6a60369770" />


```text
number
string
boolean
```

### Explanation:

JavaScript is **dynamically typed**, so the same variable can store different types of values.

* `25` is a **number**, so `typeof value` gives `number`.
* `"JavaScript"` is a **string**, so it gives `string`.
* `false` is a **boolean**, so it gives `boolean`.

---

## Q21. Write a simple HTML + JavaScript program that displays an alert box with the message "Welcome to JavaScript!" when a button is clicked.

```html
<!DOCTYPE html>
<html>
<head>
    <title>JavaScript Alert</title>
</head>
<body>

    <button onclick="showMessage()">Click Me</button>

    <script>
        function showMessage() {
            alert("Welcome to JavaScript!");
        }
    </script>

</body>
</html>
```

### Explanation:

When the user clicks the button, the `showMessage()` function runs and displays the alert message.

---

## Q22. Write JavaScript code to demonstrate event-driven programming.

When the user clicks the button, the paragraph text will change.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Event Driven Programming</title>
</head>
<body>

    <button id="myBtn">Click Me</button>

    <p id="demo">Original text</p>

    <script>
        let button = document.getElementById("myBtn");

        button.onclick = function() {
            document.getElementById("demo").innerHTML = "Button was clicked!";
        };
    </script>

</body>
</html>
```
<img width="973" height="401" alt="image" src="https://github.com/user-attachments/assets/7ee4e549-388d-4056-8882-45a07c3a8c57" />

### Explanation:

Here, clicking the button is the **event**. When the event happens, JavaScript changes the text of the paragraph from `"Original text"` to `"Button was clicked!"`.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Section F: Practical / Application Based
Q23. Complete HTML + JavaScript Program
<!DOCTYPE html>
<html>
<head>
    <title>My First JavaScript Page</title>
</head>

<body>

    <h1>My First JavaScript Page</h1>

    <button onclick="changePage()">Click Me</button>

    <script>
        console.log("JavaScript is running successfully!");

        function changePage() {
            alert("Hello, B.Tech Student!");
            document.body.style.backgroundColor = "lightblue";
        }
    </script>

</body>
</html>

output:
<img width="1071" height="401" alt="image" src="https://github.com/user-attachments/assets/f10268c2-a6c2-417c-8c12-616b206b22d1" />
<img width="1132" height="439" alt="image" src="https://github.com/user-attachments/assets/6c10dd61-cbeb-4f3a-a748-a357a1352a27" />
<img width="1157" height="452" alt="image" src="https://github.com/user-attachments/assets/8ff5ee91-6299-4d9a-bb1c-1cd9416432f4" />

Explanation:
The <h1> displays the heading "My First JavaScript Page".
The button calls the changePage() function when clicked.
The function shows the alert "Hello, B.Tech Student!".
It also changes the background color of the page to light blue.
console.log() prints "JavaScript is running successfully!" in the browser console.



----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Section G: Higher Order Thinking

## Q24. Why did JavaScript become so popular and multipurpose?

JavaScript became popular because it was easy to learn and could be used to make websites interactive. Later, its use was not limited to browsers.

**Node.js** made it possible to run JavaScript outside the browser, so developers could use it for backend and server-side development. JavaScript is also used with different frameworks and tools to make mobile and desktop applications.

**ECMAScript** updates added new features and improvements to JavaScript over time. Because of these updates and the development of new tools and frameworks, JavaScript became useful for many different types of applications, including AI/ML projects.

Overall, JavaScript became popular because it is flexible, has a large community, and can be used for many different types of development.


