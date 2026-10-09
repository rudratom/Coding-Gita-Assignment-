# Assignment: JavaScript Operators

## A. Arithmetic Operators

# 1. Addition (`+`)

### Q1. Total school collection

**Calculation:**

```javascript
let classOne = 15000;
let classTwo = 12500;
let total = classOne + classTwo;

console.log(total);
```

**Output:**
```text
27500
```

**Explanation:** I added the collections of both classes to find the total amount.

### Q2. Total pages read

```javascript
let morningPages = 18;
let eveningPages = 25;

console.log(morningPages + eveningPages);
```

**Output:**
```text
43
```

### Q3. Total items sold

```javascript
let monday = 125;
let tuesday = 178;

console.log(monday + tuesday);
```

**Output:**
```text
303
```

### Q4. Predict the output

```javascript
let a = "10";
let b = 5;
let result = a + b;

console.log(result);
```

**Output:**
```text
105
```

**Explanation:** Since `a` is a string, JavaScript joins `"10"` and `5` instead of adding them as numbers.

### Q5. Predict the output

```javascript
let x = 5;
let y = "3";
let result = x + y;

console.log(result);
```

**Output:**
```text
53
```

**Explanation:** The `+` operator joins the number `5` with the string `"3"`.

### Q6. Calculate `15 + 27`

**Answer:** \(15 + 27 = 42\)

### Q7. Total price of a book and a pen

```javascript
let book = 350;
let pen = 45;

console.log(book + pen);
```

**Output:**
```text
395
```

**Answer:** ₹395

### Q8. Find the result of `"25" + 10`

**Output:**
```text
2510
```

**Explanation:** The `+` operator performs string concatenation because one of the values is a string.

### Q9. Find the total spent and remaining balance

```javascript
let wallet = 2000;
let itemOne = 750;
let itemTwo = 320;

let totalSpent = itemOne + itemTwo;
let remaining = wallet - totalSpent;

console.log(totalSpent);
console.log(remaining);
```

**Output:**
```text
1070
930
```

**Answer:** Total spent = ₹1,070; remaining balance = ₹930.

### Q10. Predict and explain the outputs

```javascript
console.log(5 + "5" + 5);
console.log(5 + 5 + "5");
console.log("5" + 5 + 5);
```

**Output:**
```text
555
105
555
```

**Explanation:**

- In the first line, `5 + "5"` becomes `"55"`, then `5` is joined to it.
- In the second line, `5 + 5` becomes `10`, then `"5"` is joined to it.
- In the third line, the first value is a string, so all values are joined as strings.

---

# 2. Subtraction (`-`)

### Q1. Find the empty bus seats

```javascript
let totalSeats = 80;
let occupiedSeats = 53;

console.log(totalSeats - occupiedSeats);
```

**Output:**
```text
27
```

### Q2. Find the final marks

```javascript
let marks = 500;
let lostMarks = 35;

console.log(marks - lostMarks);
```

**Output:**
```text
465
```

### Q3. Find the remaining boxes

```javascript
let boxes = 2500;
let sentBoxes = 875;

console.log(boxes - sentBoxes);
```

**Output:**
```text
1625
```

### Q4. Predict the output

```javascript
let a = "10";
let b = 3;
let result = a - b;

console.log(result);
```

**Output:**
```text
7
```

**Explanation:** JavaScript converts the numeric string `"10"` into a number when using the `-` operator.

### Q5. Predict the output

```javascript
let x = "20";
let y = "5";
let result = x - y;

console.log(result);
```

**Output:**
```text
15
```

**Explanation:** Both strings are converted into numbers before subtraction.

### Q6. Calculate `100 - 37`

**Answer:** \(100 - 37 = 63\)

### Q7. Find the remaining water

```javascript
let water = 500;
let used = 175;

console.log(water - used);
```

**Output:**
```text
325
```

**Answer:** 325 litres

### Q8. Compare `"50" - 20` and `"50" - "20"`

```javascript
console.log("50" - 20);
console.log("50" - "20");
```

**Output:**
```text
30
30
```

**Explanation:** The subtraction operator converts both numeric strings into numbers. Therefore, both expressions return `30`.

