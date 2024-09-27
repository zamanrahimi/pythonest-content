# PCEP-30-02 3.3 – Collect and Process Data Using Dictionaries

---

# 1. Dictionaries: Building

A **dictionary** in Python is a collection of key-value pairs. Dictionaries are mutable and unordered, which means that they can change and do not maintain the order of elements.

### Building a Dictionary
You can create a dictionary using curly braces `{}` or the `dict()` function.

```python title="Example"
# Using curly braces
my_dict = {'name': 'Alice', 'age': 25}

# Using the dict() function
my_dict = dict(name='Alice', age=25)

print(my_dict)  # Output: {'name': 'Alice', 'age': 25}
```

---

# 2. Indexing

To access values in a dictionary, you use the corresponding keys.

```python title="Example"
my_dict = {'name': 'Alice', 'age': 25}
print(my_dict['name'])  # Output: Alice
```

Attempting to access a key that does not exist will raise a `KeyError`.

```python title="Example"
# print(my_dict['gender'])  # Uncommenting this will raise a KeyError
```

---

# 3. Adding and Removing Keys

You can add new key-value pairs or modify existing ones using assignment.

### Adding a Key-Value Pair
```python title="Example"
my_dict['gender'] = 'Female'
print(my_dict)  # Output: {'name': 'Alice', 'age': 25, 'gender': 'Female'}
```

### Removing a Key-Value Pair
You can remove a key using the `del` statement or the `pop()` method.

```python title="Example"
del my_dict['age']
print(my_dict)  # Output: {'name': 'Alice', 'gender': 'Female'}

# Using pop()
gender = my_dict.pop('gender')
print(gender)  # Output: Female
print(my_dict)  # Output: {'name': 'Alice'}
```

---

# 4. Iterating Through Dictionaries

You can iterate through dictionaries to access keys, values, or both.

### Iterating Through Keys
```python title="Example"
for key in my_dict:
    print(key)  # Output: name
```

### Iterating Through Values
```python title="Example"
for value in my_dict.values():
    print(value)  # Output: Alice
```

### Iterating Through Keys and Values
```python title="Example"
for key, value in my_dict.items():
    print(f"{key}: {value}")  # Output: name: Alice
```

---

# 5. Checking the Existence of Keys

You can check if a key exists in a dictionary using the `in` keyword.

```python title="Example"
if 'name' in my_dict:
    print("Name exists in the dictionary")  # Output: Name exists in the dictionary
```

---

# 6. Methods: `keys()`, `items()`, and `values()`

### `keys()`
Returns a view object that displays a list of all the keys in the dictionary.

```python title="Example"
print(my_dict.keys())  # Output: dict_keys(['name'])
```

### `values()`
Returns a view object that displays a list of all the values in the dictionary.

```python title="Example"
print(my_dict.values())  # Output: dict_values(['Alice'])
```

### `items()`
Returns a view object that displays a list of dictionary's key-value tuple pairs.

```python title="Example"
print(my_dict.items())  # Output: dict_items([('name', 'Alice')])
```

---
