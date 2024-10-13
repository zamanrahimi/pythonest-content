# Multi-Choice, True, False Questions

---

1. **What is the output of the following code?**
   ```python title="Example"
   def greet(name):
       return f"Hello, {name}!"

   print(greet("Alice"))
   ```
   - A. `Hello Alice!`
   - B. `Hello, Alice!`
   - C. `Hi, Alice!`
   - D. `None`
   - **Answer**: B

---

2. **Which of the following correctly defines a function in Python?**
   - A. `def my_function{}`
   - B. `def my_function():`
   - C. `my_function = function():`
   - D. `def my_function:`
   - **Answer**: B

---

3. **True or False: A function in Python can return multiple values.**
   - A. True
   - B. False
   - **Answer**: A

---

4. **What will the following code print?**
   ```python title="Example"
   def do_something():
       return 5

   print(do_something())
   ```
   - A. `None`
   - B. `5`
   - C. `do_something()`
   - D. `Error`
   - **Answer**: B

---

5. **What is the output of the following generator?**
   ```python title="Example"
   def count():
       yield 1
       yield 2
       yield 3

   for num in count():
       print(num)
   ```
   - A. `1 2 3`
   - B. `1 1 1`
   - C. `None`
   - D. `Error`
   - **Answer**: A

---

6. **Which keyword is used to exit a function and return a value?**
   - A. `break`
   - B. `continue`
   - C. `return`
   - D. `yield`
   - **Answer**: C

---

7. **What does the following function return if no argument is passed?**
   ```python title="Example"
   def greet(name="Guest"):
       return f"Hello, {name}!"
   ```
   - A. `Hello, Guest!`
   - B. `None`
   - C. `Hello, !`
   - D. `Error`
   - **Answer**: A

---

8. **True or False: A generator can return a value using the `return` keyword.**
   - A. True
   - B. False
   - **Answer**: B

---

9. **What is the output of the following code?**
   ```python title="Example"
   def add(a, b):
       print(a + b)

   result = add(3, 4)
   print(result)
   ```
   - A. `7 None`
   - B. `7`
   - C. `None`
   - D. `Error`
   - **Answer**: A

---

10. **Which keyword is used to define a generator in Python?**
    - A. `return`
    - B. `yield`
    - C. `break`
    - D. `continue`
    - **Answer**: B

---

11. **What will happen if a recursive function does not have a base case?**
    - A. It will return `None`.
    - B. It will run indefinitely until it crashes.
    - C. It will exit automatically after 1000 calls.
    - D. It will throw a syntax error.
    - **Answer**: B

---

12. **What is the result of the following function?**
    ```python title="Example"
    def factorial(n):
        if n == 0:
            return 1
        else:
            return n * factorial(n - 1)
    
    print(factorial(3))
    ```
    - A. `3`
    - B. `6`
    - C. `0`
    - D. `1`
    - **Answer**: B

---

13. **True or False: The `None` keyword is returned by default if a function does not have a `return` statement.**
    - A. True
    - B. False
    - **Answer**: A

---

14. **What will the following code print?**
    ```python title="Example"
    def my_func():
        pass

    print(my_func())
    ```
    - A. `None`
    - B. `Error`
    - C. `0`
    - D. `my_func()`
    - **Answer**: A

---

15. **Which of the following is the correct definition of a recursive function?**
    - A. A function that calls another function.
    - B. A function that calls itself.
    - C. A function that runs indefinitely.
    - D. A function with no return value.
    - **Answer**: B

---

16. **What is the output of the following code?**
    ```python title="Example"
    def even_numbers(n):
        for i in range(n):
            if i % 2 == 0:
                yield i
    
    print(list(even_numbers(5)))
    ```
    - A. `[0, 1, 2, 3, 4]`
    - B. `[0, 2, 4]`
    - C. `[2, 4, 6]`
    - D. `Error`
    - **Answer**: B

---

17. **Which of the following correctly represents a base case in a recursive function?**
    - A. `if x == 1: return x`
    - B. `if x > 0: return x`
    - C. `if x != 1: return None`
    - D. `if x == 0: pass`
    - **Answer**: A

---

18. **What will the following code print?**
    ```python title="Example"
    def my_func(a, b=10):
        return a + b

    print(my_func(5))
    ```
    - A. `15`
    -

 B. `10`
    - C. `5`
    - D. `Error`
    - **Answer**: A

---

19. **True or False: The `yield` keyword can be used in a standard function (non-generator).**
    - A. True
    - B. False
    - **Answer**: B

---

20. **Which of the following is an example of recursion?**
    - A. `def my_func(): return my_func()`
    - B. `def my_func(x): return my_func(x-1)`
    - C. `def my_func(): return my_func() if False else 0`
    - D. `def my_func(x): return my_func(x-1) if x > 0 else x`
    - **Answer**: D

---