### Q9. Find the remaining apples

```javascript
let apples = 240;
let morningSales = 95;
let eveningSales = 67;

let remaining = apples - morningSales - eveningSales;

console.log(remaining);
```

**Output:**
```text
78
```

**Answer:** 78 apples are left.

### Q10. Predict and explain the outputs

```javascript
console.log("100" - 50);
console.log("abc" - 10);
console.log(10 - "5" - "2");
console.log("10" - "5" - "2");
```

**Output:**
```text
50
NaN
3
3
```

**Explanation:**

- `"100" - 50` returns `50` because the string is converted to a number.
- `"abc" - 10` returns `NaN` because `"abc"` cannot be converted into a valid number.
- Both remaining expressions return `3` because subtraction converts numeric strings into numbers and evaluates from left to right.

---

# 3. Multiplication (`*`)

### Q1. Cost of 8 notebooks

```javascript
let notebookPrice = 45;
let quantity = 8;

console.log(notebookPrice * quantity);
```

**Output:**
```text
360
```

**Answer:** ₹360

### Q2. Machine production in 6 hours

```javascript
let bottlesPerHour = 120;
let hours = 6;

console.log(bottlesPerHour * hours);
```

**Output:**
```text
720
```

### Q3. Total plants in the garden

```javascript
let rows = 7;
let plantsPerRow = 15;

console.log(rows * plantsPerRow);
```

**Output:**
```text
105
```

### Q4. Predict the output

```javascript
let a = "5";
let b = 4;
let result = a * b;

console.log(result);
```

**Output:**
```text
20
```

**Explanation:** The multiplication operator converts `"5"` into the number `5`.

### Q5. Predict the output

```javascript
let x = "10";
let y = "2";
let result = x * y;

console.log(result);
```

**Output:**
```text
20
```

### Q6. Calculate `12 * 8`

**Answer:** \(12 \times 8 = 96\)

### Q7. Cost of 4 pizzas

```javascript
let pizzaPrice = 299;
let quantity = 4;

console.log(pizzaPrice * quantity);
```

**Output:**
```text
1196
```

**Answer:** ₹1,196

### Q8. Find the results of `"7" * 6` and `"7" * "6"`

```javascript
console.log("7" * 6);
console.log("7" * "6");
```

**Output:**
```text
42
42
```

**Explanation:** JavaScript converts both numeric strings into numbers before multiplication.

### Q9. Factory production in 8 hours

```javascript
let unitsPerHour = 45;
let hours = 8;

console.log(unitsPerHour * hours);
```

**Output:**
```text
360
```

**Answer:** 360 units

### Q10. Predict and explain the outputs

```javascript
console.log("5" * 3 * "2");
console.log("abc" * 4);
console.log(10 * "2.5");
console.log("10" * "2.5" * "0");
```

**Output:**
```text
30
NaN
25
0
```

**Explanation:**

- `"5" * 3 * "2"` returns `30` after converting the strings into numbers.
- `"abc" * 4` returns `NaN` because `"abc"` is not a valid number.
- `10 * "2.5"` returns `25`.
- `"10" * "2.5" * "0"` returns `0` because the multiplication evaluates from left to right.

---

# 4. Division (`/`)

### Q1. Pencils per student

```javascript
let pencils = 144;
let students = 12;

console.log(pencils / students);
```

**Output:**
```text
12
```

**Answer:** 12 pencils per student

### Q2. Average distance travelled per hour

```javascript
let distance = 360;
let hours = 6;

console.log(distance / hours);
```

**Output:**
```text
60
```

**Answer:** 60 kilometres per hour

### Q3. Money per department

```javascript
let amount = 72000;
let departments = 9;

console.log(amount / departments);
```

**Output:**
```text
8000
```

**Answer:** ₹8,000 per department

### Q4. Predict the output

```javascript
let a = "20";
let b = 4;
let result = a / b;

console.log(result);
```

**Output:**
```text
5
```

**Explanation:** JavaScript converts `"20"` into a number before division.

### Q5. Predict the output

```javascript
let x = "100";
let y = "5";
let result = x / y;

console.log(result);
```

**Output:**
```text
20
```

