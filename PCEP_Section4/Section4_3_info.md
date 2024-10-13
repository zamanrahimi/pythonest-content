# PCEP-30-02 4.3 – Python Built-In Exceptions Hierarchy

---

# 1. BaseException

### Description:
- `BaseException` is the root of all exceptions in Python. It is the base class for all built-in exceptions. All other exceptions, including user-defined ones, derive from this class.


```python title="Example"
try:
    raise BaseException("This is a BaseException.")
except BaseException as e:
    print(e)
```
### Output:
```
This is a BaseException.
```

- This class should be used sparingly and only when you want to catch absolutely every exception, including system-related ones.

---

# 2. Exception

### Description:
- `Exception` is the base class for all standard (non-system) exceptions. It is derived from `BaseException`, and it is more commonly used than `BaseException` to catch typical exceptions in Python code.


```python title="Example"
try:
    raise Exception("This is an Exception.")
except Exception as e:
    print(e)
```
### Output:
```
This is an Exception.
```

- Use `Exception` for catching typical runtime errors in your application.

---

# 3. SystemExit

### Description:
- `SystemExit` is an exception that is raised when Python’s `sys.exit()` function is called. It is not an error; instead, it is used to exit a running program.


```python title="Example"
import sys
try:
    sys.exit("Exiting the program!")
except SystemExit as e:
    print(e)
```
### Output:
```
Exiting the program!
```

- Catching `SystemExit` allows you to perform cleanup tasks before the program exits.

---

# 4. KeyboardInterrupt

### Description:
- `KeyboardInterrupt` is an exception that is raised when the user interrupts the program execution, typically by pressing `Ctrl + C` on the keyboard.


```python title="Example"
try:
    while True:
        pass
except KeyboardInterrupt:
    print("Program interrupted by user!")
```
### Output (after pressing Ctrl + C):
```
Program interrupted by user!
```

- Use this to handle cases where you want to stop a long-running process via user interruption.

---

# 5. Abstract Exceptions

### Description:
- Some exceptions are abstract and are not intended to be raised directly. They serve as a base for other, more specific exceptions.

#### Examples:
- `ArithmeticError`: Base class for errors related to arithmetic operations.
- `LookupError`: Base class for errors that occur when a key or index is not found in a mapping or sequence.

These classes are meant to be inherited by specific exceptions like `ZeroDivisionError` or `IndexError`.

---

# 6. ArithmeticError

### Description:
- `ArithmeticError` is the base class for exceptions related to arithmetic operations.

#### Examples of subclasses:
- `ZeroDivisionError`: Raised when division by zero is attempted.
- `OverflowError`: Raised when the result of an arithmetic operation is too large to be represented.


```python title="Example"
try:
    result = 10 / 0
except ArithmeticError as e:
    print(f"Arithmetic error occurred: {e}")
```
### Output:
```
Arithmetic error occurred: division by zero
```

---

# 7. LookupError

### Description:
- `LookupError` is the base class for exceptions raised when a lookup operation (like indexing) fails.

#### Examples of subclasses:
- `IndexError`: Raised when trying to access an index that is out of range.
- `KeyError`: Raised when trying to access a key that does not exist in a dictionary.


```python title="Example"
my_list = [1, 2, 3]
try:
    print(my_list[5])
except LookupError as e:
    print(f"Lookup error occurred: {e}")
```
### Output:
```
Lookup error occurred: list index out of range
```

---

# 8. IndexError

### Description:
- `IndexError` is raised when attempting to access an index in a sequence (like a list) that is out of range.


```python title="Example"
my_list = [1, 2, 3]
try:
    print(my_list[10])
except IndexError as e:
    print(f"IndexError: {e}")
```
### Output:
```
IndexError: list index out of range
```

---

# 9. KeyError

### Description:
- `KeyError` is raised when trying to access a key that is not present in a dictionary.


```python title="Example"
my_dict = {"name": "Alice", "age": 30}
try:
    print(my_dict["height"])
except KeyError as e:
    print(f"KeyError: {e}")
```
### Output:
```
KeyError: 'height'
```

---

# 10. TypeError

### Description:
- `TypeError` is raised when an operation or function is applied to an object of inappropriate type.


```python title="Example"
try:
    result = "2" + 3
except TypeError as e:
    print(f"TypeError: {e}")
```
### Output:
```
TypeError: can only concatenate str (not "int") to str
```

---

# 11. ValueError

### Description:
- `ValueError` is raised when a function receives an argument of the correct type but with an inappropriate value.


```python title="Example"
try:
    number = int("abc")
except ValueError as e:
    print(f"ValueError: {e}")
```
### Output:
```
ValueError: invalid literal for int() with base 10: 'abc'
```

---
