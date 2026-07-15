# Time and Space Complexity

## Introduction

When developing a program or solving a problem, multiple algorithms can produce the same result. However, not all algorithms perform equally. Some execute faster, while others use less memory. Time and Space Complexity help us analyze and compare algorithms to choose the most efficient solution.

---

# What is Time Complexity?

Time Complexity measures how the execution time of an algorithm grows as the input size increases.

It does **not** measure the actual execution time in seconds or milliseconds. Instead, it measures the growth in the number of operations performed by an algorithm.

### Example

If an array contains 100 elements, a Linear Search may check all 100 elements in the worst case.

Therefore, the Time Complexity is:

```text
O(n)
```

---

# What is Space Complexity?

Space Complexity measures the amount of memory required by an algorithm as the input size increases.

Some algorithms execute faster by using additional memory, while others use less memory but require more execution time.

### Example

If an algorithm creates another array of size **n**, the extra memory required increases with the input size.

---

# Why Do We Analyze Time and Space Complexity?

Time and Space Complexity help us:

* Compare different algorithms.
* Choose the most efficient solution.
* Improve application performance.
* Reduce unnecessary execution time.
* Optimize memory usage.

---

# Time vs Space Trade-off

In many situations, Time and Space Complexity have a trade-off.

* Faster algorithms may require more memory.
* Memory-efficient algorithms may require more execution time.

The choice depends on the application requirements.

---

# Big O Notation

Big O Notation represents the **Worst Case Time Complexity** of an algorithm.

It describes how the performance of an algorithm changes as the input size increases.

---

# Types of Asymptotic Notations

## 1. Big O - Worst Case

Represents the maximum execution time required by an algorithm.

### Example

Linear Search when the element is at the last position.

---

## 2. Big Omega (Ω) - Best Case

Represents the minimum execution time.

### Example

Linear Search when the element is found at the first position.

---

## 3. Big Theta (Θ) - Average Case / Tight Bound

Represents the average running time when both upper and lower bounds are the same.

---

# Common Time Complexities

## O(1) - Constant Time

The execution time remains constant regardless of the input size.

### Example

* Accessing an array element using its index.
* Updating an element using its index.

---

## O(log n) - Logarithmic Time

The input size is reduced by half in every step.

### Example

Binary Search.

The search space is repeatedly divided into two halves until the required element is found.

---

## O(n) - Linear Time

Every element is processed exactly once.

### Example

Linear Search.

Traversing an entire array.

---

## O(n log n) - Linearithmic Time

The input is divided into smaller parts, and all elements are processed efficiently.

### Example

* Merge Sort
* Heap Sort
* Quick Sort (Average Case)

---

## O(n²) - Quadratic Time

Nested loops are used.

For every element, all other elements are checked.

### Example

Checking duplicate elements using two nested loops.

Bubble Sort (Worst Case).

---

## O(2ⁿ) - Exponential Time

Each recursive call generates two more recursive calls until the base case is reached.

The number of function calls increases exponentially.

### Example

Naive Recursive Fibonacci.

---

## O(n!) - Factorial Time

The algorithm tries every possible permutation (arrangement) to find the required solution.

This is one of the slowest time complexities.

### Example

* Generating all permutations of a string.
* N-Queens (Brute Force / Worst Case).
* Brute Force Travelling Salesman Problem (TSP).

---

# Time Complexity of Common Array Operations

| Operation              | Time Complexity |
| ---------------------- | --------------- |
| Read                   | O(1)            |
| Write / Update         | O(1)            |
| Search (Linear Search) | O(n)            |
| Insert (Middle)        | O(n)            |
| Delete (Middle)        | O(n)            |

---

# Order of Time Complexities (Best to Worst)

```text
O(1)
↓
O(log n)
↓
O(n)
↓
O(n log n)
↓
O(n²)
↓
O(2ⁿ)
↓
O(n!)
```

---

# Summary

* **O(1)** – Constant Time
* **O(log n)** – Input size is reduced by half in every step.
* **O(n)** – Every element is processed once.
* **O(n log n)** – Efficient divide-and-conquer algorithms.
* **O(n²)** – Nested loops.
* **O(2ⁿ)** – Each recursive call creates two more recursive calls until the base case.
* **O(n!)** – Tries every possible permutation (arrangement).

---

# Conclusion

Time and Space Complexity are essential concepts in Data Structures and Algorithms.

They help developers compare algorithms, improve performance, and select the most efficient solution based on execution time and memory usage.

Understanding these concepts is an important step toward writing optimized programs and solving coding interview problems efficiently.