### Q6. Calculate `144 / 12`

**Answer:** \(144 \div 12 = 12\)

### Q7. Students per classroom

```javascript
let students = 360;
let classrooms = 9;

console.log(students / classrooms);
```

**Output:**
```text
40
```

**Answer:** 40 students per classroom

### Q8. Compare `"100" / 4` and `"100" / "4"`

```javascript
console.log("100" / 4);
console.log("100" / "4");
```

**Output:**
```text
25
25
```

**Explanation:** Both expressions return `25` because JavaScript converts numeric strings into numbers when using division.

### Q9. Calculate each friend's share

```javascript
let bill = 2400;
let friends = 6;

console.log(bill / friends);
```

**Output:**
```text
400
```

**Answer:** Each friend pays ₹400.

### Q10. Predict and explain the outputs

```javascript
console.log(10 / 0);
console.log(-10 / 0);
console.log(0 / 0);
console.log("20" / "4" / 2);
console.log("abc" / 5);
```

**Output:**
```text
Infinity
-Infinity
NaN
2.5
NaN
```

**Explanation:**

- `10 / 0` returns `Infinity`.
- `-10 / 0` returns `-Infinity`.
- `0 / 0` returns `NaN` because the result is undefined mathematically.
- `"20" / "4" / 2` returns `2.5` because division evaluates from left to right.
- `"abc" / 5` returns `NaN` because `"abc"` cannot be converted into a valid number.

**Conclusion:** The arithmetic operators perform calculations on numbers. The `+` operator can also join strings, while `-`, `*`, and `/` generally convert numeric strings into numbers. Invalid numeric conversions result in `NaN`.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Assignment: JavaScript Operators

# A. Arithmetic Operators

## 5. Modulus (`%`)

### Q1. Students left over

```javascript
let students = 53;
let groupSize = 5;

console.log(students % groupSize);
```

**Output:**
```text
3
```

**Explanation:** After forming full groups of 5, 3 students are left over.

### Q2. Candies left unpacked

```javascript
let candies = 128;
let boxSize = 10;

console.log(candies % boxSize);
```

**Output:**
```text
8
```

### Q3. Toys left after packing

```javascript
let toys = 237;
let boxSize = 6;

console.log(toys % boxSize);
```

**Output:**
```text
3
```

### Q4. Passengers left after filling buses

```javascript
let people = 185;
let busCapacity = 40;

console.log(people % busCapacity);
```

**Output:**
```text
25
```

**Explanation:** After filling 4 full buses, 25 people remain.

### Q5. Predict the output

```javascript
let a = 10;
let b = 0;
let result = a % b;

console.log(result);
```

**Output:**
```text
NaN
```

**Explanation:** The remainder cannot be calculated when dividing by zero.

### Q6. Calculate `29 % 5`

**Answer:** `29 % 5 = 4`

### Q7. Chocolates left over

```javascript
let chocolates = 23;
let boxSize = 4;

console.log(chocolates % boxSize);
```

**Output:**
```text
3
```

### Q8. Find the results of `0 % 7` and `15 % 0`

```javascript
console.log(0 % 7);
console.log(15 % 0);
```

**Output:**
```text
0
NaN
```

**Explanation:** Zero divided by 7 leaves a remainder of 0. The remainder operation with a divisor of zero returns `NaN`.

### Q9. Full sheets and remaining pages

```javascript
let pages = 47;
let pagesPerSheet = 6;

console.log(Math.floor(pages / pagesPerSheet));
console.log(pages % pagesPerSheet);
```

**Output:**
```text
7
5
```

**Explanation:** There are 7 full sheets and 5 pages left over.

### Q10. Predict and explain the outputs

```javascript
console.log(17 % 5);
console.log(-17 % 5);
console.log(17 % -5);
console.log(-17 % -5);
console.log(10 % 0);
```

**Output:**
```text
2
-2
2
-2
NaN
```

**Explanation:** In JavaScript, the remainder has the same sign as the dividend (the number on the left). If the divisor is zero, the result is `NaN`.

---

## 6. Exponentiation (`**`)

### Q1. Volume of a cube

```javascript
let side = 6;

console.log(side ** 3);
```

