# Hacker Rank: Solutions

## Problem 1
### Instructions
Given an array of integers, find the sum of its elements.

For example, if the array `ar = [1,2,3]`,`1+2+3=6` so return `6`.

**Function Description**

Complete the `simpleArraySum` function in the editor below. It must return the sum of the array elements as an integer.

simpleArraySum has the following parameter(s):


### Solution
```js
function simpleArraySum(ar) {
// Write your code here
const callbackFn = (acc,cur) => {
return acc + cur
}
return ar.reduce(callbackFn,0)

}
```

## Problem 2
### Instructions
Alice and Bob each created one problem for HackerRank. A reviewer rates the two challenges, awarding points on a scale from 1 to 100 for three categories: problem clarity, originality, and difficulty.

The rating for Alice's challenge is the triplet a = (a[0], a[1], a[2]), and the rating for Bob's challenge is the triplet b = (b[0], b[1], b[2]).

The task is to find their comparison points by comparing a[0] with b[0], a[1] with b[1], and a[2] with b[2].

    - If a[i] > b[i], then Alice is awarded 1 point.
    - If a[i] < b[i], then Bob is awarded 1 point.
    - If a[i] = b[i], then neither person receives a point.
Comparison points is the total points a person earned.

Given a and b, determine their respective comparison points.

### Solution
```js
function main() {
    const ws = fs.createWriteStream(process.env.OUTPUT_PATH);

    const a = readLine().replace(/\s+$/g, '').split(' ').map(aTemp => parseInt(aTemp, 10));

    const b = readLine().replace(/\s+$/g, '').split(' ').map(bTemp => parseInt(bTemp, 10));

    const result = compareTriplets(a, b);

    ws.write(result.join(' ') + '\n');

    ws.end();
}
```
