# PCEP-30-02 4.2 – Organize Interaction Between the Function and Its Environment

---

# 1. Parameters vs. Arguments

### Parameters:
- Parameters are the variables listed in a function's definition. They act as placeholders for values that the function will use when called.

### Arguments:
- Arguments are the actual values or data you pass into the function when calling it.


```python title="Example"
def add(x, y):  # x and y are parameters
    return x + y

result = add(3, 5)  # 3 and 5 are arguments
print(result)  # Output: 8
```

### Key Difference:
- **Parameters** define what inputs a function expects, while **arguments** are the real data provided when calling the function.

---

# 2. Positional, Keyword, and Mixed Argument Passing

### Positional Arguments:
- These are passed to the function in the order in which the parameters are defined. The position of each argument corresponds to the position of the parameter.


```python title="Example"
def greet(first_name, last_name):
    print(f"Hello, {first_name} {last_name}!")

greet("John", "Doe")  # Output: Hello, John Doe!
```

### Keyword Arguments:
- You can pass arguments by explicitly naming the parameter when calling the function. This allows you to specify arguments in any order.


```python title="Example"
greet(last_name="Doe", first_name="John")  # Output: Hello, John Doe!
```

### Mixed Argument Passing:
- You can mix positional and keyword arguments when calling a function, but positional arguments must come before keyword arguments.


```python title="Example"
greet("John", last_name="Doe")  # Output: Hello, John Doe!
```

---

# 3. Default Parameter Values

You can provide default values to parameters in a function definition. If no argument is passed for that parameter, the default value is used.


```python title="Example"
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()          # Output: Hello, Guest!
greet("Alice")   # Output: Hello, Alice!
```

### Key Point:
- If an argument is provided, it overrides the default value.

---

# 4. Name Scopes, Name Hiding (Shadowing), and the `global` Keyword

### Name Scopes:
- Variables have different scopes based on where they are defined. A variable inside a function is local to that function, while a variable defined outside all functions is global.


```python title="Example"
x = 10  # Global scope

def func():
    x = 5  # Local scope (shadows global x)
    print(x)

func()  # Output: 5
print(x)  # Output: 10 (global x)
```

### Name Hiding (Shadowing):
- When a local variable in a function has the same name as a global variable, the local variable shadows (hides) the global variable within the function’s scope.


```python title="Example"
y = 100

def shadow():
    y = 50
    print(y)  # Output: 50 (local variable)

shadow()
print(y)  # Output: 100 (global variable)
```

### The `global` Keyword:
- To modify a global variable from within a function, you must use the `global` keyword.


```python title="Example"
z = 20

def modify_global():
    global z
    z = 15

modify_global()
print(z)  # Output: 15 (global variable modified)
```

---
