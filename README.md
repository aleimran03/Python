
# Python Basics

Welcome to the Python Basics guide! This document is designed to help beginners understand the foundational concepts of Python programming through clear examples and explanations. Whether you're getting started or brushing up on skills, this guide can serve as a helpful reference.

## 1. Printing Strings

To display content in the console, you can use the `print()` function.

```python
print("Hello, World!")
```

## 2. User Input

You can prompt the user for input using the `input()` function.

```python
name = input("What's your name?")
print(f"Hello, {name}!")
```

## 3. Comments

Comments are important for documenting your code. You can add comments by using the `#` symbol. The interpreter ignores anything after this symbol on the same line.

```python
# This is a comment
print("This is code")  # This prints text to the console
```

## 4. Variables

Variables allow you to store data with a name, making it easier to manage.

```python
my_name = "Angela"
my_age = 12
```

## 5. The `+=` Operator

The `+=` operator is a shorthand for updating the value of a variable.

```python
my_age += 4  # my_age is now 16
```

## Data Types

Understanding data types is crucial in Python programming.

### 6. Integers

Integers are whole numbers:

```python
my_number = 354
```

### 7. Floating Point Numbers

Floats are numbers with decimals. Any division that results in a fractional number will yield a float.

```python
my_float = 3.14159
```

### 8. Strings

A string is a sequence of characters, enclosed in quotes.

```python
my_string = "Hello"
```

### 9. String Concatenation

Strings can be combined using the `+` operator, creating a new string.

```python
greeting = "Hello" + " Angela"  # Results in "Hello Angela"
```

### 10. Escaping Strings

To include special characters like double quotes in strings, use the escape character `\`.

```python
speech = "She said: \"Hi\""
print(speech)  # Outputs: She said: "Hi"
```

### 11. F-Strings

Format strings (f-strings) allow you to embed variable values directly into strings.

```python
days = 365
print(f"There are {days} days in a year")
```

### 12. Converting Data Types

You can convert between different data types with built-in functions:

```python
n = 354
new_n = float(n)  # Converts to a float
print(new_n)  # Outputs: 354.0
```

### 13. Checking Data Types

Use the `type()` function to check variable data types.

```python
n = 3.14159
print(type(n))  # Outputs: <class 'float'>
```

## Math Operations

### 14. Arithmetic Operators

Python supports basic arithmetic operations:

```python
3 + 2  # Addition
4 - 1  # Subtraction
2 * 3  # Multiplication
5 / 2  # Division
5 ** 2  # Exponentiation
```

### 15. The `+=` Operator Revisited

The `+=` operator can be used with any arithmetic operation.

```python
my_number = 4
my_number += 2  # Result is now 6
```

### 16. The Modulo Operator

The modulo operator `%` returns the remainder of a division.

```python
remainder = 5 % 2  # Result is 1
```

## Errors

### 17. Syntax Error

A syntax error occurs when the code is not valid Python syntax.

```python
print(12 + 4))  # SyntaxError: unmatched ')'
```

### 18. Name Error

This occurs when you try to use a variable that hasn't been defined.

```python
my_number = 4
print(my_Number)  # NameError: name 'my_Number' is not defined
```

### 19. Zero Division Error

Attempting to divide by zero will cause an error:

```python
result = 5 / 0  # ZeroDivisionError
```

## Functions

### 20. Creating Functions

Define a function to group statements that can be executed multiple times.

```python
def greet():
    print("Hello!")
```

### 21. Calling Functions

To run a function, simply call it by name.

```python
greet()  # Outputs: Hello!
```

### 22. Functions with Inputs

Functions can accept parameters to make them more dynamic.

```python
def add(n1, n2):
    return n1 + n2

result = add(2, 3)
print(result)  # Outputs: 5
```

### 23. Functions with Outputs

You can return a value from a function using the `return` statement.

```python
def add(n1, n2):
    return n1 + n2
```

### 24. Variable Scope

Variables defined inside a function are not accessible outside.

```python
n = 2
def my_function():
    n = 3
    print(n)  # Outputs: 3

print(n)  # Outputs: 2
```

### 25. Keyword Arguments

You can call a function using keyword arguments for flexibility in parameter order.

```python
def divide(n1, n2):
    return n1 / n2

divide(n2=5, n1=10)  # Outputs: 2.0
```

## Conditions

### 27. If Statements

An `if` statement checks for a condition.

```python
n = 5
if n > 2:
    print("Larger than 2")
```

### 28. Else Statements

Add an `else` statement for an alternative branch.

```python
age = 18
if age > 16:
    print("Can drive")
else:
    print("Don't drive")
```

### 29. Elif Statements

Use `elif` to check additional conditions after an `if`.

```python
weather = "sunny"
if weather == "rain":
    print("Bring an umbrella")
elif weather == "sunny":
    print("Bring sunglasses")
```

### 30. Logical Operators

Use `and`, `or`, and `not` to combine or negate conditions.

```python
s = 58
if s < 60 and s > 50:
    print("Your grade is C")
```

## Loops

### 34. While Loop

This loop continues while a condition is true.

```python
n = 1
while n < 100:
    n += 1
```

### 35. For Loop

For loops iterate over sequences like lists or ranges.

```python
all_fruits = ["apple", "banana", "orange"]
for fruit in all_fruits:
    print(fruit)
```

### 36. Using `_` in Loops

When the value isn't needed, you can use `_` to indicate it.

```python
for _ in range(100):
    # Do something 100 times.
```

### 37. Break and Continue

Use `break` to exit a loop, and `continue` to skip to the next iteration.

```python
scores = [34, 67, 99, 105]
for s in scores:
    if s > 100:
        print("Invalid score")
        break
```

### Infinite Loops

Be cautious with loops that never terminate:

```python
while True:
    print("I'm a survivor")  # DO NOT run; it's an infinite loop
```

---

We hope you find this guide useful! Happy coding!

--- 

Feel free to adjust any sections or examples to better fit your style or the intended audience!
