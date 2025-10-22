# advanced-algorithms-java
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
Overview
A growing collection of algorithm implementations in Java, developed as part of my university Advanced Algorithms (COM2031) module. Each lab focuses on applying divide-and-conquer techniques and algorithmic design principles to efficiently solve computational problems.
The repository showcases core algorithmic patterns such as recursion, partitioning, randomisation, and performance testing, implemented from first principles without relying on Java’s built-in sort or collection utilities.

How It Works
Each algorithm is implemented in a separate Java class with an embedded testing routine (main method) for validation.
Lab 02 – Divide and Conquer Algorithms
Kth Smallest Element
Implements a recursive divide-and-conquer algorithm to find the k-th smallest element in an unsorted list without fully sorting the array.
Uses partitioning logic similar to Quickselect.
Divides the array into left/right sublists around a pivot, recursively discarding unnecessary partitions.

Key Concepts:
Recursion and base cases
Array partitioning
Subproblem reduction and re-use
Test-driven design with predefined data sets

Quick Sort
Classic implementation of Quicksort, recursively dividing an array into smaller partitions using a pivot and combining results to produce a fully sorted list.
Implements its own left/right partition logic and avoids using Java’s built-in sort.
Includes automated test cases comparing results with Java’s Arrays.sort() to verify correctness.

Key Concepts:

Divide and conquer
Recursion and partition logic
Combining results from sorted subproblems
Benchmarking against standard library methods

Features
Pure Java implementations — no external libraries used.
Fully recursive algorithm structure following divide-and-conquer principles.
Inline test functions (testKthSmallest(), testQuickSort()) for validation.
Randomised large-array testing for performance and correctness verification.
Clear and modular class-based structure (KthSmallest.java, QuickSort.java).

Project Structure
/advanced-algorithms-labs/
│
├── lab02/
│   ├── KthSmallest.java
│   └── QuickSort.java
│
└── README.md

Skills Demonstrated

Algorithm Design: Recursive decomposition, partitioning, and problem reduction.
Java Programming: Arrays, ArrayLists, generics, and static method design.
Divide & Conquer: Implementation and analysis of recursive algorithms.
Testing & Debugging: Custom testing functions and comparison against Java’s standard library.
Complexity Awareness: Understanding time complexity and trade-offs between algorithms.
Clean Code Practices: Consistent naming, modular classes, inline documentation, and code comments.

Possible Improvements

Benchmarking:
Add timing utilities (System.nanoTime()) to compare performance on different input sizes.
Generics:
Generalize algorithms to work with generic comparable types (<T extends Comparable<T>>).
Error Handling:
Validate k values for KthSmallest to ensure they remain within array bounds.
Visualization:
Add optional console or graphical visualisation of partitioning and recursive depth.
Testing Framework:
Convert embedded tests into JUnit tests for structured, automated verification.

Status
This repository is in progress and will be expanded as more algorithms are implemented throughout the module — including Merge Sort, Binary Search, Closest Pair, and other divide-and-conquer problems.
