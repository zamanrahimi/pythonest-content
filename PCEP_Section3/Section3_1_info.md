# **Section** 3:  Data Collections – Tuples, Dictionaries, Lists, and Strings (25%)
# PCEP-30-02 Topic 3.1 – Collect and process data using lists

---

# 1. Constructing Vectors

A **vector** in Python is essentially a list, which can store a sequence of elements (such as numbers or strings). You can create a list (vector) using square brackets `[]`, separating elements by commas.


```python title="Example"
vector = [1, 2, 3, 4, 5]
print(vector)  # Output: [1, 2, 3, 4, 5]
```

---

# 2. Indexing and Slicing

**Indexing** allows you to access individual elements of a list by their position (index). Python uses zero-based indexing, so the first element is at index 0.


```python title="Example"
vector = [10, 20, 30, 40]
print(vector[0])  # Output: 10
print(vector[3])  # Output: 40
```

**Slicing** allows you to access a subset of the list. The syntax for slicing is `list[start:end]`, where the start index is inclusive, but the end index is exclusive.


```python title="Example"
vector = [10, 20, 30, 40, 50]
print(vector[1:4])  # Output: [20, 30, 40]
```

---

# 3. The `len()` Function

The `len()` function returns the number of elements in a list.


```python title="Example"
vector = [5, 10, 15, 20]
print(len(vector))  # Output: 4
```

---

# 4. List Methods: `append()`, `insert()`, `index()`, etc.

- **`append()`**: Adds an element to the end of the list.
- **`insert(index, value)`**: Inserts an element at the specified index.
- **`index(value)`**: Returns the index of the first occurrence of the element.


```python title="Example"
vector = [1, 2, 3]
vector.append(4)
print(vector)  # Output: [1, 2, 3, 4]

vector.insert(1, 10)
print(vector)  # Output: [1, 10, 2, 3, 4]

print(vector.index(10))  # Output: 1
```

---

# 5. Functions: `len()`, `sorted()`

- **`len()`**: Already covered above.
- **`sorted()`**: Returns a sorted copy of the list (ascending by default).


```python title="Example"
vector = [3, 1, 4, 1, 5, 9]
sorted_vector = sorted(vector)
print(sorted_vector)  # Output: [1, 1, 3, 4, 5, 9]
```

---

# 6. The `del` Instruction

The `del` instruction is used to delete elements from a list based on index, or delete the entire list.


```python title="Example"
vector = [1, 2, 3, 4, 5]
del vector[1]  # Deletes the second element
print(vector)  # Output: [1, 3, 4, 5]

del vector  # Deletes the entire list
```

---

# 7. Iterating Through Lists with the `for` Loop

You can iterate through each element in a list using a `for` loop.


```python title="Example"
vector = [10, 20, 30]
for element in vector:
    print(element)
# Output:
# 10
# 20
# 30
```

---

# 8. Initializing Loops

Loops can be initialized with a starting condition or to iterate over elements directly. With lists, a `for` loop is commonly used, but `while` loops can also be used by managing indexes manually.


```python title="Example"
vector = [10, 20, 30]
i = 0
while i < len(vector):
    print(vector[i])
    i += 1
# Output:
# 10
# 20
# 30
```

---

# 9. The `in` and `not in` Operators

- **`in`**: Checks if an element exists in a list.
- **`not in`**: Checks if an element does not exist in a list.


```python title="Example"
vector = [10, 20, 30]
print(20 in vector)  # Output: True
print(50 not in vector)  # Output: True
```

---

# 10. List Comprehensions

A list comprehension provides a concise way to create lists. It consists of brackets containing an expression followed by a `for` clause.


```python title="Example"
squared = [x**2 for x in range(5)]
print(squared)  # Output: [0, 1, 4, 9, 16]
```

---

# 11. Copying and Cloning

When you assign a list to another variable, you create a reference. To create a true copy of a list, use **slicing** or the `copy()` method.


```python title="Example"
vector = [1, 2, 3]
copy_vector = vector[:]  # Cloning using slicing
copy_vector.append(4)
print(copy_vector)  # Output: [1, 2, 3, 4]
print(vector)  # Output: [1, 2, 3]
```

---

# 12. Lists in Lists: Matrices and Cubes

Lists can contain other lists, which allows you to create multi-dimensional structures like matrices (2D arrays) and cubes (3D arrays).


```python title="Example"
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(matrix[1][2])  # Output: 6 (2nd row, 3rd column)
```

---