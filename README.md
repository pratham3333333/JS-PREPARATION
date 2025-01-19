# JavaScript Scenario-Based Questions with Answers

### Table of Contents
1. **Introduction and History of JavaScript**
2. **Syntax and Overview**
3. **JavaScript Implementation**
4. **Using HTML Tags in JavaScript**
5. **Variables in JavaScript**
6. **Operators**
7. **Conditional Statements**
8. **Alert, Confirm, and Prompt Boxes**
9. **Functions**
10. **Loops**
11. **Arrays**
12. **Objects**
13. **String Methods**
14. **Number Methods**
15. **Math Methods**
16. **Date Methods**
17. **DOM Manipulation**
18. **Event Handling**
19. **ES6 Features**

---

### 1. Introduction and History of JavaScript

**Scenario 1**: Describe the origin of JavaScript and its purpose.

**Answer**: JavaScript was created by Brendan Eich in 1995 at Netscape. Initially named Mocha, then LiveScript, it was finally renamed JavaScript. It was designed for client-side interactivity in web pages.

**Scenario 2**: Explain how JavaScript differs from Java.

**Answer**: JavaScript is a lightweight, interpreted language primarily for web applications, while Java is a compiled, object-oriented programming language for various platforms.

**Scenario 3**: What is ECMAScript?

**Answer**: ECMAScript is the standardized version of JavaScript defined by ECMA International. It ensures consistency across different implementations.

**Scenario 4**: Mention three major JavaScript frameworks or libraries and their purposes.

**Answer**: React.js (UI building), Angular (full-fledged framework), and Vue.js (progressive framework).

---

### 2. Syntax and Overview

**Scenario 1**: Write a script to print "Welcome to JavaScript" in the console.

```javascript
console.log("Welcome to JavaScript");
```

**Scenario 2**: Demonstrate variable declaration with `let` and `const`.

```javascript
let age = 25;
const name = "John";
```

**Scenario 3**: What are comments in JavaScript? Provide examples of single-line and multi-line comments.

```javascript
// Single-line comment
/* Multi-line 
   comment */
```

**Scenario 4**: Explain the importance of semicolons in JavaScript.

**Answer**: Semicolons end statements to prevent automatic semicolon insertion errors.

---

### 3. JavaScript Implementation

**Scenario 1**: Include an external JavaScript file in an HTML document.

```html
<script src="app.js"></script>
```

**Scenario 2**: Write inline JavaScript to display an alert box.

```html
<button onclick="alert('Hello!')">Click Me</button>
```

**Scenario 3**: How can you use JavaScript within a `<head>` tag?

```html
<head>
    <script>
        console.log("Script in head");
    </script>
</head>
```

**Scenario 4**: What is the best practice for placing script tags?

**Answer**: Place `<script>` tags before the closing `</body>` to ensure the DOM is loaded before JavaScript executes.

---

### 4. Using HTML Tags in JavaScript

**Scenario 1**: Dynamically add a heading to a webpage.

```javascript
const heading = document.createElement("h1");
heading.textContent = "Dynamic Heading";
document.body.appendChild(heading);
```

**Scenario 2**: Change the text of a button using JavaScript.

```javascript
document.getElementById("myButton").textContent = "Clicked!";
```

**Scenario 3**: Remove an element from the DOM.

```javascript
const element = document.getElementById("myElement");
element.remove();
```

**Scenario 4**: How do you change the background color of a div?

```javascript
document.getElementById("myDiv").style.backgroundColor = "blue";
```

---

### 5. Variables in JavaScript

**Scenario 1**: Declare a variable with `var` and assign a value.

```javascript
var city = "New York";
```

**Scenario 2**: Explain block scope using `let`.

```javascript
{
    let x = 10;
    console.log(x); // 10
}
// console.log(x); // Error
```

**Scenario 3**: Demonstrate constant declaration with `const`.

```javascript
const PI = 3.14;
```

**Scenario 4**: Explain hoisting with `var`.

```javascript
console.log(a); // undefined
var a = 5;
```

---

### 6. Operators

**Scenario 1**: Write a script to calculate the square of a number using the multiplication operator.

```javascript
const num = 4;
console.log(num * num);
```

**Scenario 2**: Demonstrate the use of the ternary operator.

```javascript
const age = 18;
const canVote = age >= 18 ? "Yes" : "No";
console.log(canVote);
```

**Scenario 3**: Use logical operators to check if a number is within a range.

```javascript
const num = 10;
if (num > 0 && num < 20) {
    console.log("Within range");
}
```

**Scenario 4**: Demonstrate the use of bitwise AND.

```javascript
console.log(5 & 1); // 1
```

---

### 7. Conditional Statements

**Scenario 1**: Use an `if` statement to check if a number is positive.

```javascript
if (num > 0) {
    console.log("Positive number");
}
```

