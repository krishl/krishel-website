---
layout: post
title:      "A Practical Guide to Algorithms with JavaScript"
date:       2019-10-24 19:39:54 -0400
permalink:  practical_algorithms
Author: Krishel Lasam
categories: 
tags: [computer science]
comments: false
---

Over the past four days, I worked through Bianca Gandolfo's [A Practical Guide to Algorithms with JavaScript](https://frontendmasters.com/courses/practical-algorithms/) course on Front End Masters. The course covered algorithms with common interview questions using a handful of algorithm techniques.

## Space & Time Complexity

**Space Complexity**: Based how much memory is used with respect to input size

**Time Complexity**: Based on how many primitive operations are executed 

**Big O**: Notation for worst case scenarios

**O(k^n)**: Exponential

**O(n^2)**: Quadratic

**O(n)**: Linear

**O(log n)**: Logarithmic

**O(1)**: Constant

## Optimization with Caching
**Caching**: A technique to make algorithms more efficient. Saves onto an object or an array.

**Execution context**: When a JavaScript function executes, a new execution context is places onto the call stack.

[Exercise 1 - Unique Sort](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/unique-sort-exercise.js)

**Memoization**: The process of caching the value that a function returns (memorization).

**Breadcrumbs method**: Caching a value that is not the result of a function.

[Exercise 2 - Memoization](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/memoization-exercise.js)

## Recursion
**Recursion**: All recursive functions can be written iteratively. Two common patterns for recursion are *wrapper functions* and *accumulators*.

**Closure**: A function inside of a function that is used to make variables private.

**Callback**: A function that is passed into another function and is called inside that function.

[Exercise 3 - Iterative Loop](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/iterative-loop-exercise.js)

[Exercise 4 - Recursive Factorial & Memoize](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/recursive-factorial-and-memoize-exercise.js)

## Divide & Conquer
**Binary Search**: A search for a value in a sorted array by cutting the search area in half. If an interview question gives a sorted array, think of utilizing binary search.

**Linear Search**: A search for a value in an array that checks each value in order.

[Exercise 5 - Linear Search](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/linear-search-exercise.js)

**When optimizing JavaScript, you are trading time complexity for space complexity.

**Implicit Return**: Returns undefined when reaching the end of a function without an explicit return.

**Selection Sort**: The smallest or largest of the original array is taken in inserted into the sorted spot of the results array.

**Insertion Sort**: Just like sorting a hand of cards, it takes elements from the original array and inserts them into the sorted spot of the results array.

**In interviews, try to go with the simplest solution, but reference the most complicated one.

**Javascript uses string-based sort, so make sure to sort numbers in ascending order using `Array.sort((a, b) => a - b)`

[Exercise 6 - Bubble Sort](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/bubble-sort-exercise.js)

[Exercise 7 - Merge Sort](https://github.com/krishl/javascript/blob/master/a-practical-guide-to-algorithms-wth-javascript/merge-sort-exercise.js)

## Greedy Algorithms
**Greedy Algorithm**: Takes the locally optimal solution without looking at the big picture. Used with the data set is very large. Brute force is more thorough.

**Brute Force**: Calculates all combinations possible.


## Dynamic Algorithms
**Dynamic Programming**: An optimization technique where values are cached to avoid repeated calculations. Used where there are overlapping sub-problems. There are two approaches to dynamic programming - *Top-Down (recursive*), and *Bottom-Up (iterative)*

---

This course took me a total of 11 hours to complete.

Total hours worked on Front End Masters: 23 hours.
