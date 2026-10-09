# JavaScript Assignment: Variables and Scope

## Q5. Choose the Correct Keyword

**Program:**

```javascript
const studentName = "Rudra";
let marks = 85;
const schoolName = "ABC School";

marks = 92;

console.log(studentName);
console.log(marks);
console.log(schoolName);
```

**Output:**

```text
Rudra
92
ABC School
```

**Explanation:**

- `const` is used for `studentName` and `schoolName` because their values should not be reassigned.
- `let` is used for `marks` because its value may change.
- The value of `marks` is changed from `85` to `92`.

---

## Q6. Understand Scope

**Program:**

```javascript
if (true) {
    var a = 10;
    let b = 20;
    const c = 30;
}

console.log(a);
console.log(b);
console.log(c);
```

**Output:**

```text
10
ReferenceError: b is not defined
```

**Explanation:**

- `var` is function-scoped or globally scoped, depending on where it is declared. Therefore, `a` can be accessed outside the `if` block.
- `let` and `const` are block-scoped, so `b` and `c` cannot be accessed outside the block.
- The program stops when it encounters the error for `b`. Therefore, `c` is not printed either.

**Conclusion:** Only the `var` variable can be accessed outside the `if` block.

---

## Q7. Test Re-declaration

**Program using `var`:**

```javascript
var user = "Rudra";
var user = "Rahul";

console.log(user);
```

**Output:**

```text
Rahul
```

**Program using `let`:**

```javascript
let user = "Rudra";
let user = "Rahul";

console.log(user);
```

**Output:**

```text
SyntaxError: Identifier 'user' has already been declared
```

**Explanation:**

- `var` allows a variable to be declared again in the same scope.
- `let` does not allow a variable to be declared again in the same scope.
- To change the value of a `let` variable, use reassignment instead of redeclaration.

**Conclusion:** `var` allows re-declaration, whereas `let` does not allow re-declaration in the same scope.

---

## Q8. Test Re-assignment

**Program:**

```javascript
var a = 10;
let b = 20;
const c = 30;

a = 15;
b = 25;
c = 35;

console.log(a);
console.log(b);
console.log(c);
```

**Output:**

```text
TypeError: Assignment to constant variable.
```

**Explanation:**

- `var` allows reassignment, so `a` changes from `10` to `15`.
- `let` allows reassignment, so `b` changes from `20` to `25`.
- `const` does not allow reassignment, so changing `c` produces a `TypeError`.
- The program stops at the error, so the `console.log()` statements are not executed.

**Conclusion:** Both `var` and `let` allow reassignment, but `const` does not.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Part B – JavaScript Variables

## Q5. Choose the Correct Keyword

**Code:**

```javascript
const studentName = "Rudra";
let marks = 85;
const schoolName = "ABC School";

marks = 92;

console.log(studentName);
console.log(marks);
console.log(schoolName);
```

**Output:**

```text
Rudra
92
ABC School
```

**Explanation:**

I used `const` for `studentName` and `schoolName` because their values will not change. I used `let` for `marks` because marks can change. Here, I changed the marks from 85 to 92 and printed all three variables.

---

## Q6. Understand Scope

**Code:**

```javascript
if (true) {
    var a = 10;
    let b = 20;
    const c = 30;
}

console.log(a);
console.log(b);
console.log(c);
```

**Output:**

```text
10
ReferenceError: b is not defined
```

**Explanation:**

I declared all three variables inside an `if` block. The `var` variable can be accessed outside the block, but `let` and `const` cannot be accessed outside it. This happens because `let` and `const` have block scope.

The program stops when it reaches the error for `b`, so `c` is not printed.

**Conclusion:** Only the `var` variable can be accessed outside the `if` block.

---

## Q7. Test Re-declaration

**Code using `var`:**

```javascript
var user = "Rudra";
var user = "Rahul";

console.log(user);
```

**Output:**

```text
Rahul
```

**Code using `let`:**

```javascript
let user = "Rudra";
let user = "Rahul";

console.log(user);
```

**Output:**

```text
SyntaxError: Identifier 'user' has already been declared
```

**Explanation:**

When I declared `user` again using `var`, the program worked and printed `Rahul`. But when I tried the same thing using `let`, it showed an error because `let` does not allow the same variable to be declared twice in the same scope.

**Conclusion:** `var` allows re-declaration in the same scope, but `let` does not.

---

## Q8. Test Re-assignment

**Code:**

```javascript
var a = 10;
let b = 20;
const c = 30;

a = 15;
b = 25;
c = 35;

console.log(a);
console.log(b);
console.log(c);
```

