# Day 14 - Prime Number Checker in Python

## 📌 Description
This Python program checks whether a given number is a prime number or not. A prime number is a number greater than 1 that is divisible only by 1 and itself.

The program uses an `if-else` statement, a `for` loop, and the modulo operator (`%`) to check whether the number has any divisors. It uses the square root of the number to make the checking process more efficient.

## 💻 Python Code
```python
n = int(input("Enter number: "))

if n < 2:
    print("Not Prime")
else:
    prime = True

    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            prime = False
            break

    print("Prime" if prime else "Not Prime")
```

## ▶️ Example Output

**Example 1:**
```text
Enter number: 7
Prime
```

**Example 2:**
```text
Enter number: 10
Not Prime
```

## 🧠 Concepts Learned
- User input using `input()`
- Type conversion using `int()`
- Conditional statements (`if-else`)
- `for` loops and `range()`
- Modulo operator (`%`)
- Boolean variables
- `break` statement
- Square root optimization

## 🎯 Learning Objective
To understand how to identify prime numbers using Python and improve efficiency by checking divisors only up to the square root of the given number.

## 🚀 Challenge
Modify the program to print all prime numbers between 1 and 100.

---
**100 Days of Python Challenge — Day 14 Completed!** ✅
