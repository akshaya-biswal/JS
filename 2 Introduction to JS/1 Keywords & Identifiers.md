# Keywords

- Keywords are reserved words that are part of the syntax in the programming language.
- `const` is a keyword that denotes that `a` is a constant.

```js
const a = "hello";
```

# Identifiers

An identifier is a name that is given to entities like variables, functions, class, etc.

```js
//valid
const a = "hello";
const _a = "hello";
const $a = "hello";
```

```js
//invalid
const 1a = 'hello';
```

```js
const y = "hi";
const Y = 5;
console.log(y); // hi
console.log(Y); // 5
```

```js
//invalid
const new = 5; // Error! new is a keyword.
```

# Variables

# Constants

https://www.programiz.com/javascript/variables-constants

https://www.programiz.com/javascript/console

https://www.programiz.com/javascript/data-types

primitive data types are simple and immutable, while non-primitive data types are more complex and mutable.

Primitive Data Types:
Primitive data types are basic, immutable data types that directly operate upon the actual values stored in variables. In JavaScript, there are six primitive data types:

    Number: Represents numeric values (integers and floating-point numbers).
    String: Represents sequences of characters enclosed in single or double quotes.
    Boolean: Represents a logical value, either true or false.
    Undefined: Represents a variable that has been declared but not assigned a value.
    Null: Represents the intentional absence of any object value.
    Symbol (introduced in ECMAScript 6): Represents a unique identifier.

```js
let num = 42; // Number
let str = "Hello"; // String
let bool = true; // Boolean
let undef = undefined; // Undefined
let n = null; // Null
let sym = Symbol("foo"); // Symbol
```

Non-Primitive (Reference) Data Types:
Non-primitive data types are more complex, and they are not directly manipulated with the values they contain. Instead, they store references to the memory locations where the actual data is held. Objects, arrays, and functions are examples of non-primitive data types.

    Object: Represents a collection of key-value pairs and is used for more complex data structures.
    Array: A specialized type of object used for storing ordered lists of values.
    Function: Represents a reusable block of code.

```js
let obj = { key: "value" }; // Object
let arr = [1, 2, 3]; // Array
let func = function () {}; // Function
```

<!-- ------------------------- -->

null is a deliberate absence of a value.
undefined is a default value assigned by JavaScript to variables that have not been given a value.
0 is a numeric value representing the integer zero.

<!-- -------------Special Charachers------------------------- -->

## Semicolon (;):

Used to terminate statements. While JavaScript allows statements to be terminated by a newline character, it's a good practice to use semicolons explicitly.

```js
var x = 5;
console.log(x);
```

## Curly Braces ({ }):

Used to define blocks of code, such as those in functions, loops, and conditional statements.

```js
if (condition) {
  // code block
} else {
  // another block
}
```

## Parentheses (()):

Used for grouping expressions and in function declarations and calls.

```js
function myFunction(parameter) {
  // function body
}

myFunction(argument);
```

## Square Brackets ([]):

Used for creating arrays and accessing elements in an array.

```js
var myArray = [1, 2, 3];
var firstElement = myArray[0];
```

## Comma (,):

Used to separate items in a list, such as elements in an array or parameters in a function.

```js
var fruits = ["apple", "banana", "orange"];
```

## Dot (.):

Used to access properties or methods of an object.

```js
var person = {
  name: "John",
  age: 30,
};

console.log(person.name);
```

## Quotes (' and "):

Used to define string literals. JavaScript allows the use of single or double quotes for strings.

```js
var greeting = "Hello, World!";
```

## Backslash ():

Used as an escape character to include special characters in a string.

```js
var myString = 'This is a "quoted" string.';
```

<!-- ------------------ Operators ---------------------------- -->

## 1. Arithmetic Operators:

```
+ (Addition)
- (Subtraction)
* (Multiplication)
/ (Division)
% (Modulus)
++ (Increment)
-- (Decrement)
```

```js
var x = 10;
var y = 5;
var sum = x + y; // 15
var product = x * y; // 50
```

## 2.Assignment Operators:

```
= (Assignment)
+=, -=, *=, /= (Compound Assignment)
```

```js
var a = 10;
a += 5; // Equivalent to: a = a + 5; (a is now 15)
```

## 3. Relational / Comparison Operators:

```
== (Equality)
=== (Strict Equality)
!= (Inequality)
!== (Strict Inequality)
> (Greater Than)
< (Less Than)
>= (Greater Than or Equal To)
<= (Less Than or Equal To)
```

```js
var num1 = 5;
var num2 = "5";
console.log(num1 == num2); // true (loose equality)
console.log(num1 === num2); // false (strict equality)
```

## 4. Logical Operators:

```
&& (Logical AND)
|| (Logical OR)
! (Logical NOT)
```