**Output:**

```text
TypeError: Assignment to constant variable.
```

**Explanation:**

I created three variables using `var`, `let`, and `const`. I was able to change the values of `a` and `b`, but changing the value of `c` caused an error because it was declared using `const`.

The program stopped at the error, so none of the `console.log()` statements were executed.

**Conclusion:** `var` and `let` allow re-assignment, but `const` does not.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# JavaScript Assignment – Part C and Part D

## Q9. Predict and Explain

**Code:**

```javascript
var x = 10;

if (true) {
    var x = 20;
    let y = 30;
    const z = 40;
}

console.log(x);
console.log(y);
console.log(z);
```

**Predicted Output:**

```text
20
ReferenceError: y is not defined
```

**Explanation:**

The first `console.log(x)` prints `20` because `var` is not block-scoped. The variable `x` inside the `if` block changes the same variable.

The second line causes an error because `y` was declared using `let` inside the block. The third line would also cause an error because `z` was declared using `const` inside the block.

The program stops at the first error, so the third line is not executed.

**Conclusion:** `var` can be accessed outside the block, but `let` and `const` cannot.

---

## Q10. Fix the Program

**Original Problems:**

- `const name` has no initial value.
- `age` is declared twice using `let` in the same scope.
- `country` is accessed outside its block.
- `score` is reassigned even though it uses `const`.

**Corrected Code:**

```javascript
const name = "Rudra";

let age = 20;
age = 25;

if (true) {
    var city = "Delhi";
    let country = "India";
    console.log(country);
}

console.log(name);
console.log(age);
console.log(city);

const score = 50;
console.log(score);
```

**Output:**

```text
India
Rudra
25
Delhi
50
```

**Explanation:**

I assigned a value to `name` when declaring it because `const` needs an initial value. I changed the value of `age` instead of declaring it again. I printed `country` inside the `if` block because it cannot be accessed outside that block. I also removed the reassignment of `score` because its value cannot be changed when using `const`.

**Conclusion:** The program now follows the rules of initialization, re-declaration, re-assignment, and scope.

---

## Q11. Predict the Hoisting Behavior

**Code:**

```javascript
console.log(a);
console.log(b);
console.log(c);

var a = 10;
let b = 20;
const c = 30;
```

**Predicted Output:**

```text
undefined
ReferenceError: Cannot access 'b' before initialization
```

**Explanation:**

The `var` variable is hoisted and initialized with `undefined`, so the first line prints `undefined`.

The `let` and `const` variables are also hoisted, but they cannot be accessed before their declarations are initialized. Therefore, the second line causes a `ReferenceError`. The third line would also cause a `ReferenceError`, but it is not executed because the program stops at the second line.

**Conclusion:** `var` can be accessed before its declaration and returns `undefined`, while `let` and `const` cannot be accessed before initialization.

---

## Q12. Fix the Hoisting Errors

**Original Code:**

```javascript
console.log(x);
console.log(y);
console.log(z);

var x = "Hello";
let y = "World";
const z = "!";

console.log(x + " " + y + z);
```

**Corrected Code:**

```javascript
var x = "Hello";
let y = "World";
const z = "!";

console.log(x);
console.log(y);
console.log(z);

console.log(x + " " + y + z);
```

**Output:**

```text
Hello
World
!
Hello World!
```

**Explanation:**

I moved all three variable declarations above the `console.log()` statements. This makes sure that each variable is initialized before it is used. The program now runs without any errors.

**Conclusion:** It is better to declare and initialize variables before using them, especially when working with `let` and `const`.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# JavaScript Assignment – Primitive and Non-Primitive Data Types

# Part E – Basic Identification

## Q1. Classify the Types

**Code:**

```javascript
let wholeNumber = 10;
let decimalNumber = 12.5;
let text = "Hello World";
let isPassed = true;

console.log(wholeNumber, typeof wholeNumber);
console.log(decimalNumber, typeof decimalNumber);
console.log(text, typeof text);
console.log(isPassed, typeof isPassed);
```

**Output:**

```text
10 number
12.5 number
Hello World string
true boolean
```

**Explanation:**

I created four variables with different values. JavaScript uses the `number` type for both whole and decimal numbers. Text is stored as a `string`, and true or false values are stored as `boolean`.

---

## Q2. Undefined vs Null

**Code:**

```javascript
let a;
let b = null;

console.log(a, typeof a);
console.log(b, typeof b);
```

**Output:**

```text
undefined undefined
null object
```

**Explanation:**

The variable `a` has no value assigned to it, so its value is `undefined`. The variable `b` is intentionally assigned `null`, which means an empty or missing value.

