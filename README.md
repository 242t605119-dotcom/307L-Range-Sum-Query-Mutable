# LeetCode 307 - Range Sum Query - Mutable

## Problem Statement

Given an integer array `nums`, handle two types of operations:

* Update the value of an element.
* Calculate the sum of elements between two indices.

## Example

### Input

```text id="3j4h4u"
nums = [1, 3, 5]
sumRange(0, 2)
update(1, 2)
sumRange(0, 2)
```

### Output

```text id="1f9g4n"
9
8
```

## Approach

Use a **Fenwick Tree (Binary Indexed Tree)** to efficiently update elements and calculate range sums.

## Algorithm

1. Build a Fenwick Tree from the given array.
2. For an update, calculate the difference between the new and old values.
3. Update the Fenwick Tree using this difference.
4. Calculate prefix sums using the tree.
5. Find the range sum using two prefix sums.

## Time Complexity

* Initialization: `O(n log n)`
* Update: `O(log n)`
* Sum Query: `O(log n)`

## Space Complexity

`O(n)`

## Key Concepts

* Fenwick Tree
* Binary Indexed Tree
* Prefix Sum
* Range Query
* Array Update

## Language

Python

## LeetCode Details

* **Problem:** 307
* **Title:** Range Sum Query - Mutable
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
