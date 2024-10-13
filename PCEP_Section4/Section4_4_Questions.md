# Multi-Choice, True/False Questions and Answers

---

### 1. Which keyword is used to catch exceptions in Python?
- A. `try`
- B. `except`
- C. `catch`
- D. Both A and B
- **Answer**: D

---

### 2. What will the following code output?
   ```python title="Example"
   try:
       result = 10 / 0
   except ZeroDivisionError:
       print("Division by zero is not allowed.")
   ```
   - A. `None`
   - B. `ZeroDivisionError`
   - C. `Division by zero is not allowed.`
   - D. `Error`
   - **Answer**: C

---

### 3. True or False: The `except` block will always run, even if there is no exception in the `try` block.
- A. True
- B. False
- **Answer**: B

---

### 4. What happens if an exception is not caught in a function?
- A. The program exits.
- B. The exception propagates to the caller.
- C. The exception is ignored.
- D. The function returns `None`.
- **Answer**: B

---

### 5. What is the correct order to place `except` clauses?
- A. From most specific to most general.
- B. From most general to most specific.
- C. It doesn't matter.
- D. Only one `except` clause is allowed.
- **Answer**: A

---

### 6. What does the following code output?
   ```python title="Example"
   def func():
       try:
           10 / 0
       except ZeroDivisionError:
           print("Caught ZeroDivisionError.")
           raise

   try:
       func()
   except ZeroDivisionError:
       print("Caught exception in the caller.")
   ```
   - A. `Caught ZeroDivisionError.`
   - B. `Caught exception in the caller.`
   - C. Both A and B
   - D. Error
   - **Answer**: C

---

### 7. True or False: Catching the base class `Exception` will catch all exceptions, including system-exit exceptions.
- A. True
- B. False
- **Answer**: B

---

### 8. Which of the following exceptions will NOT be caught by the following code?
   ```python title="Example"
   try:
       # Some code
   except Exception:
       pass
   ```
   - A. `KeyboardInterrupt`
   - B. `ZeroDivisionError`
   - C. `TypeError`
   - D. `ValueError`
   - **Answer**: A

---

### 9. What does the `raise` keyword do?
- A. It stops the program execution.
- B. It re-raises an exception.
- C. It raises a custom exception.
- D. Both B and C.
- **Answer**: D

---

### 10. What will the following code output?
   ```python title="Example"
   try:
       raise ValueError("Invalid value")
   except ValueError as e:
       print(e)
   ```
   - A. `None`
   - B. `Invalid value`
   - C. `Error`
   - D. `ValueError`
   - **Answer**: B

---

### 11. True or False: Specific exceptions should be placed after more general exceptions in `except` clauses.
- A. True
- B. False
- **Answer**: B

---

### 12. Which of the following is a valid way to catch multiple exceptions in one `except` clause?
- A. `except (ValueError, TypeError):`
- B. `except [ValueError, TypeError]:`
- C. `except {ValueError, TypeError}:`
- D. `except ValueError | TypeError:`
- **Answer**: A

---

### 13. What will the following code output?
   ```python title="Example"
   try:
       1 + '1'
   except TypeError:
       print("TypeError occurred.")
   except Exception:
       print("General exception occurred.")
   ```
   - A. `TypeError occurred.`
   - B. `General exception occurred.`
   - C. Both A and B
   - D. Error
   - **Answer**: A

---

### 14. What does exception propagation mean?
- A. Exceptions are handled immediately in the function where they occur.
- B. Exceptions are passed up the call stack until they are handled.
- C. Exceptions propagate to the operating system.
- D. Exceptions stop the program entirely.
- **Answer**: B

---

### 15. True or False: You must handle all exceptions in every function.
- A. True
- B. False
- **Answer**: B

---

### 16. What is the correct way to delegate responsibility for handling an exception to the calling code?
- A. Using `try-except` inside the function.
- B. Raising the exception using `raise`.
- C. Catching and suppressing the exception.
- D. Ignoring the exception.
- **Answer**: B

---

### 17. What will the following code output?
   ```python title="Example"
   def my_function():
       try:
           return 10 / 0
       except ZeroDivisionError:
           print("Handled in function.")
           raise

   try:
       my_function()
   except ZeroDivisionError:
       print("Handled by caller.")
   ```
   - A. `Handled in function.`
   - B. `Handled by caller.`
   - C. Both A and B.
   - D. Error
   - **Answer**: C

---

### 18. True or False: An exception raised inside a function will propagate up the call stack if not

 caught.
- A. True
- B. False
- **Answer**: A

---

### 19. Which keyword is used to handle exceptions in Python?
- A. `catch`
- B. `raise`
- C. `except`
- D. `throw`
- **Answer**: C

---

### 20. What will the following code output?
   ```python title="Example"
   try:
       print("Start")
       raise Exception("Something went wrong")
   except Exception as e:
       print(e)
   finally:
       print("End")
   ```
   - A. `Start`
   - B. `Something went wrong`
   - C. `End`
   - D. All of the above
   - **Answer**: D

---