JavaScript shows `typeof null` as `object`. This is a known behavior of JavaScript.

---

## Q3. Number Special Values

**Code:**

```javascript
let positiveInfinity = Infinity;
let negativeInfinity = -Infinity;
let notANumber = NaN;
let scientificNumber = 2.5e3;
let largeNumber = 1_000_000;

console.log(positiveInfinity, typeof positiveInfinity);
console.log(negativeInfinity, typeof negativeInfinity);
console.log(notANumber, typeof notANumber);
console.log(scientificNumber, typeof scientificNumber);
console.log(largeNumber, typeof largeNumber);
```

**Output:**

```text
Infinity number
-Infinity number
NaN number
2500 number
1000000 number
```

**Explanation:**

All these values have the `number` type in JavaScript. `Infinity` represents infinity, while `NaN` means Not-a-Number. Scientific notation is used to write numbers in a shorter form. Underscores make large numbers easier to read and do not change their value.

---

## Q4. String Styles

**Code:**

```javascript
let singleQuote = 'Hello';
let doubleQuote = "World";
let name = "Riya";
let templateString = `My name is ${name}`;

console.log(singleQuote);
console.log(doubleQuote);
console.log(templateString);
```

**Output:**

```text
Hello
World
My name is Riya
```

**Explanation:**

JavaScript allows strings to be written using single quotes, double quotes, or backticks. Template literals use backticks and allow variables to be included inside a string using `${}`.

---

# Part F – Advanced Primitive Types

## Q5. Symbol Uniqueness

**Code:**

```javascript
let symbol1 = Symbol("id");
let symbol2 = Symbol("id");

console.log(symbol1 === symbol2);

let student = {
    [symbol1]: "Riya",
    [symbol2]: "Rahul"
};

console.log(student[symbol1]);
console.log(student[symbol2]);
```

**Output:**

```text
false
Riya
Rahul
```

**Explanation:**

Both Symbols have the same description, but they are different values. Every call to `Symbol()` creates a unique Symbol. That is why the comparison returns `false`. Both Symbols can also be used as separate object keys.

---

## Q6. BigInt Precision

**Code:**

```javascript
let num = 9007199254740991;

console.log(num + 1);
console.log(num + 2);
console.log(num + 3);

let bigNum = 9007199254740991n;

console.log(bigNum + 1n);
console.log(bigNum + 2n);
console.log(bigNum + 3n);
```

**Output:**

```text
9007199254740992
9007199254740992
9007199254740994
9007199254740992n
9007199254740993n
9007199254740994n
```

**Explanation:**

JavaScript Numbers can represent integers exactly only up to `9007199254740991`. Beyond this limit, some integers cannot be represented exactly, so the result of adding `2` to the regular Number is rounded.

`BigInt` can store much larger integers with exact precision. I used `n` at the end of the BigInt value and its additions.

---

## Q7. Choose the Correct Type

**Answers:**

1. **Symbol:** Used for a unique identifier.

   ```javascript
   let id = Symbol("id");
   ```

2. **BigInt:** Used for very large integers that need exact precision.

   ```javascript
   let largeNumber = 12345678901234567890n;
   ```

3. **Undefined:** Represents a variable that has been declared but not assigned a value.

   ```javascript
   let value;
   ```

4. **Null:** Represents an intentional empty value.

   ```javascript
   let data = null;
   ```

**Explanation:**

Each type has a different purpose. `Symbol` creates unique values, `BigInt` handles large integers, `undefined` represents an unassigned variable, and `null` is used when I intentionally want to represent no value.

---

# Part G – Prediction and Fixing

## Q8. Predict the Output

**Code:**

```javascript
let a;
let b = null;
let c = 42;
let d = "Hello";
let e = true;
let f = Symbol("key");
let g = 123n;

console.log(typeof a, a);
console.log(typeof b, b);
console.log(typeof c, c);
console.log(typeof d, d);
console.log(typeof e, e);
console.log(typeof f, f);
console.log(typeof g, g);
```

**Output:**

```text
undefined undefined
object null
number 42
string Hello
boolean true
symbol Symbol(key)
bigint 123n
```

**Explanation:**

The `typeof` operator returns the type of each value. The type of `a` is `undefined` because no value was assigned. The surprising result is `typeof null`, which returns `object` instead of `null`. The remaining values return their respective types.

---

## Q9. Fix the Code

**Corrected Code:**

```javascript
let num = 10;
let text = "Hello";
let flag = true;
let empty;
let nothing = null;
let unique = Symbol("id");
let big = 9007199254740991n;

console.log(num, text, flag, empty, nothing, unique, big);
```

