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