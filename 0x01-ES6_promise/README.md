# ES6 Promises

## Learning Objectives

This project covers the following concepts:

- Understand Promises: What they are, why they are used, and how they function.
- Utilize the `then`, `resolve`, and `catch` methods for handling Promise states and results.
- Employ the `every` method of the Promise object for managing multiple promises.
- Understand error handling with throw/try.
- Utilize the `await` operator for asynchronous programming.
- Implement and use async functions effectively.

## Introduction to Promises

Promises are a core concept in JavaScript for managing asynchronous operations. They represent a value that may be available now, or in the future, or never. Promises provide a clean and efficient way to handle asynchronous code.

## Using `then`, `resolve`, and `catch` Methods

The `then` method is used to handle the result of a Promise. It takes two optional callback functions as arguments: one for success (`resolve`) and one for failure (`reject`). `resolve` is invoked when the Promise is fulfilled, and `reject` is invoked when it is rejected. The `catch` method is used to handle errors in Promises.

## Utilizing the `every` Method

The `every` method of the Promise object is used to handle multiple promises concurrently. It returns a single Promise that resolves when all of the promises in the iterable argument have resolved, or rejects with the reason of the first promise that rejects.

## Error Handling with Throw/Try

The `throw` statement is used to throw an exception. When an exception is thrown, JavaScript will stop and check the surrounding code for a `try` block. If a matching `catch` block is found, the exception is caught, and execution continues after the `catch` block. Otherwise, the program terminates.

## Understanding the `await` Operator

The `await` operator is used to wait for a Promise to resolve or reject. It can only be used within an `async` function. When `await` is used, the execution of the `async` function is paused until the Promise is settled. If the Promise is fulfilled, the `await` expression returns the value. If the Promise is rejected, the `await` expression throws an error.

## Implementing and Using Async Functions

Async functions are functions that operate asynchronously via the event loop, using an `async` keyword before the function declaration. Inside an async function, you can use the `await` operator to wait for a Promise to resolve. Async functions always return a Promise
