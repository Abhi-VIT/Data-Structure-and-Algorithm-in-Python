# Python Basics and Data Types

This document provides a brief overview of Python basics, a description of its standard data types, and their mutability status.

## 1. Python Basics

Python is a high-level, interpreted programming language known for its readability and simplicity.
- **Mutable**: The object's value *can* be changed after it is created.
- **Immutable**: The object's value *cannot* be changed after it is created. (New objects are created when "modifying").

### Variables and Syntax
- **Variables**: Containers for storing data values. Python has no command for declaring a variable; it is created the moment you first assign a value to it.
- **Indentation**: Python uses indentation (whitespace) to define scope (e.g., loops, functions, classes) instead of brackets `{}`.

```python
x = 5           # Integer
y = "Hello"     # String
if x > 0:
    print("Positive")  # Indentation is crucial
```

### Comments
Comments start with a `#`, and Python renders the rest of the line as a comment.

```python
# This is a comment
print("Hello, World!") # This is also a comment
```

### Input/Output
- **`print()`**: Outputs data to the screen.
- **`input()`**: Allows user input.

```python
name = input("Enter your name: ")
print("Hello, " + name)
```

## 2. Python Data Types

Python has the following built-in data types by default.

### Numeric Types (Immutable)
- **`int`**: Integers (whole numbers), positive or negative, without decimals.
  ```python
  x = 10
  ```
- **`float`**: Floating point numbers, positive or negative, containing one or more decimals.
  ```python
  x = 10.5
  ```
- **`complex`**: Complex numbers are written with a "j" as the imaginary part.
  ```python
  x = 1j
  ```

### Text Type (Immutable)
- **`str`**: Strings in Python are surrounded by either single quotation marks or double quotation marks. You cannot change individual characters in place.
  ```python
  x = "Hello World"
  ```

### Sequence Types
- **`list` (Mutable)**: Ordered and changeable. Allows duplicate members.
  ```python
  x = ["apple", "banana", "cherry"]
  x[0] = "orange" # Valid
  ```
- **`tuple` (Immutable)**: Ordered and unchangeable. Allows duplicate members.
  ```python
  x = ("apple", "banana", "cherry")
  # x[0] = "orange" # Error
  ```
- **`range` (Immutable)**: Represents a sequence of numbers.
  ```python
  x = range(6)
  ```

### Mapping Type (Mutable)
- **`dict`**: Ordered (as of Python 3.7+) and changeable. No duplicate keys.
  ```python
  x = {"name": "John", "age": 36}
  x["age"] = 40 # Valid
  ```

### Set Types
- **`set` (Mutable)**: Unordered, unindexed, and no duplicate members.
  ```python
  x = {"apple", "banana", "cherry"}
  x.add("orange") # Valid
  ```
- **`frozenset` (Immutable)**: Immutable version of a set.
  ```python
  x = frozenset({"apple", "banana", "cherry"})
  ```

### Boolean Type (Immutable)
- **`bool`**: Represents one of two values: `True` or `False`.
  ```python
  x = True
  ```

### None Type (Immutable)
- **`NoneType`**: Represents the absence of a value or a null value.
  ```python
  x = None
  ```

## Summary: Mutable vs Immutable

| **Mutable (Can Change)** | **Immutable (Cannot Change)** |
| :--- | :--- |
| `list` | `int`, `float`, `complex` |
| `dict` | `str` |
| `set` | `tuple` |
| `bytearray` | `range` |
| | `frozenset` |
| | `bool` |
| | `None` |
