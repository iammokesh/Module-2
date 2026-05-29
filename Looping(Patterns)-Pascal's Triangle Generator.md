# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```python
import math

rows = int(input("Enter number of rows: "))

for n in range(rows):

    # Print spaces
    for space in range(rows - n - 1):
        print(" ", end="")

    # Print values
    for k in range(n + 1):

        value = math.factorial(n) // (
            math.factorial(k) * math.factorial(n - k)
        )

        print(value, end=" ")

    print()
```
## Sample Output
<img width="451" height="202" alt="WhatsApp Image 2026-05-29 at 6 56 02 PM" src="https://github.com/user-attachments/assets/9fcb3823-5867-4572-95c9-b6ddc125eb75" />


## Result
By using python the code executed successfully.

