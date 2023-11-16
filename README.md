# Homework-1

## 📅 History of Javascript

#### 1995 - Birth of JavaScript:

JavaScript was created by Brendan Eich in just 10 days while working at Netscape Communications. It was initially called "Mocha" and later renamed "LiveScript."

#### 1996 - JavaScript 1.1

Netscape introduced JavaScript 1.1 with several enhancements. It gained popularity as a client-side scripting language for web development.

#### 1997 - ECMAScript Standardization

Netscape submitted JavaScript to the Ecma International organization for standardization. This led to the creation of ECMAScript, the standardized specification for JavaScript.

#### 1999 - ECMAScript 3

ECMAScript 3 was released, bringing many important features, making it the foundation for modern JavaScript.

#### 2005 - AJAX Revolution

The term AJAX (Asynchronous JavaScript and XML) was coined, highlighting the use of JavaScript for creating interactive web applications without full page reloads. This marked a significant turning point in web development.

#### 2006 - ECMAScript 4 Abandoned

A proposed major update to ECMAScript, known as ECMAScript 4, was abandoned due to disagreements within the community. This led to a focus on smaller, incremental updates.

#### 2009 - ECMAScript 5

ECMAScript 5 was released with new features and improvements, making JavaScript a more robust and versatile language.

#### 2015 - ECMAScript 6 (ES2015)

This major update introduced several new features, including arrow functions, classes, and the let and const keywords. It marked a significant step forward in JavaScript's evolution.

#### 2017 - ECMAScript 8 (ES2017)

ES2017 brought new features like async/await for handling asynchronous code more elegantly, and improvements to regular expressions.

#### 2020 - ECMAScript 11 (ES2020)

The latest major update at the time of my last knowledge update brought features like optional chaining and nullish coalescing operators, improving JavaScript's expressiveness and error handling.

## 🧊 Differences between Js and Java

#### Type:

Java is an object-oriented programming (OOP) language commonly used across a broad spectrum, including server-side applications, desktop applications, and mobile applications.
JavaScript is a scripting language primarily used in client-side applications that run within web browsers.

#### Runtime Environment:

Java typically requires an independent runtime environment called Java Virtual Machine (JVM). Java applications run on a JVM.
JavaScript is directly supported by web browsers. Browsers have integrated JavaScript engines to interpret and execute JavaScript code.

#### Syntax and Structure:

Java's syntax is similar to C++. It is a statically typed language with predetermined variable types and type safety.
JavaScript has a syntax similar to C and Java but is dynamically typed. This means variable types are determined at runtime.

#### Use Cases:

Java is preferred for large-scale, complex, multi-user applications. It is used in a wide range of applications from large-scale enterprise applications to games.
JavaScript is used in client-side applications within web browsers. It is commonly employed to make web pages interactive, update user interfaces, and develop web applications.

#### Object Model:

Java is known for its strict object-oriented nature. Everything is an object, and it is class-based.
JavaScript uses a prototype-based object-oriented model, where objects are derived from prototypes.

## 🕹️ Explain Data Types in Javascript.

#### Number:

Used to represent numeric values, including integers and floating-point numbers.

#### String:

Used to represent text data, a sequence of characters.

#### Boolean:

Represents true or false values and is commonly used in conditional statements.

#### Object:

Complex data type that can contain properties and methods.

#### Array:

Represents an ordered list of values, and each value can be accessed using an index.

#### Null:

Represents the intentional absence of any object value.

#### Undefined:

Indicates that a variable has been declared but has not been assigned a value.

#### Symbol:

Introduced in ECMAScript 2015 (ES6), represents a unique and immutable data type.

## 🎃 Differences between Null and Undefined

#### null:

- It is a special value that represents the intentional absence of any object value.
- When a variable is assigned the value null, it means that the variable has no object, array, or function assigned to it.
- It is often used as a placeholder to indicate that a variable or object property intentionally does not have a meaningful value.

#### undefined:

- It is a primitive value automatically assigned to variables that have been declared but have not yet been assigned a value.
- It is the default value of function parameters that are not provided when the function is called.
- It can also be the result of an expression or statement that does not explicitly return a value.

## 🎏 What is NaN