**Scenario 2**: Use `if-else` to check if a number is even or odd.

```javascript
if (num % 2 === 0) {
    console.log("Even");
} else {
    console.log("Odd");
}
```

**Scenario 3**: Use `if-else if-else` to grade a student.

```javascript
if (marks >= 90) {
    console.log("A grade");
} else if (marks >= 75) {
    console.log("B grade");
} else {
    console.log("C grade");
}
```

**Scenario 4**: Use a `switch` to check the type of fruit.

```javascript
switch (fruit) {
    case "Apple":
        console.log("Red fruit");
        break;
    case "Banana":
        console.log("Yellow fruit");
        break;
    default:
        console.log("Unknown fruit");
}
```

---


### 8. Alert, Confirm, and Prompt Boxes

**Scenario 1**: Show an alert box with a welcome message.

```javascript
alert("Welcome to our website!");
```

**Scenario 2**: Display a confirmation box asking the user if they want to continue.

```javascript
const userConfirmed = confirm("Do you want to proceed?");
console.log(userConfirmed); // true or false
```

**Scenario 3**: Prompt the user for their name and display it in the console.

```javascript
const userName = prompt("Enter your name:");
console.log(`Hello, ${userName}!`);
```

**Scenario 4**: Use a prompt to take a number input and calculate its square.

```javascript
const number = prompt("Enter a number:");
const square = number * number;
alert(`The square of ${number} is ${square}`);
```

---

### 9. Functions

**Scenario 1**: Create a function to calculate the sum of two numbers.

```javascript
function sum(a, b) {
    return a + b;
}
console.log(sum(5, 10));
```

**Scenario 2**: Write a function to check if a number is even or odd.

```javascript
function isEven(number) {
    return number % 2 === 0 ? "Even" : "Odd";
}
console.log(isEven(7));
```

**Scenario 3**: Demonstrate a function with default parameters.

```javascript
function greet(name = "Guest") {
    console.log(`Hello, ${name}!`);
}
greet();
greet("Alice");
```

**Scenario 4**: Create an arrow function to calculate the area of a rectangle.

```javascript
const area = (length, width) => length * width;
console.log(area(5, 10));
```

---

### 10. Loops

**Scenario 1**: Use a `while` loop to print numbers from 1 to 5.

```javascript
let i = 1;
while (i <= 5) {
    console.log(i);
    i++;
}
```

**Scenario 2**: Demonstrate a `do-while` loop to collect user input until it matches a condition.

```javascript
let password;
do {
    password = prompt("Enter the password:");
} while (password !== "1234");
alert("Access granted!");
```

**Scenario 3**: Use a `for` loop to print the multiplication table of a number.

```javascript
const number = 3;
for (let i = 1; i <= 10; i++) {
    console.log(`${number} x ${i} = ${number * i}`);
}
```

**Scenario 4**: Create a nested loop to print a 3x3 grid.

```javascript
for (let i = 1; i <= 3; i++) {
    let row = "";
    for (let j = 1; j <= 3; j++) {
        row += "* ";
    }
    console.log(row);
}
```

---

### 11. Arrays

**Scenario 1**: Declare an array and print its elements using `forEach`.

```javascript
const fruits = ["Apple", "Banana", "Cherry"];
fruits.forEach((fruit) => console.log(fruit));
```

**Scenario 2**: Add and remove elements using `push` and `pop`.

```javascript
const numbers = [1, 2, 3];
numbers.push(4);
console.log(numbers); // [1, 2, 3, 4]
numbers.pop();
console.log(numbers); // [1, 2, 3]
```

**Scenario 3**: Use `shift` and `unshift` to manipulate an array.

```javascript
const queue = ["First", "Second", "Third"];
queue.shift();
console.log(queue); // ["Second", "Third"]
queue.unshift("New First");
console.log(queue); // ["New First", "Second", "Third"]
```

**Scenario 4**: Combine two arrays using `concat`.

```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combined = arr1.concat(arr2);
console.log(combined); // [1, 2, 3, 4, 5, 6]
```

---

### 12. Objects

**Scenario 1**: Create an object representing a person and access its properties.

```javascript
const person = {
    name: "John",
    age: 30,
    job: "Developer",
};
console.log(person.name);
console.log(person.age);
```

**Scenario 2**: Add and delete properties of an object.

```javascript
const car = { brand: "Toyota", model: "Corolla" };
car.year = 2020;
delete car.model;
console.log(car);
```

**Scenario 3**: Use a method inside an object.

```javascript
const calculator = {
    add(a, b) {
        return a + b;
    },
};
console.log(calculator.add(5, 10));
```

**Scenario 4**: Loop through an object’s properties using `for-in`.

```javascript
const book = { title: "1984", author: "George Orwell", year: 1949 };
for (let key in book) {
    console.log(`${key}: ${book[key]}`);
}
```

---

---

### 13. String Methods