```js
var condition1 = true;
var condition2 = false;

console.log(condition1 && condition2); // false (AND)
console.log(condition1 || condition2); // true (OR)
console.log(!condition1); // false (NOT)
```

## 5. Unary Operators:

```js
+ (Unary Plus)
- (Unary Minus)
++ (Increment)
-- (Decrement)
typeof (Typeof)
```

```js
var num = 5;
console.log(-num); // -5 (Unary Minus)
console.log(++num); // 6 (Increment)
console.log(typeof num); // "number" (Typeof)
```

## 6. Conditional (Ternary) Operator:

```
condition ? expression1 : expression2
```

```js
var age = 20;
var isAdult = age >= 18 ? "Yes" : "No";
```

## 7. Bitwise Operators:

In JavaScript, bitwise operators perform operations on the binary representation of numeric values.

#### & (Bitwise AND)

```js
var result = 5 & 3; // Binary: 0101 & 0011 = 0001 (Decimal: 1)
```

#### | (Bitwise OR)

```js
var result = 5 | 3; // Binary: 0101 | 0011 = 0111 (Decimal: 7)
```

#### ^ (Bitwise XOR)

```js
var result = 5 ^ 3; // Binary: 0101 ^ 0011 = 0110 (Decimal: 6)
```

#### ~ (Bitwise NOT)

Note: The result is a signed 32-bit integer, and the leftmost bit represents the sign (0 for positive, 1 for negative).

```js
var result = ~5; // Binary: ~0101 = 1010 (Decimal: -6)
```

#### << (Left Shift)

```js
var result = 5 << 1; // Binary: 0101 << 1 = 1010 (Decimal: 10)
```

#### >> (Right Shift)

```js
var result = 5 >> 1; // Binary: 0101 >> 1 = 0010 (Decimal: 2)
```

#### >>> (Unsigned Right Shift)

Similar to the right shift, but the leftmost bits are filled with zeros.

```js
var result = 5 >>> 1; // Binary: 0101 >>> 1 = 0010 (Decimal: 2)
```

<!-- ---------- Short Circuiting --------------- -->

## Short Circuiting

Short-circuiting in JavaScript refers to the behavior of logical operators (AND `&&` and `OR` ||) where the second operand is not evaluated if the result can be determined by the first operand alone.

```js
var result = false && someFunction();
console.log(result); // false
```

```js
var result = true || someFunction();
console.log(result); // true
```

```js
console.log(10 && 6); // 6
```

```js
console.log(10 || 6); // 10
```

<!-- ---------------- Special Numbers ---------------- -->

## 0

- Represents the integer zero.
- It is a valid number and is considered falsy in a boolean context (e.g., if (0) evaluates to false).

```js
let num = 0;
```

## -0

- JavaScript distinguishes between positive zero (0) and negative zero (-0), although the distinction is rarely significant.
- In most contexts, -0 is treated the same as 0.

```js
let negativeZero = -0;
```

```js
console.log(0 === -0); // true
console.log(Object.is(0, -0)); // false
```

## NaN (Not a Number)

- Represents the result of an operation that cannot produce a meaningful numeric result.
- It is a special value and is considered falsy in a boolean context.
- Any arithmetic operation involving NaN will result in NaN.

```js
let result = 10 / "abc"; // NaN
```

## Infinity

- Represents positive infinity.
- It is a value greater than any other numeric value.

```js
var positiveInfinity = Infinity;
console.log(positiveInfinity); // Infinity
```

## -Infinity

- Represents negative infinity.
- It is a value smaller than any other numeric value.

```js
var negativeInfinity = -Infinity;
console.log(negativeInfinity); // -Infinity
```

```js
console.log(1 / 0); // Infinity
console.log(-1 / 0); // -Infinity
console.log(Infinity + 1); // Infinity
console.log(-Infinity - 1); // -Infinity
```

<!-- ----------------------------------------------------------------- -->

## Equality Operators

#### Loose Equality (==)

- The loose equality operator compares values for equality after performing type coercion
- It attempts to convert operands to the same type before making the comparison.

```js
console.log(5 == "5"); // true, because "5" is coerced to a number
```

#### Strict Equality (===)

- The strict equality operator compares values for equality without performing type coercion.
- Both the value and the type must be the same for the comparison to be true.

```js
console.log(5 === "5"); // false, because the types are different
```

#### Inequality Operators:

Similarly, there are also loose inequality (!=) and strict inequality (!==) operators.

```js
console.log(5 != "5"); // false, because "5" is coerced to a number
console.log(5 !== "5"); // true, because the types are different
```

> Some more examples

```js
console.log(0 == false); // true, because both are coerced to a number 0
console.log("" == false); // true, because the empty string is coerced to a number 0
console.log(null == undefined); // true, because they are loosely equal
```