- NaN stands for "Not a Number" in JavaScript. It is a special value indicating the result of a mathematical operation that should return a valid number but doesn't. NaN is often the result of operations involving undefined or non-numeric values and serves as a signal for errors in numeric calculations. You can check for NaN using the isNaN() function, but care should be taken as it can return true for values that are not strictly NaN.

## 🛹 How many different ways are there to add a comment line in Javascript?

In JavaScript, there are two main ways to add comments:

#### Single-line Comments:

- Single-line comments are created by using //. Anything following // on the same line is treated as a comment.

```Javascript
// This is a single-line comment
var x = 5; // This is also a single-line comment
```

#### Multi-line Comments:

- Multi-line comments are created by enclosing the comment text between /_ and _/. This allows for comments that span multiple lines.

```Javascript
/*
  This is a multi-line comment
  It can span multiple lines
*/
var y = 10;
```

## 🎡 Explain what global variable means

- A global variable in JavaScript is a variable declared outside any function or block, making it accessible throughout the entire program. It has a global scope, allowing it to be used in functions and code blocks. While convenient for accessibility, overuse of global variables can lead to naming conflicts and maintenance challenges. It is generally advisable to minimize the use of global variables for cleaner and more maintainable code.

## ♾️ Explain what is this keyword in Javascript?

- In JavaScript, the this keyword is a special identifier that refers to the current instance of an object in which the code is being executed. The value of this is dynamically determined based on how a function is invoked, and it can have different values in different contexts.

## ♾🪩 Explain differences between == and === With Examples ?

In JavaScript, == and === are two different comparison operators that can yield different results. Let's illustrate the difference with examples:

#### == (Loose Equality):

- When comparing two values, it performs type coercion to compare values.

```Javascript
'5' == 5; // true, because it coerces types and compares values
```

#### === (Strict Equality):

- When comparing two values, it checks both values and their types without type coercion.

```Javascript
'5' === 5; // false, because it checks both values and types, and one is a string, the other is a number
```

- In this case, even though the values are equal (5 and '5'), the types are different, so the comparison result is false.

Generally, it's recommended to use === whenever possible because it provides a more accurate comparison by considering both values and types. Especially when you want to ensure that the values and types are exactly the same, === is a safer choice.

## 🥕 Make a table of let var const difference

- **_var_** and **_let_** create variables that can be **_reassigned_** another value.
- **_const_** creates "**_constant_**" variables that cannot be reassigned another value.
- developers shouldn't use **_var_** anymore. They should use **_let_** or **_const_** instead.
- if you're not going to change the value of a variable, it is good practice to use **_const_**.

To analyze the differences between these keywords, We'll be using three factors:

- Scope of variables
- Redeclaration and reassignment
- Hoisting

#### Scope of variables

The scope of a variable defines where in your code that variable can be accessed or modified. Variables can have local scope, limited to a specific block or function, or global scope, accessible from anywhere in the code.

#### Redeclaration and reassignment

Redeclaring a variable within the same scope is generally not allowed in JavaScript, but variables can be reassigned new values. However, if a variable is declared using **_let_** or **_const_**, it can't be redeclared within the same scope.

#### Hoisting

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their containing scope during compilation. This allows you to use variables or functions before they're actually declared in your code, but it's essential to understand how hoisting works to prevent unexpected behavior.

| Keywords    | Scope           | Redeclare | Reassign | Hoisted |
| :---------- | :-------------- | :-------- | -------- | ------- |
| **_var_**   | Global or Local | Yes       | Yes      | Yes     |
| **_const_** | Block           | No        | No       | No      |
| **_let_**   | Block           | No        | Yes      | No      |

## 👒 What are the differences between Arrow function and normal function?

#### Syntax

- Arrow function

```Javascript
const arrowFunction = (param1, param2) => {
  // function body
};
```

- Normal Function

```Javascript
function normalFunction(param1, param2) {
  // function body
}
```

#### this Binding:

Arrow Function:

- Arrow functions do not have their own this context. They inherit the this value from the enclosing lexical scope.

Normal Function:

- Normal functions have their own this context, which is dynamically determined based on how the function is called. It can be affected by how the function is invoked, leading to potential complexities.

#### Arguments Object:

Arrow Function:

