
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

To include special characters like double quotes in strings, use the escape character "\".

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

You can convert between different data types with built-in functions: Converting to float: float() Converting to int: int() Converting to string: str()

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

Syntax errors occur when your code doesn't make sense to the computer. This can happen due to misspellings, an excess of brackets, or missing commas. 

```python
print(12 + 4))  # SyntaxError: unmatched ')'
```

### 18. Name Error

This occurs when there is a variable with a name that the computer does not recognize. This is typically due to a misspelling of a variable name you created earlier. Note: Variable names are case-sensitive.

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

This is the basic syntax for a function in Python. It allows you to assign a name to a set of instructions, enabling you to call it multiple times without the need to rewrite or copy-paste the code. The contents of the function must be indented to indicate that they are part of the function.

```python
def greet():
    print("Hello!")
```

### 21. Calling Functions

You activate a function by calling it. This is done by writing the name of the function followed by a set of parentheses. This allows you to determine when to execute the function and how many times it should be called.

```python
greet()  # Outputs: Hello!
```

### 22. Functions with Inputs

In addition to simple functions, you can provide inputs to the function. This allows the function to perform different actions each time it is called, depending on the provided input. This feature enhances the utility and reusability of your function.

```python
def add(n1, n2):
    return n1 + n2

result = add(2, 3)
print(result)  # Outputs: 5
```

### 23. Functions with Outputs

In addition to inputs, a function can also have an output. The output value is specified using the keyword "return." This allows you to store the result from a function for further use.

```python
def add(n1, n2):
    return n1 + n2
```

### 24. Variable Scope

Variables created inside a function are destroyed once the function has finished executing. The value of a variable is determined by its scope, which is defined by the location in the code where it is used. For example, if n is 2 outside the function but is assigned the value of 3 within my_function(), printing n inside the function will yield 3, whereas printing n outside the function will yield 2. This demonstrates how the scope of a variable affects its value.

```python
n = 2
def my_function():
    n = 3
    print(n)  # Outputs: 3

print(n)  # Outputs: 2
```

### 25. Keyword Arguments

When calling a function, you can provide either keyword arguments or positional values. Using keyword arguments allows you to specify the name of the parameter, which means you don’t have to follow the order of the parameters when providing the inputs. This can make your function calls clearer and more readable.

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

Sure! Here’s an enhanced version of the provided text, formatted to be more suitable for a GitHub page update, with improved clarity and structure:

---

## 37. `break` Keyword
The `break` keyword allows you to exit a loop prematurely. It can be used in both `for` and `while` loops. Here's an example:

```python
scores = [34, 67, 99, 105]
for s in scores:
    if s > 100:
        print("Invalid")
        break
    print(s)
```

## 38. `continue` Keyword
The `continue` keyword enables you to skip the current iteration of a loop and proceed to the next iteration. The loop itself continues executing:

```python
n = 0
while n < 100:
    n += 1
    if n % 2 == 0:
        continue
    print(n)  # Prints all odd numbers
```

## 39. Infinite Loops
An infinite loop occurs when the condition for continuing execution never becomes false. This is most commonly seen with `while` loops:

```python
while 5 > 1:
    print("I'm a survivor")  # DO NOT run; this creates an infinite loop
```

---

## List Methods

### 40. Adding Lists Together
You can concatenate lists using the `extend` method or the `+` operator:

```python
list1 = [1, 2, 3]
list2 = [9, 8, 7]
new_list = list1 + list2
list1 += list2
```

### 41. Adding an Item to a List
To add a single item to a list, use the `.append()` method:

```python
all_fruits = ["apple", "banana", "orange"]
all_fruits.append("pear")
```

### 42. List Indexing
Retrieve specific elements from a list using their index. Negative indexing allows you to count from the end:

```python
letters = ["a", "b", "c"]
print(letters[0])  # Result: "a"
print(letters[-1])  # Result: "c"
```

### 43. List Slicing
Using indices, you can slice lists to obtain specific portions:

```python
letters = ["a", "b", "c", "d"]
print(letters[1:3])  # Result: ["b", "c"]
```

---

## Built-in Functions

### 44. `range()`
Generate a sequence of numbers with specified start, end, and step values:

```python
for i in range(6, 0, -2):
    print(i)  # Result: 6, 4, 2 (0 is not included)
```

### 45. Randomization
The `random` module provides functions to generate random numbers. You'll need to import it first:

```python
import random
n = random.randint(2, 5)  # n can be 2, 3, 4, or 5
```

### 46. `round()`
Mathematically rounds numbers to the nearest integer:

```python
print(round(4.6))  # Result: 5
```

### 47. `abs()`
Returns the absolute value of a number, effectively removing negative signs:

```python
print(abs(-4.6))  # Result: 4.6
```

---

## Modules

### 48. Importing Modules
Some modules come pre-installed with Python, like `random` and `datetime`, while others can be installed from [PyPI](https://pypi.org):

```python
import random
n = random.randint(3, 10)
```

### 49. Aliasing Modules
You can rename a module while importing by using the `as` keyword:

```python
import random as r
n = r.randint(1, 5)
```

### 50. Importing Specific Attributes
Use the `from` keyword to import specific functions or classes from modules:

```python
from random import randint
n = randint(1, 5)
```

### 51. Importing Everything
Using a wildcard can import all attributes from a module, but this may reduce code readability:

```python
from random import *
list = [1, 2, 3]
print(choice(list))  # More readable: random.choice(list)
```

---

## Classes & Objects

### 52. Creating a Python Class
Define a class using the `class` keyword. Class names follow PascalCase conventions:

```python
class MyClass:
    # Define class properties and methods here
```

### 53. Creating an Object from a Class
You can create an instance of a class by invoking it with parentheses:

```python
class Car:
    pass

my_toyota = Car()
```

### 54. Class Methods
Define functions within a class, known as methods:

```python
class Car:
    def drive(self):
        print("Move")
        
my_honda = Car()
my_honda.drive()
```

### 55. Class Variables
Variables defined within a class are shared among all instances:

```python
class Car:
    colour = "black"

car1 = Car()
print(car1.colour)  # Result: black
```

### 56. The `__init__` Method
This special method is called when a new instance is created:

```python
class Car:
    def __init__(self):
        print("Building car")

my_toyota = Car()  # Output: Building car
```

### 57. Class Properties
Define variables within `__init__` for instance-specific attributes:

```python
class Car:
    def __init__(self, name):
        self.name = name

my_car = Car("Jimmy")
```

### 58. Class Inheritance
Create new classes that inherit properties and methods from existing classes:

```python
class Animal:
    def breathe(self):
        print("Breathing")

class Fish(Animal):
    def breathe(self):
        super().breathe()
        print("Underwater")

nemo = Fish()
nemo.breathe()
# Output:
# Breathing
# Underwater
```

---

### 59. Thank You!
We hope this guide helps you learn Python programming. Happy coding!

---

