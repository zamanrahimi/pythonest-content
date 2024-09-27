
# Multi-Choice, True, False Questions

---

1. **What will the following code output?**
   ```python title="Example"
   def greet(name="Guest"):
       return f"Hello, {name}!"

   print(greet())
   ```
   - A. `Hello, Guest!`
   - B. `None`
   - C. `Hello, !`
   - D. `Error`
   - **Answer**: A

---

2. **What is the difference between a parameter and an argument?**
   - A. A parameter is passed during function invocation; an argument is defined in the function.
   - B. A parameter is a placeholder in the function; an argument is the actual data passed to the function.
   - C. They are the same.
   - D. An argument is defined using the `def` keyword.
   - **Answer**: B

---

3. **True or False: Keyword arguments must always come before positional arguments.**
   - A. True
   - B. False
   - **Answer**: B

---

4. **What is the output of the following code?**
   ```python title="Example"
   def add(x, y=5):
       return x + y

   print(add(3))
   ```
   - A. `8`
   - B. `3`
   - C. `5`
   - D. `Error`
   - **Answer**: A

---

5. **What does the `global` keyword do in Python?**
   - A. It allows you to access local variables inside a function.
   - B. It allows a function to modify a global variable.
   - C. It makes a variable global for all functions.
   - D. It creates a new global variable.
   - **Answer**: B

---

6. **Which of the following statements about positional arguments is true?**
   - A. They must always be strings.
   - B. Their order matters.
   - C. They can only be used with the `def` keyword.
   - D. Their order doesn’t matter if followed by keyword arguments.
   - **Answer**: B

---

7. **What is the output of the following code?**
   ```python title="Example"
   def multiply(a, b=2):
       return a * b

   print(multiply(3, 4))
   ```
   - A. `8`
   - B. `6`
   - C. `12`
   - D. `Error`
   - **Answer**: C

---

8. **What is the scope of a variable defined outside a function in Python?**
   - A. Local
   - B. Enclosed
   - C. Global
   - D. Built-in
   - **Answer**: C

---

9. **True or False: You can pass both positional and keyword arguments in the same function call.**
   - A. True
   - B. False
   - **Answer**: A

---

10. **What will happen if a function tries to modify a global variable without the `global` keyword?**
    - A. It will modify the global variable.
    - B. It will modify a local copy of the variable.
    - C. It will throw an error.
    - D. It will modify the variable for that function only.
    - **Answer**: B

---

11. **What is the correct way to pass keyword arguments in this function?**
    ```python title="Example"
    def describe_person(name, age, job):
        return f"{name} is {age} years old and works as a {job}."
    ```
    - A. `describe_person("John", 30, job="Engineer")`
    - B. `describe_person(name="John", age=30, "Engineer")`
    - C. `describe_person(30, job="Engineer", name="John")`
    - D. `describe_person(job="Engineer", name="John", age=30)`
    - **Answer**: D

---

12. **What will the following code output?**
    ```python title="Example"
    def outer():
        x = 10
        def inner():
            x = 5
            return x
        return inner()
    
    print(outer())
    ```
    - A. `10`
    - B. `5`
    - C. `Error`
    - D. `None`
    - **Answer**: B

---

13. **True or False: A variable defined inside a function has global scope.**
    - A. True
    - B. False
    - **Answer**: B

---

14. **What is the output of the following code?**
    ```python title="Example"
    x = 100

    def change_x():
        global x
        x = 200
    
    change_x()
    print(x)
    ```
    - A. `100`
    - B. `200`
    - C. `None`
    - D. `Error`
    - **Answer**: B

---

15. **Which of the following is the correct way to define a function with default parameters?**
    - A. `def my_func(a=10, b):`
    -

 B. `def my_func(a, b=10):`
    - C. `def my_func(a=10, b=20):`
    - D. `def my_func(a, b=20, c):`
    - **Answer**: B

---

16. **What will the following code output?**
    ```python title="Example"
    def example(a, b=5):
        return a + b
    
    print(example(10, b=3))
    ```
    - A. `13`
    - B. `15`
    - C. `8`
    - D. `Error`
    - **Answer**: A

---

17. **Which of the following is NOT a valid argument passing technique?**
    - A. Positional arguments
    - B. Keyword arguments
    - C. Default arguments
    - D. Dynamic arguments
    - **Answer**: D

---

18. **Which keyword is used to access a global variable from within a function?**
    - A. `global`
    - B. `local`
    - C. `enclosed`
    - D. `nonlocal`
    - **Answer**: A

---

19. **What is the difference between local and global variables?**
    - A. Local variables are defined inside functions, global variables are defined outside.
    - B. Global variables are more secure.
    - C. Local variables cannot be accessed outside the function.
    - D. Both A and C.
    - **Answer**: D

---

20. **What will the following code output?**
    ```python title="Example"
    def example(a, b=5):
        a = 3
        return a + b

    print(example(10))
    ```
    - A. `8`
    - B. `15`
    - C. `Error`
    - D. `3`
    - **Answer**: A

---