- Arrow functions do not have their own arguments object. Instead, they inherit the arguments object from the enclosing scope.

Normal Function:

- Normal functions have their own arguments object, which is an array-like object containing the arguments passed to the function.

#### Binding of this in Methods:

Arrow Function:

- Arrow functions are not suitable for methods within objects where you expect this to refer to the object itself.

Normal Function:

- Normal functions, when used as methods within objects, bind this to the object.

#### Use of new:

Arrow Function:

- Arrow functions cannot be used as constructors with the new keyword.

Normal Function:

- Normal functions can be used as constructors with the new keyword to create instances of objects.

## 🌸 How to define a variable within the switch block without errors?

```Javascript
var dayOfWeek = "Monday";
var message;

switch (dayOfWeek) {
  case "Monday":
    message = "It's Monday!";
    break;
  case "Tuesday":
    message = "It's Tuesday!";
    break;
  // Diğer günler için case'leri buraya ekleyebilirsiniz
  default:
    message = "It's another day.";
}

console.log(message);

```

## ♦️ Explain what pure function means

#### Referential Transparency:

- A function is considered referentially transparent if it consistently produces the same output given the same input values. This means that whenever the function is called with the same inputs at any point in time, it will always yield the same result without any side effects.

#### Lack of Side Effects:

- A function is considered side effect-free if it does not modify variables outside of its scope or cause any other observable effects, such as writing to files or making network requests. Side effects are actions that go beyond computing a result based solely on the input parameters.

## 🧢 What is the rest operator? Explain with an example.

The rest operator in JavaScript allows you to represent an indefinite number of arguments as an array. It is indicated by three dots (...) followed by the name of the array that will contain the rest of the values. The rest parameter must be the last parameter in a function.

```Javascript
// Using the rest operator to gather remaining arguments into an array
function sum(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}

const result = sum(1, 2, 3, 4, 5);
console.log(result); // Output: 15
```

- The sum function is defined with the rest parameter ...numbers, which collects any number of arguments passed to the function into an array called numbers.
- The reduce method is then used to sum up all the values in the numbers array, starting from an initial total of 0.

## 🥽 Explain what object destructuring is with an example.

Object destructuring is a JavaScript feature that allows you to extract values from objects and assign them to variables in a concise and readable way. It provides a shorter syntax for extracting values from objects and can be especially useful when working with functions that return objects.

```Javascript
// Sample object
const person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30,
  address: {
    city: 'New York',
    country: 'USA'
  }
};

// Destructuring assignment
const { firstName, lastName, age, address: { city, country } } = person;

// Using the extracted values
console.log(firstName); // Output: John
console.log(lastName);  // Output: Doe
console.log(age);       // Output: 30
console.log(city);      // Output: New York
console.log(country);   // Output: USA
```

- The person object has properties like firstName, lastName, age, and address.
- The destructuring assignment **{ firstName, lastName, age, address: { city, country } } = person;** extracts these properties from the **person** object and assigns them to corresponding variables.
- After destructuring, you can use the extracted variables directly.

## 🍮 Create an object with 2 elements in 6 different ways

#### Using Object Literal:

```Javascript
const obj1 = { key1: 'value1', key2: 'value2' };
```

#### Using Object Constructor:

```Javascript
const obj2 = new Object();
obj2.key1 = 'value1';
obj2.key2 = 'value2';
```

#### Using Object.create() Method:

```Javascript
const obj3 = Object.create(null);
obj3.key1 = 'value1';
obj3.key2 = 'value2';
```

#### Using Object.assign() Method:

```Javascript
const obj4 = Object.assign({}, { key1: 'value1', key2: 'value2' });
```

#### Using Spread Operator:

```Javascript
const { key1, key2 } = { key1: 'value1', key2: 'value2' };
const obj5 = { key1, key2 };
```

#### Using Dynamic Keys:

```Javascript
const key1 = 'key1';
const key2 = 'key2';
const obj6 = { [key1]: 'value1', [key2]: 'value2' };
```

## 🧿 Create a new object using 2 different loop methods with the number of characters of the key and value values of an object with 2 elements.

You can create a new object by iterating over the keys and values of a two-property object and calculating the character count for each key and value. Here's an example using two different loop methods: for...in loop and Object.entries() with forEach().