**Output:**
```text
216
```

**Answer:** 216 cm³

### Q2. Total cells in a square arrangement

```javascript
let side = 9;

console.log(side ** 2);
```

**Output:**
```text
81
```

### Q3. Calculate \(5^4\)

```javascript
console.log(5 ** 4);
```

**Output:**
```text
625
```

### Q4. Total pixels in a square image

```javascript
let pixels = 1024;

console.log(pixels ** 2);
```

**Output:**
```text
1048576
```

### Q5. Predict the output

```javascript
let base = 2;
let power = -1;
let result = base ** power;

console.log(result);
```

**Output:**
```text
0.5
```

**Explanation:** A negative exponent gives the reciprocal. Therefore, \(2^{-1} = 1/2\).

### Q6. Calculate `3 ** 4`

**Answer:** `3 ** 4 = 81`

### Q7. Area of a square

```javascript
let side = 9;

console.log(side ** 2);
```

**Output:**
```text
81
```

**Answer:** 81 square units

### Q8. Compare `2 ** 5` and `5 ** 2`

```javascript
console.log(2 ** 5);
console.log(5 ** 2);
```

**Output:**
```text
32
25
```

**Explanation:** They are not the same because the base and exponent are different.

### Q9. Predict and explain the outputs

```javascript
console.log(2 ** 3 ** 2);
console.log((2 ** 3) ** 2);
console.log(2 ** -3);
// console.log(-2 ** 2);
console.log((-2) ** 2);
console.log(4 ** 0.5);
```

**Output:**
```text
512
64
0.125
4
2
```

**Explanation:**

- `2 ** 3 ** 2` returns `512` because exponentiation is right-associative: `2 ** (3 ** 2)`.
- `(2 ** 3) ** 2` returns `64` because the parentheses make the first exponentiation happen first.
- `2 ** -3` returns `0.125`.
- `(-2) ** 2` returns `4` because the negative number is inside parentheses.
- `4 ** 0.5` returns `2`, which is the square root of 4.
- The expression `-2 ** 2` causes a `SyntaxError` in JavaScript unless the negative base is placed inside parentheses.

### Q10. Predict the output

```javascript
let a = 10;
let b = 0;
let result = a ** b;

console.log(result);
```

**Output:**
```text
1
```

**Explanation:** Any non-zero number raised to the power of zero equals 1.

---

# B. Assignment Operators

## 1. Simple Assignment (`=`)

### Q1. Store a student's name and marks

```javascript
let studentName = "Priya";
let marks = 92;

console.log(studentName);
console.log(marks);
```

**Output:**
```text
Priya
92
```

### Q2. Assign zero to score

```javascript
let score = 0;

console.log(score);
```

**Output:**
```text
0
```

### Q3. Assign 50 to three variables

```javascript
let a, b, c;

a = b = c = 50;

console.log(a, b, c);
```

**Output:**
```text
50 50 50
```

### Q4. Predict the output

```javascript
let x;
x = 100;

console.log(x);
```

**Output:**
```text
100
```

**Explanation:** The variable is declared first and assigned a value later.

### Q5. Predict the output

```javascript
let p = 15;
let q = p;
q = 30;

console.log(p, q);
```

**Output:**
```text
15 30
```

**Explanation:** Changing `q` does not change `p` because both variables hold separate number values.

---

## 2. Add and Assign (`+=`)

### Q1. Update the player's score

```javascript
let score = 80;
score += 25;

console.log(score);
```

**Output:**
```text
105
```

### Q2. Update the wallet balance

```javascript
let balance = 1500;
balance += 120;

console.log(balance);
```

**Output:**
```text
1620
```

**Answer:** ₹1,620

### Q3. Predict the output

```javascript
let count = 10;
count += 5;

console.log(count);
```

**Output:**
```text
15
```

### Q4. Predict the output

```javascript
let msg = "Good";
msg += " Morning";

console.log(msg);
```

**Output:**
```text
Good Morning
```

### Q5. Find the final value

```javascript
let n = 20;
n += "5";

console.log(n);
```

**Output:**
```text
205
```

**Explanation:** The `+=` operator joins the number `20` with the string `"5"` to produce `"205"`.

