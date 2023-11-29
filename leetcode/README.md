# LeetCode: Solutions

## Problem 1: Two Sum
### Instructions
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

### Solution
```js
function twoSumSolution(arr,target) {
   //  Fist sort the array
    const sorted = arr.sort((a,b) => a-b)
   var result = [];
   for (i = 0; i< sorted.length; i++) {
       result.push(sorted[i]);
   }
   return result;
}
```

## Problem 2: Adding Two Numbers
### Instructions
You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order, and each of their nodes contains a single digit. Add the two numbers and return the sum as a linked list.

You may assume the two numbers do not contain any leading zero, except the number 0 itself.

### Solution
```js
function mul (x,y) {
  return function (t) { // anonymous function
    return function (z) { // anonymous function
      return x * t * z;
    };
  };
}
```