```Javascript
// Original object with two properties
const originalObject = {
  key1: 'value123',
  key2: 'value456'
};

// Method 1: Using for...in loop
const newObj1 = {};
for (let key in originalObject) {
  const value = originalObject[key];
  newObj1[key] = { key: key.length, value: value.length };
}

// Method 2: Using Object.entries() and forEach()
const newObj2 = {};
Object.entries(originalObject).forEach(([key, value]) => {
  newObj2[key] = { key: key.length, value: value.length };
});

console.log(newObj1);
console.log(newObj2);
```

- The for...in loop is used to iterate over the keys of the original object.
- The Object.entries() method is used to get an array of **[key, value]** pairs, and the forEach() method is used to iterate over these pairs.
- For each key-value pair, a new object is created with the key length and value length, and it is added to the new object.

## 🏂 Make a table of the differences between cookie, local storage and session storage.

| Feature                 | Cookie                                  | Local Storage                     | Session Storage              |
| ----------------------- | --------------------------------------- | --------------------------------- | ---------------------------- |
| **Data Type**           | Text                                    | Text                              | Text                         |
| **Storage Limit**       | 4 KB                                    | Approximately 5 MB                | Approximately 5 MB           |
| **Persistence**         | Optional                                | Persistent until manually cleared | Lasts for the session        |
| **Scope**               | Domain-wide                             | Domain-wide                       | Domain-wide                  |
| **JavaScript Access**   | Yes                                     | Yes                               | Yes                          |
| **Data Sent to Server** | Automatically included in every request | No                                | No                           |
| **Security**            | Weak                                    | Moderate                          | Moderate                     |
| **Use Case**            | Session Information, Preferences        | Persistent Data Storage           | Session-specific Information |

## 🫗 What is the difference between asynchronous and synchronous operations?

Synchronous operations in programming are executed sequentially, one after the other, with each operation blocking the next until completion. In contrast, asynchronous operations allow the program to initiate tasks and proceed with other operations without waiting for the completion of the initiated tasks. Asynchronous operations are commonly used for tasks that involve waiting for external resources, such as fetching data from a server, to avoid blocking the program's execution.

## 🪮 What is a promise and why do we need it?

A promise in JavaScript is an object that represents the outcome of an asynchronous operation, either its successful completion with a value or its failure with an error. Promises provide a structured and readable way to handle asynchronous code, preventing callback hell and simplifying error management. They support sequential and parallel execution, chaining, and are widely used in modern JavaScript for managing asynchronous tasks.

# ARRAY QUESTIONS

```Javascript
var dolap = ["Shirt", "Pant", "TShirt"];
```

#### Delete the last element in the cabinet array and print it to the console

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];

var removedItem = dolap.pop();

console.log("Modified dolap array:", dolap);
console.log("Removed item:", removedItem);
```

#### Delete the first element in the cabinet array, send the “Hat” element instead and print it to the console.

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];

var removedItem = dolap.shift();
dolap.unshift("Hat");

console.log("Modified dolap array:", dolap);
console.log("Removed item:", removedItem);

```

#### Check if the closet variable is array and set the result equal to a variable

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];

var isDolapArray = Array.isArray(dolap);

console.log("Is dolap an array?", isDolapArray);
```

#### Check whether there is a "Pants" element in the wardrobe array with 3 different methods

- Using indexOf() Method:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var hasPants1 = dolap.indexOf("Pant") !== -1;
console.log("Method 1:", hasPants1);
```

- Using includes() Method:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var hasPants2 = dolap.includes("Pant");
console.log("Method 2:", hasPants2);

```

- Using some() Method:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var hasPants3 = dolap.some(item => item === "Pant");
console.log("Method 3:", hasPants3);
```

#### Write a function that will add the number of characters of the elements in the cabinet array and return them back.

```JavaScript
function calculateTotalCharacters(array) {
  // Check if the input is an array
  if (!Array.isArray(array)) {
    return "Input is not an array.";
  }

  // Calculate total number of characters
  const totalCharacters = array.reduce((total, item) => total + item.length, 0);

  return totalCharacters;
}

// Example usage with the dolap array
var dolap = ["Shirt", "Pant", "TShirt"];
var result = calculateTotalCharacters(dolap);

console.log("Total characters in dolap array:", result);
```