---

## 3. Subtract and Assign (`-=`)

### Q1. Update the player's health

```javascript
let health = 100;
health -= 35;

console.log(health);
```

**Output:**
```text
65
```

### Q2. Update the stock

```javascript
let stock = 300;
stock -= 45;

console.log(stock);
```

**Output:**
```text
255
```

### Q3. Predict the output

```javascript
let lives = 5;
lives -= 2;

console.log(lives);
```

**Output:**
```text
3
```

### Q4. Predict the output

```javascript
let num = "40";
num -= 15;

console.log(num);
```

**Output:**
```text
25
```

**Explanation:** The subtraction assignment operator converts the numeric string into a number.

### Q5. Find the result

```javascript
let x = "abc";
x -= 5;

console.log(x);
```

**Output:**
```text
NaN
```

**Explanation:** `"abc"` cannot be converted into a valid number, so the subtraction returns `NaN`.

---

## 4. Multiply and Assign (`*=`)

### Q1. Apply 18% GST

```javascript
let price = 500;
price *= 1.18;

console.log(price);
```

**Output:**
```text
590
```

**Answer:** ₹590, including GST.

### Q2. Triple the quantity

```javascript
let quantity = 8;
quantity *= 3;

console.log(quantity);
```

**Output:**
```text
24
```

### Q3. Predict the output

```javascript
let amount = 200;
amount *= 1.1;

console.log(amount);
```

**Output:**
```text
220.00000000000003
```

**Explanation:** JavaScript uses floating-point numbers, so some decimal calculations may have a small precision difference.

### Q4. Predict the output

```javascript
let val = "7";
val *= 3;

console.log(val);
```

**Output:**
```text
21
```

### Q5. Find the result

```javascript
let y = "hello";
y *= 2;

console.log(y);
```

**Output:**
```text
NaN
```

**Explanation:** The string `"hello"` cannot be converted into a valid number for multiplication.

---

## 5. Divide and Assign (`/=`)

### Q1. Share chocolates equally

```javascript
let chocolates = 180;
chocolates /= 6;

console.log(chocolates);
```

**Output:**
```text
30
```

**Answer:** Each child receives 30 chocolates.

### Q2. Find the average speed

```javascript
let distance = 300;
distance /= 5;

console.log(distance);
```

**Output:**
```text
60
```

**Answer:** 60 km/h

### Q3. Predict the output

```javascript
let total = 400;
total /= 8;

console.log(total);
```

**Output:**
```text
50
```

### Q4. Predict the output

```javascript
let num = "100";
num /= 4;

console.log(num);
```

**Output:**
```text
25
```

### Q5. Find the result

```javascript
let z = 50;
z /= 0;

console.log(z);
```

**Output:**
```text
Infinity
```

**Explanation:** Dividing a positive, non-zero number by zero produces `Infinity` in JavaScript.

---

**Conclusion:** Arithmetic operators are used to perform calculations, while assignment operators update the value stored in a variable. JavaScript can convert numeric strings into numbers during mathematical operations, but the `+` and `+=` operators may join strings instead.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 6. Modulus and Assign `%=`

### 1. Store the remainder when 47 is divided by 6.

```javascript
let num = 47;
num %= 6;
console.log(num);
```

**Output:**
```text
5
```

**Explanation:** 47 divided by 6 leaves a remainder of 5.

### 2. Keep only the remainder when 23 is divided by 12.

```javascript
let counter = 23;
counter %= 12;
console.log(counter);
```

**Output:**
```text
11
```

### 3. Predict the output.

```javascript
let num = 29;
num %= 5;
console.log(num);
```

**Output:**
```text
4
```

### 4. Predict the output.

```javascript
let x = "17";
x %= 3;
console.log(x);
```

**Output:**
```text
2
```

**Explanation:** JavaScript converts the string `"17"` into the number `17` before performing the calculation.

### 5. What happens when we use `%=` with zero?

```javascript
let m = 15;
m %= 0;
console.log(m);
```

**Output:**
```text
NaN
```

**Explanation:** A number cannot be divided by zero to get a valid remainder, so the result is `NaN` (Not a Number).

