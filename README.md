# Data Structure and Algorithm in Python

Welcome to the **Data Structure and Algorithm in Python** repository! This project contains implementations of fundamental data structures and algorithms using Python and Jupyter Notebooks. It serves as a learning resource and reference for understanding core computer science concepts.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Implemented Modules](#implemented-modules)
  - [Binary Search](#binary-search)
  - [Linked List](#linked-list)
  - [Queue](#queue)
  - [Recursion](#recursion)

## Overview

This repository demonstrates how to implement and utilize common data structures and algorithms in Python. Each concept is explored in a dedicated Jupyter Notebook, providing code examples and explanations.

> **Note:** If you are new to Python or need a quick refresher, checking out the [Python Basics and Data Types](PYTHON_BASICS.md) guide is highly recommended.

## Prerequisites

To run the code in this repository, you need:

- **Python 3.x**
- **Jupyter Notebook** or **JupyterLab**

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Abhi-VIT/Data-Structure-and-Algorithm-in-Python.git
    cd Data-Structure-and-Algorithm-in-Python
    ```

2.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

3.  Open the desired `.ipynb` file to view and run the code.

## Implemented Modules

### Binary Search
*File: `Binary_Search.ipynb`*

This notebook demonstrates the **Binary Search** algorithm, an efficient way to find an element in a *sorted* array.
- **Algorithm**: Iteratively divides the search interval in half.
- **Key Function**: `binary_search(arr, target)`
- **Complexity**: O(log n)

### Linked List
*File: `LinkedList.ipynb`*

This notebook provides a complete implementation of a **Singly Linked List**.
- **Components**:
    - `node` class: Represents a single node with data and a pointer to the next node.
    - `LinkedList` class: Manages the list.
- **Operations**:
    - `append(data)`: Adds a node to the end.
    - `insert_first(data)`: Adds a node to the beginning.
    - `insert_last(data)`: Alias for append.
    - `insert_position(data, position)`: Inserts a node at a specific index.
    - `display()`: Prints the list elements.

### Queue
*File: `Queue.ipynb`* and `Queues.py`

This notebook explores **Queue** data structures using different approaches.
- **List Implementation**: managing a queue using a standard Python list (inefficient for large data sets due to O(n) pops from the beginning).
- **Deque Implementation**: Using `collections.deque` for efficient O(1) appends and pops from both ends.
- **Custom Queue Class**: A wrapper class around `deque` providing standard queue methods:
    - `enqueue(val)`
    - `dequeue()`
    - `is_empty()`
    - `size()`

### Recursion
*File: `Recursion.ipynb`*

This notebook illustrates the concept of **Recursion**.
- **Example**: Calculating the factorial of a number.
- **Concepts**: Base case, recursive step, and recursion depth limits (demonstrating `RecursionError`).

---
*Happy Coding!*