#### Convert all elements in the wardrobe array to uppercase and assign them to a new variable in 3 different ways

- Using map() Method:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var uppercasedArray1 = dolap.map(item => item.toUpperCase());
console.log("Method 1:", uppercasedArray1);
```

- Using for...of Loop:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var uppercasedArray2 = [];
for (let item of dolap) {
  uppercasedArray2.push(item.toUpperCase());
}
console.log("Method 2:", uppercasedArray2);

```

- Using forEach() Method:

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];
var uppercasedArray3 = [];
dolap.forEach(item => uppercasedArray3.push(item.toUpperCase()));
console.log("Method 3:", uppercasedArray3);
```

#### Convert the cabinet array into an object with index numbers as keys.

```JavaScript
var dolap = ["Shirt", "Pant", "TShirt"];

var dolapObject = dolap.reduce((obj, item, index) => {
  obj[index] = item;
  return obj;
}, {});

console.log("Converted dolap object:", dolapObject);
```

#### What is the difference between slice and splice?

slice() Method:

- Purpose: Used to extract a portion of an array and create a new array without modifying the original array.
- Parameters: Takes start and end indices as arguments.

```JavaScript
const arr = [1, 2, 3, 4, 5];
const slicedArr = arr.slice(1, 4);
// Result: slicedArr = [2, 3, 4], arr = [1, 2, 3, 4, 5] (original array unchanged)

```

splice() Method:

- Purpose: Used to remove or replace elements in an array, modifying the original array.
- Parameters: Takes start index, number of elements to remove, and optional elements to add.

```JavaScript
const arr = [1, 2, 3, 4, 5];
const removedItems = arr.splice(1, 3, 6, 7, 8);
// Result: arr = [1, 6, 7, 8, 5], removedItems = [2, 3, 4] (original array modified)
```

###

```JavaScript
const arr = [1,2,3,4,5,6,7,7,8,6,10];
```

#### Find duplicate numbers in array

```JavaScript
const uniqueSet = new Set(arr);
const duplicatesSet = new Set(arr.filter(item => uniqueSet.has(item)));

const duplicateNumbers = Array.from(duplicatesSet);

console.log("Duplicate numbers:", duplicateNumbers);
```

#### Delete all duplicate numbers in the array and create a new array with 2 different methods

```JavaScript
// Use Set to filter duplicates
const uniqueSet = new Set(arr);
const newArray1 = Array.from(uniqueSet);

console.log("New array (Set method):", newArray1);
```

#### Find the highest and lowest value in the array with 2 different methods

- 1st way

```JavaScript
const highestValue1 = Math.max(...arr);
const lowestValue1 = Math.min(...arr);

console.log("Highest value (Math method):", highestValue1);
console.log("Lowest value (Math method):", lowestValue1);
```

- 2nd way

```JavaScript
const { highestValue2, lowestValue2 } = arr.reduce(
  (acc, current) => ({
    highestValue2: Math.max(acc.highestValue2, current),
    lowestValue2: Math.min(acc.lowestValue2, current),
  }),
  { highestValue2: -Infinity, lowestValue2: Infinity }
);

console.log("Highest value (Reduce method):", highestValue2);
console.log("Lowest value (Reduce method):", lowestValue2);
```

###

## Outputs of Codes

### 1st QUESTION

```JavaScript
Error 1
Success 4
```

- The job() function returns a promise that is immediately rejected.
- The catch block is triggered when the promise is rejected, and it logs 'Error 1'.
- The then block after the catch block (console.log('Success 4')) is executed regardless of the rejection because it is not directly connected to the rejected promise. This is a characteristic of promises in JavaScript. It will log 'Success 4'.

The key point here is that then blocks following a catch block are not affected by the rejection; they will be executed regardless of whether there was an error. This behavior is a part of the promise chaining mechanism in JavaScript.

So, even though an error occurred and was caught, the subsequent then block (console.log('Success 4')) is still executed.

### 2nd QUESTION

```JavaScript
success
Defeat
error
Error caught
Success: test
```

"# Odev-1-Furkanlebit7"