---

## 7. Exponentiation and Assign `**=`

### 1. Calculate the volume of a cube with side 5.

```javascript
let side = 5;
side **= 3;
console.log(side);
```

**Output:**
```text
125
```

**Explanation:** The volume of a cube is side × side × side, so \(5^3 = 125\).

### 2. Square the number 4.

```javascript
let num = 4;
num **= 2;
console.log(num);
```

**Output:**
```text
16
```

### 3. Predict the output.

```javascript
let base = 2;
base **= 5;
console.log(base);
```

**Output:**
```text
32
```

### 4. Predict the output.

```javascript
let n = 4;
n **= 0.5;
console.log(n);
```

**Output:**
```text
2
```

**Explanation:** Raising a number to the power of `0.5` gives its square root.

### 5. What happens when the exponent is -1?

```javascript
let p = 2;
p **= -1;
console.log(p);
```

**Output:**
```text
0.5
```

**Explanation:** A negative exponent gives the reciprocal. Therefore, \(2^{-1} = \frac{1}{2}\).

---

# C] Comparison Operators

## 1. Loose Equality `==`

### 1. Check whether `"25"` is loosely equal to `25`.

```javascript
console.log("25" == 25);
```

**Output:**
```text
true
```

**Explanation:** The `==` operator converts the string into a number before comparing.

### 2. Check if `0 == false` returns true or false.

```javascript
console.log(0 == false);
```

**Output:**
```text
true
```

### 3. Predict the output.

```javascript
console.log(10 == "10");
console.log(null == undefined);
```

**Output:**
```text
true
true
```

### 4. Predict the output.

```javascript
console.log("" == 0);
console.log([] == false);
```

**Output:**
```text
true
true
```

**Explanation:** With loose equality, JavaScript converts values in certain cases before comparing them.

### 5. Why does `NaN == NaN` return `false`?

```javascript
console.log(NaN == NaN);
```

**Output:**
```text
false
```

**Explanation:** `NaN` means Not a Number. In JavaScript, `NaN` is not equal to any value, including itself.

---

## 2. Loose Inequality `!=`

### 1. Check whether `"18" != 18` returns true or false.

```javascript
console.log("18" != 18);
```

**Output:**
```text
false
```

**Explanation:** Both values become the number `18`, so they are equal.

### 2. A password is `"1234"`, and the user enters the number `1234`. Will `!=` return true?

```javascript
let password = "1234";
let enteredPassword = 1234;

console.log(password != enteredPassword);
```

**Output:**
```text
false
```

**Explanation:** The `!=` operator converts the values for comparison, so they are treated as equal. In real applications, password handling should use proper validation rather than relying on loose equality.

### 3. Predict the output.

```javascript
console.log(5 != "5");
console.log(0 != false);
```

**Output:**
```text
false
false
```

### 4. Predict the output.

```javascript
console.log(null != undefined);
console.log("" != 0);
```

**Output:**
```text
false
false
```

### 5. What does `NaN != NaN` return?

```javascript
console.log(NaN != NaN);
```

**Output:**
```text
true
```

**Explanation:** Since `NaN` is not equal to itself, the inequality operator returns `true`.

---

## 3. Strict Equality `===`

### 1. Check whether `"25" === 25` returns true or false.

```javascript
console.log("25" === 25);
```

**Output:**
```text
false
```

**Explanation:** The `===` operator checks both value and data type. One value is a string, and the other is a number.

### 2. Check `0 === false` and `null === undefined`.

```javascript
console.log(0 === false);
console.log(null === undefined);
```

**Output:**
```text
false
false
```

**Explanation:** The values have different data types.

### 3. Predict the output.

```javascript
console.log(10 === "10");
console.log(true === 1);
```

**Output:**
```text
false
false
```

### 4. Predict the output.

```javascript
console.log("" === 0);
console.log([] === false);
```

**Output:**
```text
false
false
```

### 5. Why is `===` preferred over `==` in most real-world code?

**Answer:**

The `===` operator checks both the value and the data type without automatically converting values. This makes comparisons more predictable and helps avoid unexpected results. Therefore, `===` is generally preferred over `==` in JavaScript.****