**Output:**

```text
10 Hello true undefined null Symbol(id) 9007199254740991n
```

**Explanation:**

I fixed the mistakes by putting quotes around the string, using lowercase `true`, assigning `null` correctly, and using `Symbol()` with a capital S. I also added `n` to the large integer to make it a BigInt. The variable `empty` remains `undefined` because no value was assigned to it.

---

## Q10. Primitive vs Non-Primitive

### a) What is the main difference between Primitive and Non-Primitive data types?

Primitive data types store individual values, such as numbers, strings, and booleans. Non-primitive data types can store collections of values or more complex data.

**Example:**

```javascript
let age = 18;
let student = { name: "Riya", age: 18 };
```

Here, `age` is a primitive value, while `student` is an object.

### b) Why are Numbers, Strings, Booleans, Undefined, Null, Symbol, and BigInt called Primitive?

They are called primitive types because they represent basic values in JavaScript rather than objects. These types are built into the language and are used to store simple values.

**Example:**

```javascript
let age = 18;
let name = "Riya";
let isStudent = true;
```

### c) Give one example of a Non-Primitive data type and explain why it is considered Non-Primitive.

An object is a non-primitive data type because it can store multiple related values as properties.

**Example:**

```javascript
let student = {
    name: "Riya",
    age: 18,
    isEnrolled: true
};

console.log(student);
```

The object stores multiple values together under one variable.

---

# Part H – Non-Primitive Data Types: Basic Creation and Usage

## Q1. Create an Object

**Code:**

```javascript
let student = {
    name: "Riya",
    age: 18,
    isEnrolled: true
};

console.log(student);
console.log(student.name);
console.log(student.age);
console.log(student.isEnrolled);
```

**Output:**

```text
{ name: 'Riya', age: 18, isEnrolled: true }
Riya
18
true
```

**Explanation:**

I created an object named `student` with three properties. Each property stores a different value. I used dot notation to print each property separately.

---

## Q2. Work with Arrays

**Code:**

```javascript
let scores = [85, 92, 78, 90];

let mixedData = [10, "Hello", true, null];

console.log(scores);
console.log(mixedData);
console.log(scores[0]);
console.log(scores[scores.length - 1]);
```

**Output:**

```text
[85, 92, 78, 90]
[10, 'Hello', true, null]
85
90
```

**Explanation:**

I created two arrays. The `scores` array contains only numbers, while `mixedData` contains different types of values. Array indexing starts from `0`, so `scores[0]` gives the first element. I used `scores.length - 1` to access the last element.

---

## Q3. Declare and Call a Function

**Code:**

```javascript
function calculateArea(length, width) {
    return length * width;
}

console.log(calculateArea(5, 4));
console.log(calculateArea(8, 3));
```

**Output:**

```text
20
24
```

**Explanation:**

I created a function named `calculateArea` that takes two parameters, `length` and `width`. It multiplies them and returns the area of the rectangle. I called the function twice with different values.

---

## Q4. Check Types with `typeof`

**Code:**

```javascript
let num = 25;
let text = "Hello";
let flag = true;
let empty = null;
let student = { name: "Riya" };
let numbers = [10, 20, 30];

function greet() {
    return "Hello";
}

console.log(num, typeof num);
console.log(text, typeof text);
console.log(flag, typeof flag);
console.log(empty, typeof empty);
console.log(student, typeof student);
console.log(numbers, typeof numbers);
console.log(greet, typeof greet);
```

**Output:**

```text
25 number
Hello string
true boolean
null object
{ name: 'Riya' } object
[10, 20, 30] object
[Function: greet] function
```

**Explanation:**

I created variables of different types and checked them using `typeof`. Numbers, strings, and booleans return their expected types. The result for `null` is `object`, which is a special behavior in JavaScript. Arrays also return `object` because they are a type of object in JavaScript. A function returns `function`.

**Conclusion:** The `typeof` operator is useful for checking data types, but `null` and arrays have results that may be surprising.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# JavaScript Assignment – Part I and Part J

# Part I – Naming Rules and Best Practices

## Q5. Valid vs Invalid Variable Names

**Answers:**

| Variable Name | Valid/Invalid | Reason |
|---|---|---|
| `userName` | Valid | It starts with a letter. |
| `2ndPlace` | Invalid | A variable name cannot start with a number. |
| `_privateData` | Valid | An underscore can be used at the beginning. |
| `$price` | Valid | A dollar sign is allowed in variable names. |
| `my-age` | Invalid | A hyphen is not allowed in a variable name. |
| `function` | Invalid | `function` is a reserved keyword. |
| `totalCount` | Valid | It follows the naming rules. |
| `const` | Invalid | `const` is a reserved keyword. |