**Scenario 1**: Convert a string to uppercase and lowercase.

```javascript
const text = "Hello, World!";
console.log(text.toUpperCase()); // "HELLO, WORLD!"
console.log(text.toLowerCase()); // "hello, world!"
```

**Scenario 2**: Find the index of a substring in a string.

```javascript
const sentence = "The quick brown fox jumps over the lazy dog.";
console.log(sentence.indexOf("fox")); // 16
```

**Scenario 3**: Extract a portion of a string using `slice`.

```javascript
const greeting = "Good Morning!";
console.log(greeting.slice(0, 4)); // "Good"
```

**Scenario 4**: Replace part of a string with another string.

```javascript
const phrase = "I love JavaScript!";
console.log(phrase.replace("JavaScript", "coding")); // "I love coding!"
```

---

### 14. Number Methods

**Scenario 1**: Convert a string to a number.

```javascript
const strNum = "42";
console.log(Number(strNum)); // 42
```

**Scenario 2**: Fix a number to two decimal places.

```javascript
const num = 5.6789;
console.log(num.toFixed(2)); // "5.68"
```

**Scenario 3**: Parse a floating-point number.

```javascript
const floatString = "3.14";
console.log(parseFloat(floatString)); // 3.14
```

**Scenario 4**: Parse an integer.

```javascript
const intString = "42";
console.log(parseInt(intString)); // 42
```

---

### 15. Math Methods

**Scenario 1**: Round a number to the nearest integer.

```javascript
console.log(Math.round(4.5)); // 5
console.log(Math.round(4.4)); // 4
```

**Scenario 2**: Generate a random number between 0 and 1.

```javascript
console.log(Math.random());
```

**Scenario 3**: Find the maximum and minimum of a set of numbers.

```javascript
console.log(Math.max(1, 5, 10, 20)); // 20
console.log(Math.min(1, 5, 10, 20)); // 1
```

**Scenario 4**: Calculate the square root of a number.

```javascript
console.log(Math.sqrt(16)); // 4
```

---

### 16. Date Methods

**Scenario 1**: Get the current date and time.

```javascript
const now = new Date();
console.log(now);
```

**Scenario 2**: Extract the year, month, and day from a date.

```javascript
const today = new Date();
console.log(today.getFullYear()); // e.g., 2025
console.log(today.getMonth()); // 0-based month index
console.log(today.getDate());
```

**Scenario 3**: Set a specific date.

```javascript
const specificDate = new Date("2025-01-01");
console.log(specificDate);
```

**Scenario 4**: Compare two dates.

```javascript
const date1 = new Date("2025-01-01");
const date2 = new Date("2025-01-02");
console.log(date1 < date2); // true
```

---

### 17. DOM Manipulation

**Scenario 1**: Change the content of an HTML element.

```javascript
document.getElementById("myElement").innerText = "New Content!";
```

**Scenario 2**: Change the style of an HTML element.

```javascript
document.getElementById("myElement").style.color = "red";
```

**Scenario 3**: Add a new HTML element to the DOM.

```javascript
const newElement = document.createElement("p");
newElement.innerText = "I am a new paragraph!";
document.body.appendChild(newElement);
```

**Scenario 4**: Remove an HTML element from the DOM.

```javascript
const elementToRemove = document.getElementById("removeMe");
elementToRemove.parentNode.removeChild(elementToRemove);
```

---

### 18. Event Handling

**Scenario 1**: Add an event listener to a button.

```javascript
document.getElementById("myButton").addEventListener("click", () => {
    alert("Button clicked!");
});
```

**Scenario 2**: Handle the `mouseover` event.

```javascript
document.getElementById("hoverMe").addEventListener("mouseover", () => {
    console.log("Mouse is over!");
});
```

**Scenario 3**: Prevent the default behavior of a form submission.

```javascript
document.getElementById("myForm").addEventListener("submit", (event) => {
    event.preventDefault();
    alert("Form submission prevented!");
});
```

**Scenario 4**: Use event delegation to handle clicks on multiple elements.

```javascript
document.getElementById("parent").addEventListener("click", (event) => {
    if (event.target && event.target.matches(".child")) {
        console.log("Child element clicked!");
    }
});
```

---

### 19. ES6 Features

**Scenario 1**: Use `let` and `const` instead of `var`.

```javascript
let name = "John";
const age = 30;
console.log(name, age);
```

**Scenario 2**: Use template literals for string interpolation.

```javascript
const firstName = "John";
const lastName = "Doe";
console.log(`Hello, ${firstName} ${lastName}!`);
```

**Scenario 3**: Use arrow functions.

```javascript
const add = (a, b) => a + b;
console.log(add(5, 10));
```

**Scenario 4**: Use the spread operator to merge arrays.

```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combined = [...arr1, ...arr2];
console.log(combined); // [1, 2, 3, 4, 5, 6]
```

---


