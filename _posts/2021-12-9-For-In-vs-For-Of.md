---
layout: post
title: For...In vs For...Of
---

This is a short post to explain the difference between the For...In loop and the For...Of loop in JavaScript. Both are iterating methods, but there's are a couple of key differences.

##### For...In is for iterating objects, For...Of is for iterating arrays and strings


### For...In

The `for...in` statement is useful for iterating through objects (specifically, objects with *enumerable* properties). A regular `for` loop can't iterate through an object, but a `for...in` loop can. Here's an example of iterating through both keys and properties.

    const obj = {
      1: "apple",
      2: "orange",
      3: "banana"
    }

    for (const key in obj) {
        console.log(key);
    }
    // output:
    // 1
    // 2
    // 3

    for (const property in obj) {
        console.log(obj[property])
    }
    // output:
    // apple
    // banana
    // orange

Other ways to get information from objects include the `Object.entries()` method, which returns a nested array of an object's key:value pairs, and the `Object.keys()` method, which returns an array of property keys.

    console.log(Object.entries(obj))
    // --> [ [ '1', 'apple' ], [ '2', 'orange' ], [ '3', 'banana' ] ]

    console.log(Object.keys(obj))
    // --> [ '1', '2', '3' ]

### For...Of

The `for...of` loop is a slightly shorter way of iterating through iterable objects like arrays or a strings. It does not mutate the original array.

    let arr = [10, 20, 30];
    for (let value of arr) {
      value += 1;
      console.log(value)
    }
    console.log(arr);

    // output:
    // 11
    // 21
    // 31
    // [ 10, 20, 30 ]

Other useful array methods to remember are 
- `.foreach()` which executes a callback function on each element
- `.map()` which returns a new array of return values after executing a callback on each element
- `.filter()` which returns a new array of elements in the original array that return true from a boolean condition
- `.reduce()` which executes a callback function on each element, and passes each subsequent return value into the callback execution on the next element, eventually returning a single value.

Regular for loops are handy and reliable, but they can get cumbersome when trying to iterate through objects, very large arrays, or more complex data structures than simple arrays.