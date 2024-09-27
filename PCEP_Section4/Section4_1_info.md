# **Section** 4: Functions and Exceptions (28%)
# PCEP-30-02 4.1 – Decompose the Code Using Functions

---

# 1. Defining and Invoking User-Defined Functions and Generators

### Functions:
A function in Python is a reusable block of code that performs a specific task. Functions are defined using the `def` keyword, followed by a function name, parentheses, and a colon. Code inside the function is indented.

### Syntax for defining a function:

```python title="Example"
def function_name(parameters):
    # Function body
    return value
```

```python title="Example"
def greet(name):
    return f"Hello, {name}!"

# Invoking the function
print(greet("Alice"))  # Output: Hello, Alice!
```

### Generators:
A generator is a special type of iterator that allows you to iterate over a sequence of values lazily (one at a time). A generator is defined like a function but uses the `yield` keyword to produce values one at a time.

### Syntax for defining a generator:
```python title="Example"
def my_generator():
    yield value
```


```python title="Example"
def countdown(n):
    while n > 0:
        yield n
        n -= 1

# Invoking the generator
for number in countdown(5):
    print(number)  # Output: 5, 4, 3, 2, 1
```

---

# 2. The `return` Keyword, Returning Results

The `return` keyword is used to exit a function and optionally send back a value to the caller. Once `return` is encountered, the function execution stops.


```python title="Example"
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

If no `return` statement is present, Python automatically returns `None`.

---

# 3. The `None` Keyword

`None` is a special keyword in Python that represents the absence of a value or a null value. It is used to signify that a variable or function has no value.


```python title="Example"
def do_nothing():
    pass

result = do_nothing()
print(result)  # Output: None
```

You can explicitly return `None` using the `return None` statement.

---

# 4. Recursion

Recursion is a technique where a function calls itself. A recursive function must have a **base case** to avoid infinite recursion. It's often used to solve problems that can be broken down into smaller sub-problems of the same type.


```python title="Example"
def factorial(n):
    if n == 1:  # Base case
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # Output: 120
```

---
