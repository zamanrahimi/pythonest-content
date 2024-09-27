# PCEP-30-02 4.4 – Basics of Python Exception Handling

---

# 1. `try-except` / the `try-except` Exception

### Description:
- The `try-except` block is used to handle exceptions in Python. Code that may raise an exception is placed inside the `try` block, and the handling of that exception is placed inside the `except` block.
- If an exception is raised inside the `try` block, the `except` block catches and handles it.


```python title="Example"
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
```

### Output:
```
Cannot divide by zero!
```

- In this example, the `ZeroDivisionError` is caught and handled by the `except` block.

---

# 2. Ordering the `except` Branches

### Description:
- Multiple `except` clauses can be used to handle different exceptions. More specific exceptions should be listed first because Python will check the `except` blocks in order, from top to bottom.
- If a general exception (like `Exception`) is placed before a more specific exception (like `ZeroDivisionError`), the specific exception will never be caught.


```python title="Example"
try:
    result = 10 / 0
except ZeroDivisionError:
    print("ZeroDivisionError caught")
except ArithmeticError:
    print("ArithmeticError caught")
except Exception:
    print("General Exception caught")
```

### Output:
```
ZeroDivisionError caught
```

- Python tries to match the raised exception to the most specific `except` branch. In this case, `ZeroDivisionError` is caught because it’s more specific than `ArithmeticError`.

---

# 3. Propagating Exceptions Through Function Boundaries

### Description:
- Exceptions raised inside a function can propagate outside the function, meaning that if a function raises an exception and it is not caught inside the function, it will propagate to the caller.
- If the calling code also does not catch the exception, it will propagate further up the call stack.


```python title="Example"
def divide(a, b):
    return a / b

try:
    divide(10, 0)
except ZeroDivisionError:
    print("Exception propagated to the caller.")
```

### Output:
```
Exception propagated to the caller.
```

- Here, the `ZeroDivisionError` raised inside the `divide()` function is caught outside the function, demonstrating exception propagation through function boundaries.

---

# 4. Delegating Responsibility for Handling Exceptions

### Description:
- Sometimes, it is better to let the calling code handle exceptions rather than catching them inside the function where they occur. This is known as delegating the responsibility for handling exceptions.
- By using the `raise` keyword, you can re-raise an exception inside the `except` block, allowing the caller to handle it.


```python title="Example"
def divide(a, b):
    try:
        return a / b
    except ZeroDivisionError:
        print("Handling inside the function.")
        raise  # Re-raise the exception

try:
    divide(10, 0)
except ZeroDivisionError:
    print("Handled by the caller.")
```

### Output:
```
Handling inside the function.
Handled by the caller.
```

- Here, the exception is caught inside the `divide()` function, but it is re-raised to allow the caller to handle it.

---