**Explanation:**

JavaScript variable names can contain letters, numbers, underscores, and dollar signs. However, they cannot start with a number or contain spaces and hyphens. Reserved keywords like `function` and `const` cannot be used as variable names.

---

## Q6. Apply Best Practices

**Original Code:**

```javascript
let x = 10;
let y = 5;
let a = x * y;
let b = 100;
```

**Improved Code:**

```javascript
const length = 10;
const width = 5;
const area = length * width;
const MAX_VALUE = 100;

console.log(area);
console.log(MAX_VALUE);
```

**Output:**

```text
50
100
```

**Explanation:**

I replaced the short variable names with meaningful names so the code is easier to understand. I used `const` because these values are not reassigned. I also used uppercase letters for `MAX_VALUE` to show that it represents a constant value.

---

## Q7. Declaration and Assignment

**Code:**

```javascript
let age;
age = 18;

let studentName = "Riya";

const schoolName = "ABC School";

console.log(age);
console.log(studentName);
console.log(schoolName);
```

**Output:**

```text
18
Riya
ABC School
```

**Explanation:**

I declared `age` without assigning a value and assigned `18` later. I declared and assigned `studentName` in one step. I used `const` for `schoolName` because its value should not be reassigned.

---

# Part J – Prediction and Fixing

## Q8. Predict the Output

**Code:**

```javascript
let person = { name: "Amit", age: 22 };
let colors = ["red", "green", "blue"];

function sayHi() {
    return "Hi!";
}

let empty = null;

console.log(typeof person);
console.log(typeof colors);
console.log(typeof sayHi);
console.log(typeof empty);
console.log(person.name);
console.log(colors[1]);
console.log(sayHi());
```

**Output:**

```text
object
object
function
object
Amit
green
Hi!
```

**Explanation:**

- `typeof person` returns `object` because `person` is an object.
- `typeof colors` also returns `object` because arrays are a type of object in JavaScript.
- `typeof sayHi` returns `function` because it is a function.
- `typeof empty` returns `object` because of a special behavior in JavaScript.
- `person.name` prints `Amit` because it accesses the `name` property.
- `colors[1]` prints `green` because array indexing starts from `0`.
- `sayHi()` calls the function and prints the value it returns.

---

## Q9. Fix the Program

**Corrected Code:**

```javascript
let student = { name: "Neha", age: 19 };

let scores = [90, 85, 88];

function greet(name) {
    return "Hello " + name;
}

const MAX_SCORE = 100;

console.log(student.name);
console.log(scores[0]);
console.log(greet("Neha"));
console.log(MAX_SCORE);
```

**Output:**

```text
Neha
90
Hello Neha
100
```

**Explanation:**

I fixed the variable name by removing the number from the beginning. I used lowercase `age` to follow camelCase naming conventions. I placed the scores inside an array and added parentheses to the function declaration. I also added the missing semicolons and removed the reassignment of the constant because a `const` variable cannot be reassigned.

---

## Q10. Concept Questions

### a) What is the main difference between an Object and an Array?

An object stores data using named properties, while an array stores values in an ordered list using indexes.

**Example:**

```javascript
let student = {
    name: "Amit",
    age: 22
};

let colors = ["red", "green", "blue"];

console.log(student.name);
console.log(colors[0]);
```

**Output:**

```text
Amit
red
```

### b) Why does `typeof null` return `"object"`? Is `null` really an object?

JavaScript returns `"object"` for `typeof null` because of an old behavior in the language. However, `null` is a primitive value, not an actual object.

**Example:**

```javascript
let data = null;

console.log(typeof data);
console.log(data === null);
```

**Output:**

```text
object
true
```

### c) Why is it recommended to keep arrays with a single data type?

It is recommended because arrays with the same type of data are easier to read, understand, and work with. It also helps avoid confusion when performing operations on array elements.

**Example:**

```javascript
let marks = [85, 90, 78, 92];

console.log(marks[0]);
```

**Output:**

```text
85
```

### d) When should you use `const` and when should you use `let`?

I use `const` when I do not want to reassign a variable. I use `let` when I need to change its value later.

**Example:**

```javascript
const schoolName = "ABC School";

let marks = 80;
marks = 90;

console.log(schoolName);
console.log(marks);
```

**Output:**

```text
ABC School
90
```

**Conclusion:** I prefer `const` by default and use `let` whenever a variable needs reassignment.
