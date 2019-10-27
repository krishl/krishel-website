---
layout: post
title:      "Four Semesters of CS"
date:       2019-10-20 12:56:47 -0400
permalink:  four_semesters_of_cs
Author: Krishel Lasam
categories: 
tags: [javascript, computer science]
comments: false
---

Touching up on fundamentals once again. I spent the past week going through Brian Holt's [Four Semesters of Computer Science in 5 Hours](https://frontendmasters.com/courses/computer-science/), which goes through algorithms, Big O analysis, recursion, sorting, data structures and functional programming.

## Big O & Recursion

**Recursion**: A function that calls itself. Less efficient than iterative functions.

[Exercise 1 - Recursion](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-1-recursion-solution.js)

## Sorting Algorithms
**Bubble Sort**: Loops through an array comparing adjacent values/indices until the entire array is sorted. Involves 2 loops -- an outer do-while loop and an inner for loop. O(n^2), very inefficient. [5,7,6,4] -> [5,6,7,4] -> [5,6,4,7] -> [5,4,6,7] -> [4,5,6,7]

[Exercise 2 - Bubble Sort](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-2-bubble-sort-solution.js)

**Insertion Sort**: Good for partially sorted arrays. Takes items from the unsorted portion of the list and places them into their sorted position. [10,5,3,8] -> [5,10,3,8] -> [3,5,10,8] -> [3,5,8,10]

[Exercise 3 - Insertion Sort](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-3-insertion-sort-solution.js)

**Merge Sort**: Uses divide-and-conquer recursion, which throws O(log n) into the mix. Most widely used sort since it is a stable sort. Easy to predict what the result will be. The basic gist of merge sort is that a big list will be recursively divided into halves until you have lists of one. This part has O(log n) time complexity. Next, the lists of 1 are merged simultaneously by inserting the smaller value first into the final sorted list. This part of the algorithm would have O(n) time complexity, resulting in a final time complexity of O(n log n). Sorting algorithms require us to look at everything at least once to find out their values. The space complexity is O(n) since arrays are created and destroyed as we go.

[Exercise 4 - Merge Sort](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-4-merge-sort-solution.js)

**Stable Sort**: In a stable sort, equivalent elements will keep their original order in the array.

**Array.concat()**: Used to join 2 or more arrays, returning a new array. `array.concat(array2, array3, ..., arrayX)`

**Array.splice() vs Array.slice()**: `splice()`changes the original array, while `slice()` does not. `splice()` returns the removed items, while `slice()` returns the selected elements. `splice()`can take additional arguments.

**Quick Sort**: Recursive, O(n log n). Takes up less memory than merge sort. It would do poorly if you passed it a sorted list, which causes a worst case time complexity of O(n^2), with the largest number selected as the pivot. [5,7,4,9,6] -> [5,4] [7,9] -> [ ][5] [7][ ] -> [4,5] [7,9] -> [4,5,6,7,9]

[Exercise 5 - Quick Sort](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-5-quick-sort-solution.js)

**Quick Sort 3**: This is where 3 pivots are used -- the first element, the middle element, and the last element. The middle *value* between the three elements is used to mitigate the risk of using Quick Sort on a sorted list.

## Data Structure Interfaces
**Set**: Also known as collections. Sets are objects that do not contain duplicates. Useful for deduplication. Sets have `add()`, `remove()`, `contains()`, `toList()` functionalities. Sets have no sense of order.

**Map**: Also known as dictionaries. Contains key-value pairs. Has no concept of order.

**Weak Maps & Weak Sets**: Allows for garbage collection if all references to the key are lost and there are no references to the value.

**Stack**: Last In, First Out. Stacks are where `push()` and `pop()` come from. Arrays have stack interfaces, but aren't stacks since they can do more than `push()` and `pop()`. `peek()` returns what is on the top without removing it.

**Queue**: First In, Last Out. Works like a line of people and print queues. Has `enqueue()` for add/push functionality, `dequeue()` for remove/pop, and `peek()` which returns the next element to be dequeued.

**Priority Queue**: Used in networking for more important packets that need to be pushed to the front of the queue (i.e. streaming video)

## Implementing Data Structures
**Array List**: Treated just like an array, except that the list shifts/collapses down to the spot the element was deleted from when deleting items from an Array List. Great for get operations because the target element can be directly accessed from memory. Inefficient for delete operations.

[Exercise 6 - Array List](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-6-array-list-solution.js)

**delete**: A keyword in JavaScript that removes a property from an object.

**Linked List**: Has two base properties - `value` and `next`. The first element in a linked list is called the head. The last element is called the tail. While get operations are slow, delete operations are fast. Its base functions are `push()`, `pop()`, `get()`, `delete()`, and `.length`.

[Exercise 7 - Linked List](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-7-linked-list-solution.js)

**Binary Search Tree**: Has O(log n) lookups and deletes. Its worst case is O(n), while dealing with sorted lists. When dealing with duplicates, duplicates either always go to the left or always to to the right node. The basic Binary Search Tree is rarely used in production. Self-balancing trees are used instead so that the worst case from using a binary search tree will not occur. One practical use of  binary search trees is for autocomplete.

[Exercise 8 - Binary Search Tree](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-8-binary-search-tree-solution.js)

**AVL Tree**: A type of binary search tree that keeps the tree in balance. The worst case is O(log n). It does a rotation when the tree is out of balance. It is considered out of balance when the heights of both children differ by 2 or more.

**Leaf Node**: Nodes that do not have children.

**Single Rotation AVL**: Keeps the tree balanced to maintain faster lookups. Left rotations mirror the steps of right rotations. Right rotations are performed when the right cild is heavy, and vice-versa. A single rotation is performed if the unbalanced tree roots are straight.

**Double Rotation AVL**: Double rotations are performed when the unbalanced tree roots are bent, i.e. when the left child of the right child is heavy. In this example case, we would do a left rotation on the right child before doing a right rotation on the root node.

[Exercise 9 - AVL Tree](https://github.com/krishl/javascript/blob/master/four-semesters-of-computer-science-in-5-hours/exercise-9-avl-tree-solution.js)

**Hash Table**: Hash tables are key-value stores.  Keys are run through a hashing algorithm to find where the element is in memory. It does very fast lookups and has no concept of order. Caches and databases use hash tables. Hash tables need a large memory footprint to store objects without collisions. Hashing algorithms are required to be idempotent and performant to maintain fast lookup operations and fast write operations.

**Idempotent**: A function that always gives the same output, given the same input.

**Caesar Cipher**: A hashing algorithm that retrieves a value associated with each letter and multiplies each with its index. Modulo is used afterwards to keep the resulting index inside the range of the hash table.

## Functional Programming 101
**map()**: Applies a function to each individual element to an array and returns the transformed array. Map is chainable.

**reduce()**: Takes a list and transforms it down to one number/string.

**filter()**: Creates a new array containing all elements that returned true from the provided function.

---

This course took me a total of 12 hours to complete.

Total hours worked on Front End Masters: 12 hours.
