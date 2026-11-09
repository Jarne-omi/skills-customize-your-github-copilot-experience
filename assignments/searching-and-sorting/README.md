# 📘 Assignment: Searching and Sorting Algorithms

## 🎯 Objective

Implement linear search and selection sort in Python, and count the comparisons each algorithm makes. Use those counts to explore how an algorithm's work changes with the input.

## 📝 Tasks

### 🛠️ Implement Linear Search

#### Description
Write a function that checks each item in a list until it finds a target value or reaches the end. Return both the target's index and the number of equality checks made.

#### Requirements
Completed program should:

- Define `linear_search(values, target)` and return `(index, comparisons)`.
- Return the index of the first matching value, or `-1` if the target is not present.
- Count each equality check, including the final check that finds the target; an empty list should require zero checks.

### 🛠️ Implement Selection Sort

#### Description
Write selection sort to produce a new list with the values in ascending order. Count each comparison between two values as the algorithm looks for the next smallest value.

#### Requirements
Completed program should:

- Define `selection_sort(values)` and return `(sorted_values, comparisons)`.
- Sort without using Python's built-in `sort()` method or `sorted()` function.
- Leave the original list unchanged and return zero comparisons for lists with fewer than two items.

### 🛠️ Compare the Work

#### Description
Run both functions with lists of different lengths. Try searching for a value at the start, at the end, and not in the list. Record the comparison counts and describe what you notice.

#### Requirements
Completed program should:

- Print the result and comparison count for each search and sort test.
- Include tests for an empty list, a one-item list, and a list with several items.
- Add a short written observation describing how search position and list length affect the comparison counts.
