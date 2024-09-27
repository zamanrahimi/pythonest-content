# PCEP-30-02 3.4 – Operate with Strings

---

# 1. Constructing Strings

In Python, strings are sequences of characters enclosed in quotes. You can use single quotes (`'`), double quotes (`"`), or triple quotes (`'''` or `"""`) to create strings.


```python title="Example"
single_quote_string = 'Hello, World!'
double_quote_string = "Python is fun!"
triple_quote_string = '''This is a multi-line string.'''
print(single_quote_string)  # Output: Hello, World!
print(double_quote_string)   # Output: Python is fun!
print(triple_quote_string)    # Output: This is a multi-line string.
```

---

# 2. Indexing and Slicing

Strings are indexed, meaning you can access individual characters using their position. The first character has an index of 0.

### Indexing Example:
```python title="Example"
my_string = "Python"
print(my_string[0])  # Output: P
print(my_string[5])  # Output: n
```

### Slicing Example:
You can extract a substring by specifying a range of indices.

```python title="Example"
print(my_string[0:2])  # Output: Py
print(my_string[2:])   # Output: thon
```

---

# 3. Immutability

Strings in Python are **immutable**, meaning once a string is created, it cannot be changed. Any operation that seems to modify a string actually creates a new string.


```python title="Example"
original_string = "Hello"
# Attempting to change the first character will raise an error
# original_string[0] = 'h'  # Uncommenting this will raise a TypeError

new_string = 'h' + original_string[1:]  # Correct way to modify
print(new_string)  # Output: hello
```

---

# 4. Escaping Using the `\` Character

To include special characters in strings, such as quotes or backslashes, you can use the escape character `\`.


```python title="Example"
escaped_single_quote = 'It\'s a nice day.'
escaped_double_quote = "He said, \"Hello!\""
escaped_backslash = "This is a backslash: \\"
print(escaped_single_quote)  # Output: It's a nice day.
print(escaped_double_quote)   # Output: He said, "Hello!"
print(escaped_backslash)      # Output: This is a backslash: \
```

---

# 5. Quotes and Apostrophes Inside Strings

You can include quotes or apostrophes inside strings without escaping them by using different types of quotes to enclose the string.


```python title="Example"
string_with_apostrophe = "It's a sunny day."
string_with_quotes = 'She said, "Hello!"'
print(string_with_apostrophe)  # Output: It's a sunny day.
print(string_with_quotes)       # Output: She said, "Hello!"
```

---

# 6. Multi-line Strings

Multi-line strings can be created using triple quotes. They are often used for documentation or comments.


```python title="Example"
multi_line_string = """This is a string that spans
multiple lines. It is useful for long text."""
print(multi_line_string)
```

---

# 7. Basic String Functions and Methods

Python provides many built-in string methods for common operations.

### Common Methods:
- **`len()`**: Returns the length of the string.
- **`.lower()`**: Converts the string to lowercase.
- **`.upper()`**: Converts the string to uppercase.
- **`.strip()`**: Removes leading and trailing whitespace.
- **`.replace(old, new)`**: Replaces occurrences of a substring.


```python title="Example"
sample_string = " Hello, World! "
print(len(sample_string))          # Output: 14
print(sample_string.lower())        # Output: " hello, world! "
print(sample_string.upper())        # Output: " HELLO, WORLD! "
print(sample_string.strip())        # Output: "Hello, World!"
print(sample_string.replace("World", "Python"))  # Output: " Hello, Python! "
```

---

