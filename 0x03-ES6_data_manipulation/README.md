# 0x03. ES6 Data Manipulation

## Learning Objectives

By the end of this project, you should be able to explain the following concepts without needing to consult external resources:

- How to use `map`, `filter`, and `reduce` on arrays
- Typed arrays
- The `Set`, `Map`, and `WeakMap` data structures

---

## Introduction

ES6 (ECMAScript 2015) introduced a variety of new features and improvements to JavaScript. Among these are powerful methods for manipulating data in arrays, typed arrays for handling binary data more efficiently, and new data structures like `Set`, `Map`, and `WeakMap` for managing collections of data.

This README will guide you through the key concepts and techniques related to ES6 data manipulation.

---

## Table of Contents

1. [Array Manipulation](#array-manipulation)
    - [Using `map`](#using-map)
    - [Using `filter`](#using-filter)
    - [Using `reduce`](#using-reduce)
2. [Typed Arrays](#typed-arrays)
3. [Set, Map, and WeakMap](#set-map-and-weakmap)

---

## Array Manipulation

### Using `map`

The `map` method creates a new array by applying a function to each element in the original array.

\`\`\`javascript
const numbers = [1, 2, 3, 4, 5];
const squaredNumbers = numbers.map(num => num * num);

console.log(squaredNumbers); // [1, 4, 9, 16, 25]
\`\`\`

### Using `filter`

The `filter` method creates a new array containing elements that pass a test specified by a provided function.

\`\`\`javascript
const numbers = [1, 2, 3, 4, 5];
const evenNumbers = numbers.filter(num => num % 2 === 0);

console.log(evenNumbers); // [2, 4]
\`\`\`

### Using `reduce`

The `reduce` method executes a reducer function on each element of the array, resulting in a single output value.

\`\`\`javascript
const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((acc, num) => acc + num, 0);

console.log(sum); // 15
\`\`\`

---

## Typed Arrays

Typed arrays provide a way to work with binary data in JavaScript. They offer a more efficient way to handle data buffers, making them ideal for tasks like WebGL rendering or handling network protocols.

\`\`\`javascript
const buffer = new ArrayBuffer(16);
const intArray = new Int32Array(buffer);

intArray[0] = 42;
console.log(intArray[0]); // 42
\`\`\`

---

## Set, Map, and WeakMap

### Set

A `Set` is a collection of unique values, allowing you to store primitive values and object references.

\`\`\`javascript
const mySet = new Set();

mySet.add(1);
mySet.add(2);
mySet.add(3);

console.log(mySet.has(2)); // true
\`\`\`

### Map

A `Map` is a collection of key-value pairs, allowing you to store and retrieve values based on keys.

\`\`\`javascript
const myMap = new Map();

myMap.set('name', 'John');
myMap.set('age', 30);

console.log(myMap.get('name')); // John
\`\`\`

### WeakMap

A `WeakMap` is similar to a `Map`, but with some differences in behavior. It only allows objects as keys and does not prevent its keys from being garbage collected.

\`\`\`javascript
const weakMap = new WeakMap();
const obj = {};

weakMap.set(obj, 'some value');

console.log(weakMap.get(obj)); // 'some value'
\`\`\`

---

