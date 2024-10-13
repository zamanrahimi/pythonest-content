# PCEP-30-02 3.2 – Collect and Process Data Using Tuples

---

# 1. Tuples: Indexing, Slicing, Building, Immutability

A **tuple** is a collection of ordered elements in Python, similar to lists but immutable. Tuples are defined using parentheses `()` instead of square brackets `[]`.

### Indexing
Tuples support indexing, which allows access to individual elements.

```python title="Example"
tuple_example = (1, 2, 3, 4, 5)
print(tuple_example[0])  # Output: 1
print(tuple_example[3])  # Output: 4
```

### Slicing
You can slice tuples just like lists.

```python title="Example"
tuple_example = (10, 20, 30, 40, 50)
print(tuple_example[1:4])  # Output: (20, 30, 40)
```

### Building
You can create a tuple by enclosing elements in parentheses.

```python title="Example"
tuple_building = ('apple', 'banana', 'cherry')
print(tuple_building)  # Output: ('apple', 'banana', 'cherry')
```

### Immutability
Once a tuple is created, its elements cannot be changed, added, or removed.

```python title="Example"
tuple_example = (1, 2, 3)
# tuple_example[1] = 5  # This will raise a TypeError
```

---

# 2. Tuples vs. Lists: Similarities and Differences

### Similarities
- Both tuples and lists are ordered collections.
- Both can contain heterogeneous data types (e.g., integers, strings).

### Differences
- **Mutability**: Lists are mutable; tuples are immutable.
- **Syntax**: Lists use square brackets `[]`, while tuples use parentheses `()`.
- **Performance**: Tuples are generally faster than lists for iterations due to their immutability.


```python title="Example"
list_example = [1, 2, 3]
tuple_example = (1, 2, 3)

# Attempting to change an element in a tuple will raise an error
# tuple_example[1] = 5  # Uncommenting this will raise a TypeError

list_example[1] = 5  # This works fine
print(list_example)  # Output: [1, 5, 3]
```

---

# 3. Lists Inside Tuples and Tuples Inside Lists

You can nest lists within tuples and vice versa. This allows for more complex data structures.

### Lists Inside Tuples
```python title="Example"
tuple_with_list = (1, 2, [3, 4, 5])
tuple_with_list[2].append(6)
print(tuple_with_list)  # Output: (1, 2, [3, 4, 5, 6])
```

### Tuples Inside Lists
```python title="Example"
list_with_tuple = [("apple", 1), ("banana", 2)]
list_with_tuple.append(("cherry", 3))
print(list_with_tuple)  # Output: [('apple', 1), ('banana', 2), ('cherry', 3)]
```

---


