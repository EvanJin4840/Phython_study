# Python Key Concepts Guide

A quick reference for Python essentials, coming from C/C++/Java background.

## Dynamic Typing

| Feature | C/C++/Java | Python |
|---------|------------|--------|
| Variable Declaration | `int x = 5;` | `x = 5` |
| Type Declaration | Required | Optional (inferred at runtime) |
| Type Annotations | Not available (except C++11+) | Supported from Python 3.5+ |

**Example:**
```python
x = 5          # Integer
name = "John"  # String
price = 9.99   # Float
```
* Type annotations (also called "type hints") are a Python feature that let you explicitly specify the expected data types of variables, function parameters, and return values. They were introduced in Python 3.5 (PEP 484) to bring optional static typing to Python's dynamically typed nature.

#### Iterators and Generators

- Iterators are objects that can be looped over, implementing __iter__() and __next__() methods. Generators use the yield keyword to produce values on-demand, making them memory-efficient for large datasets:
- Generators are useful when processing large files or infinite sequences without loading everything into memory.

### Decorators

- A decorator is a higher‑order function that takes another function as input, wraps it inside an inner function (often called wrapper) where it can run extra code before and/or after the original function call, and then returns this wrapper as the new version of the function.
- Using the @decorator_name syntax above a function definition is just shorthand for “pass this function into the decorator and replace it with the decorated version.”
This lets you add reusable cross‑cutting features like logging, timing, authentication checks, caching, or validation to many functions, without changing their original bodies and while keeping their core logic clean.