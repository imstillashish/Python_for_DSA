# Only Python needed to start DSA - Complete Notes
---
> *I hope it's easy to read and understand!*

**Credit**: [<span style="color: #007bffff;">Bro Code</span>](https://www.youtube.com/@BroCodez)

**Video Tutorial**: [<span style="color:#007bffff;">Python Tutorial for Beginners</span>](https://youtu.be/ix9cRaBkVe0)

---
<!-- Core Programming Fundamentals:
- #2 variables - #3 type casting - #6 arithmetic & math - #7 if statements - #11 logical operators - #12 conditional expressions - #16 while loops - #19 for loops - #20 nested loops - #31 functions - #32 default arguments - #33 keyword arguments - #34 args & kwargs* 
Data Structures:
- #13 string methods - #14 string indexing - #21 lists, sets, and tuples - #23 2D collections - #25 dictionaries - #35 iterables - #37 list comprehensions 
Important Concepts:
- #36 membership operators - #38 match-case statements - #40 scope resolution - #51 polymorphism - #58 exception handling 
Useful but Secondary:
- #27 random numbers (for testing/generating test cases) - #39 modules (for organizing code) - #46 Python object-oriented programming (for advanced DSA implementations) - #48 inheritance (for advanced data structure implementations) -->

# Table of Contents

1. [Python Tutorial for Beginners 🐍](#1-python-tutorial-for-beginners-)  
2. [Variables ❎](#2-variables-)  
3. [Type Casting 💱](#3-type-casting-)  
4. [User Input ⌨️](#4-user-input-%EF%B8%8F)  
5. [Arithmetic & Math 📐](#5-arithmetic--math-)  
6. [If Statements 🤔](#6-if-statements-)  
7. [Logical Operators 🌦️](#7-logical-operators-%EF%B8%8F)  
8. [Conditional Expressions ❓](#8-conditional-expressions-%EF%B8%8F)  
9. [String Methods 〰️](#9-string-methods-%EF%B8%8F)  
10. [String Indexing ✂️](#10-string-indexing-%EF%B8%8F)  
11. [Format Specifiers 💬](#11-format-specifiers-)  
12. [While Loops ♾️](#12-while-loops-%EF%B8%8F)  
13. [For Loops 🔁](#13-for-loops-)  
14. [Nested Loops ➿](#14-nested-loops-)  
15. [Lists, Sets, and Tuples 🍎](#15-lists-sets-and-tuples-)  
16. [2D Collections ⬜](#16-2d-collections-)  
17. [Dictionaries 📙](#17-dictionaries-)  
18. [Random Numbers 🎲](#18-random-numbers-)  
19. [Functions 📞](#19-functions-)  
20. [Default Arguments 👍](#20-default-arguments-)  
21. [Keyword Arguments 🗝️](#21-keyword-arguments-%EF%B8%8F)  
22. [*args & **kwargs 📦](#22-args--kwargs-)  
23. [Iterables 🔂](#23-iterables-)  
24. [Membership Operators 🔎](#24-membership-operators-)  
25. [List Comprehensions 📃](#25-list-comprehensions-)  
26. [Match-Case Statements 📆](#26-match-case-statements-)  
27. [Modules 📨](#27-modules-)
28. [Scope Resolution 🔬](#28-scope-resolution-)  
29. [if __name__ == '__main__': 📥](#29-if-name--main-)  
30. [Python Object-Oriented Programming 🚗](#30-python-object-oriented-programming-)  
31. [Class Variables 🎓](#31-class-variables-)  
32. [Inheritance 👨‍👦‍👦](#32-inheritance-)  
33. [Polymorphism 🎭](#33-polymorphism-)  
34. [Exception Handling 🚦](#34-exception-handling-)

---
## 1. Python Tutorial for Beginners 🐍
**Core Concepts:**
- Python is an interpreted, high-level programming language
- Known for readability and simplicity
- Uses indentation for code blocks (not braces)
- Case-sensitive language
- File extension: `.py`

**Key Points:**
- Install Python from python.org
- Use IDE/editor (VS Code, PyCharm, IDLE)
- Run programs: `python filename.py`
- Interactive mode: type `python` in terminal
- Comments: `#` for single line, `'''` or `"""` for multi-line

**Bullet Points to Remember:**
- Python emphasizes code readability and simplicity
- Indentation is mandatory and defines code structure
- Python is interpreted, not compiled
- Case sensitivity matters (Name ≠ name)

---
## 2. Variables ❎
**Definition:** Named storage locations for data

**Rules:**
- Start with letter or underscore
- Can contain letters, numbers, underscores
- Case-sensitive (age ≠ Age)
- No spaces or special characters
- Can't use Python keywords

**Examples:**
```python
name = "John"          # String
age = 25              # Integer
height = 5.9          # Float
is_student = True     # Boolean
```

**Best Practices:**
- Use descriptive names
- Use snake_case for variables
- Constants in UPPERCASE

**Bullet Points to Remember:**
- Variables are containers that store data values
- No need to declare variable type (dynamically typed)
- Variable names should be descriptive and meaningful
- Use snake_case convention for readability

---
## 3. Type Casting 💱
**Definition:** Converting one data type to another

**Common Conversions:**
```python
# String to Integer
age = int("25")

# Integer to String
age_str = str(25)

# String to Float
price = float("19.99")

# Integer to Float
decimal = float(10)

# Boolean conversions
bool(1)    # True
bool(0)    # False
bool("")   # False
bool("Hi") # True
```

**Important Notes:**
- Invalid conversions raise ValueError
- Loss of precision when converting float to int
- Empty strings/0/None convert to False

**Bullet Points to Remember:**
- Type casting allows conversion between data types
- int() truncates decimal part, doesn't round
- Always handle potential ValueError exceptions
- Empty values generally convert to False in boolean context

---
## 4. User Input ⌨️
**Basic Syntax:**
```python
name = input("Enter your name: ")  # Always returns string
age = int(input("Enter age: "))    # Convert to integer
```

**Key Points:**
- `input()` always returns a string
- Must convert for numerical operations
- Program pauses until user provides input
- Can include prompt message

**Bullet Points to Remember:**
- input() function always returns string type
- Convert input to appropriate type for calculations
- Always validate user input when possible
- Include clear prompts for better user experience

---
## 5. Arithmetic & Math 📐
**Basic Operators:**
```python
+   # Addition
-   # Subtraction
*   # Multiplication
/   # Division (float result)
//  # Floor division
%   # Modulus (remainder)
**  # Exponentiation
```

**Math Module:**
```python
import math

math.sqrt(16)      # Square root
math.ceil(4.3)     # Round up
math.floor(4.7)    # Round down
math.pi            # Pi constant
math.pow(2, 3)     # Power
abs(-5)            # Absolute value (built-in)
round(3.7)         # Round (built-in)
```

**Order of Operations:** PEMDAS
1. Parentheses
2. Exponents
3. Multiplication/Division (left to right)
4. Addition/Subtraction (left to right)

**Bullet Points to Remember:**
- / always returns float, // returns integer division
- % operator gives remainder, useful for even/odd checks
- Import math module for advanced mathematical functions
- PEMDAS rules apply, use parentheses for clarity

---
## 6. If Statements 🤔
**Basic Structure:**
```python
if condition:
    # code block
elif another_condition:
    # code block
else:
    # code block
```

**Comparison Operators:**
```python
==  # Equal to
!=  # Not equal to
>   # Greater than
<   # Less than
>=  # Greater than or equal
<=  # Less than or equal
```

**Examples:**
```python
age = 18
if age >= 18:
    print("Adult")
elif age >= 13:
    print("Teenager")
else:
    print("Child")
```

**Bullet Points to Remember:**
- Use == for equality comparison, = for assignment
- elif allows multiple conditions to be checked
- else is optional and catches all remaining cases
- Indentation is crucial for code block definition

---
## 7. Logical Operators 🌦️
**Operators:**
- `and`: Both conditions must be True
- `or`: At least one condition must be True
- `not`: Inverts the boolean value

**Truth Tables:**
```python
# AND
True and True   # True
True and False  # False
False and False # False

# OR
True or False   # True
False or False  # False

# NOT
not True        # False
not False       # True
```

**Example:**
```python
age = 25
has_license = True

if age >= 18 and has_license:
    print("Can drive")
```

**Bullet Points to Remember:**
- 'and' requires all conditions to be True
- 'or' requires at least one condition to be True
- 'not' flips the boolean value
- Use parentheses to group complex logical expressions

---
## 8. Conditional Expressions ❓
**Ternary Operator:**
```python
# Syntax: value_if_true if condition else value_if_false
age = 20
status = "Adult" if age >= 18 else "Minor"

# Equivalent to:
if age >= 18:
    status = "Adult"
else:
    status = "Minor"
```

**Nested Conditional:**
```python
score = 85
grade = "A" if score >= 90 else "B" if score >= 80 else "C"
```

**Bullet Points to Remember:**
- Ternary operator is shorthand for simple if-else
- Keep ternary expressions simple for readability
- Nested ternaries can become hard to read
- Use regular if-else for complex logic

---
## 9. String Methods 〰️
**Common Methods:**
```python
text = "Hello World"

text.upper()          # "HELLO WORLD"
text.lower()          # "hello world"
text.capitalize()     # "Hello world"
text.title()          # "Hello World"
text.strip()          # Remove whitespace
text.replace("o", "0") # "Hell0 W0rld"
text.split()          # ["Hello", "World"]
text.find("World")    # 6 (index)
text.count("l")       # 3
text.startswith("He") # True
text.endswith("ld")   # True
text.isalpha()        # False (has space)
text.isdigit()        # False
len(text)             # 11 (built-in function)
```

**Bullet Points to Remember:**
- String methods don't modify original string (immutable)
- Use strip() to remove unwanted whitespace
- find() returns -1 if substring not found
- isdigit() and isalpha() useful for input validation

---
## 10. String Indexing ✂️
**Concepts:**
```python
text = "Python"
# Indices: 0  1  2  3  4  5
#          P  y  t  h  o  n
# Negative:-6 -5 -4 -3 -2 -1

# Accessing characters
first = text[0]       # 'P'
last = text[-1]       # 'n'

# Slicing [start:end:step]
text[0:3]    # "Pyt" (end exclusive)
text[2:]     # "thon"
text[:4]     # "Pyth"
text[::2]    # "Pto" (every 2nd char)
text[::-1]   # "nohtyP" (reverse)
```

**Bullet Points to Remember:**
- String indexing starts at 0
- Negative indices count from the end
- Slicing end index is exclusive
- [::-1] is common way to reverse strings

---
## 11. Format Specifiers 💬
**Methods:**
```python
name = "Alice"
age = 25
height = 5.7

# f-strings (Python 3.6+)
print(f"Name: {name}, Age: {age}")

# .format() method
print("Name: {}, Age: {}".format(name, age))

# % formatting (older)
print("Name: %s, Age: %d" % (name, age))

# Format specifiers
price = 19.99
print(f"Price: ${price:.2f}")      # 2 decimal places
print(f"Binary: {10:b}")            # Binary
print(f"Hex: {255:x}")              # Hexadecimal
print(f"Percentage: {0.25:.1%}")    # 25.0%
print(f"Padded: {5:03d}")           # 005
```

**Bullet Points to Remember:**
- f-strings are the modern, preferred method
- :.2f formats to 2 decimal places
- Format specifiers control number display
- f-strings are more readable and faster

---
## 12. While Loops ♾️
**Structure:**
```python
while condition:
    # code block
    # update condition

# Example
count = 0
while count < 5:
    print(count)
    count += 1

# Infinite loop with break
while True:
    user_input = input("Enter 'quit' to exit: ")
    if user_input == 'quit':
        break
```

**Control Statements:**
- `break`: Exit loop immediately
- `continue`: Skip to next iteration
- `else`: Executes if loop completes normally

**Bullet Points to Remember:**
- Always ensure the condition will eventually become False
- Use break to exit loops based on user input
- continue skips current iteration, doesn't exit loop
- Avoid infinite loops unless intentional

---
## 13. For Loops 🔁
**Syntax:**
```python
# Iterate over sequence
for item in sequence:
    # code block

# Range function
for i in range(5):        # 0 to 4
    print(i)

for i in range(1, 6):     # 1 to 5
    print(i)

for i in range(0, 10, 2): # 0, 2, 4, 6, 8
    print(i)

# Iterate over string
for char in "Python":
    print(char)

# Enumerate
fruits = ["apple", "banana", "orange"]
for index, fruit in enumerate(fruits):
    print(f"{index}: {fruit}")
```

**Bullet Points to Remember:**
- for loops iterate over sequences automatically
- range(stop) starts at 0, range(start, stop, step)
- enumerate() provides both index and value
- More pythonic than while loops for known iterations

---
## 14. Nested Loops ➿
**Concept:**
```python
# Multiplication table
for i in range(1, 4):
    for j in range(1, 4):
        print(f"{i} x {j} = {i*j}")
    print()  # New line after each row

# Pattern printing
rows = 5
for i in range(rows):
    for j in range(i + 1):
        print("*", end="")
    print()
```

**Bullet Points to Remember:**
- Inner loop completes fully for each outer loop iteration
- Useful for 2D data structures and patterns
- Can impact performance with large datasets
- Break and continue affect the immediate containing loop

---
## 15. Lists, Sets, and Tuples 🍎
**Lists (Mutable, Ordered):**
```python
fruits = ["apple", "banana", "orange"]
fruits.append("grape")      # Add to end
fruits.insert(1, "mango")   # Insert at index
fruits.remove("banana")     # Remove by value
fruits.pop()               # Remove last item
fruits.pop(0)              # Remove at index
fruits.sort()              # Sort in place
fruits.reverse()           # Reverse in place
fruits.clear()             # Remove all items
```

**Tuples (Immutable, Ordered):**
```python
coordinates = (10, 20)
x, y = coordinates  # Unpacking
# coordinates[0] = 15  # Error! Immutable
```

**Sets (Mutable, Unordered, No Duplicates):**
```python
numbers = {1, 2, 3, 3}  # {1, 2, 3}
numbers.add(4)
numbers.remove(2)
numbers.discard(5)  # No error if not exists

# Set operations
set1 = {1, 2, 3}
set2 = {3, 4, 5}
set1.union(set2)        # {1, 2, 3, 4, 5}
set1.intersection(set2) # {3}
set1.difference(set2)   # {1, 2}
```

**Bullet Points to Remember:**
- Lists are ordered and mutable, use for sequences
- Tuples are ordered and immutable, use for fixed data
- Sets are unordered and unique, use for membership testing
- Choose the right data structure for your needs

---
## 16. 2D Collections ⬜
**2D Lists:**
```python
# Matrix
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

# Accessing elements
matrix[0][0]  # 1
matrix[1][2]  # 6

# Iterating
for row in matrix:
    for element in row:
        print(element, end=" ")
    print()

# List comprehension for 2D
grid = [[0 for _ in range(3)] for _ in range(3)]
```

**Bullet Points to Remember:**
- Use [row][column] indexing for 2D lists
- Nested loops required for full traversal
- List comprehension can create 2D structures
- Useful for grids, matrices, and game boards

---
## 17. Dictionaries 📙
**Basic Operations:**
```python
# Creating dictionaries
student = {"name": "Alice", "age": 20, "grade": "A"}
student = dict(name="Alice", age=20, grade="A")

# Accessing values
print(student["name"])      # Alice
print(student.get("age"))   # 20
print(student.get("height", "Unknown"))  # Unknown (default)

# Modifying
student["age"] = 21         # Update
student["city"] = "NYC"     # Add new key

# Dictionary methods
student.keys()              # dict_keys(['name', 'age', 'grade'])
student.values()            # dict_values(['Alice', 21, 'A'])
student.items()             # key-value pairs

# Iteration
for key in student:
    print(f"{key}: {student[key]}")

for key, value in student.items():
    print(f"{key}: {value}")
```

**Bullet Points to Remember:**
- Dictionaries store key-value pairs
- Keys must be immutable (strings, numbers, tuples)
- Use .get() to avoid KeyError for missing keys
- items() returns key-value pairs for iteration

---
## 18. Random Numbers 🎲
**Random Module:**
```python
import random

# Random integer
random.randint(1, 6)        # 1 to 6 inclusive
random.randrange(1, 11)     # 1 to 10 (11 exclusive)

# Random float
random.random()             # 0.0 to 1.0
random.uniform(1.5, 10.5)   # Between 1.5 and 10.5

# Random choice
colors = ["red", "blue", "green"]
random.choice(colors)

# Shuffle list
random.shuffle(colors)      # Modifies original list

# Multiple choices
random.choices(colors, k=3) # With replacement
random.sample(colors, 2)    # Without replacement
```

**Bullet Points to Remember:**
- Always import random module first
- randint() is inclusive on both ends
- randrange() excludes the stop value
- choice() picks one item, choices() picks multiple
- shuffle() modifies the original list

---
## 19. Functions 📞
**Basic Syntax:**
```python
def function_name(parameters):
    """Optional docstring"""
    # function body
    return value  # optional

# Examples
def greet(name):
    return f"Hello, {name}!"

def add_numbers(a, b):
    return a + b

def print_info(name, age):
    print(f"Name: {name}, Age: {age}")

# Function call
result = add_numbers(5, 3)
print_info("Alice", 25)
```

**Bullet Points to Remember:**
- Use def keyword to define functions
- Parameters are variables that receive arguments
- return statement sends value back to caller
- Functions promote code reusability
- Use descriptive function names

---
## 20. Default Arguments 👍
**Syntax:**
```python
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

def calculate_area(length, width=None):
    if width is None:
        return length ** 2  # Square
    return length * width   # Rectangle

# Usage
print(greet("Alice"))           # Uses default greeting
print(greet("Bob", "Hi"))       # Custom greeting
print(calculate_area(5))        # Square: 25
print(calculate_area(4, 6))     # Rectangle: 24
```

**Bullet Points to Remember:**
- Default parameters must come after non-default ones
- Use None for mutable default arguments
- Allows function overloading-like behavior
- Makes functions more flexible

---
## 21. Keyword Arguments 🗝️
**Syntax:**
```python
def create_profile(name, age, city="Unknown", country="Unknown"):
    return f"{name}, {age} from {city}, {country}"

# Positional arguments
print(create_profile("Alice", 25, "NYC", "USA"))

# Keyword arguments
print(create_profile(name="Bob", age=30, country="Canada"))
print(create_profile("Charlie", age=35, city="London"))

# Mixed (positional first, then keyword)
print(create_profile("Diana", 28, country="Australia"))
```

**Bullet Points to Remember:**
- Keyword arguments can be in any order
- More readable and self-documenting
- Positional args must come before keyword args
- Useful for functions with many parameters

---
## 22. *args & **kwargs 📦
**Variable Arguments:**
```python
def sum_all(*args):
    """Accept any number of positional arguments"""
    return sum(args)

def print_info(**kwargs):
    """Accept any number of keyword arguments"""
    for key, value in kwargs.items():
        print(f"{key}: {value}")

def full_function(name, *args, **kwargs):
    print(f"Name: {name}")
    print(f"Args: {args}")
    print(f"Kwargs: {kwargs}")

# Usage
print(sum_all(1, 2, 3, 4, 5))  # 15
print_info(name="Alice", age=25, city="NYC")
full_function("Bob", 1, 2, 3, age=30, city="LA")
```

**Bullet Points to Remember:**
- *args collects extra positional arguments into tuple
- **kwargs collects extra keyword arguments into dict
- Order: positional, *args, keyword, **kwargs
- Useful for wrapper functions and APIs

---
## 23. Iterables 🔂
**Definition and Usage:**
```python
# Iterables: objects that can be looped over
numbers = [1, 2, 3, 4, 5]
text = "Python"
my_dict = {"a": 1, "b": 2}

# iter() and next()
iterator = iter(numbers)
print(next(iterator))  # 1
print(next(iterator))  # 2

# Custom iterable
class Countdown:
    def __init__(self, start):
        self.start = start
    
    def __iter__(self):
        return self
    
    def __next__(self):
        if self.start <= 0:
            raise StopIteration
        self.start -= 1
        return self.start + 1

# Usage
for num in Countdown(3):
    print(num)  # 3, 2, 1
```

**Bullet Points to Remember:**
- Iterables can be used in for loops
- iter() creates iterator from iterable
- next() gets next item from iterator
- StopIteration exception ends iteration
- Lists, strings, dicts are built-in iterables

---
## 24. Membership Operators 🔎
**Operators:**
```python
# 'in' operator
fruits = ["apple", "banana", "orange"]
print("apple" in fruits)        # True
print("grape" in fruits)        # False

# 'not in' operator
print("grape" not in fruits)    # True

# With strings
text = "Hello World"
print("World" in text)          # True
print("world" in text)          # False (case sensitive)

# With dictionaries (checks keys)
student = {"name": "Alice", "age": 20}
print("name" in student)        # True
print("grade" in student)       # False

# With ranges
print(5 in range(1, 10))        # True
print(15 in range(1, 10))       # False
```

**Bullet Points to Remember:**
- 'in' checks if item exists in sequence
- 'not in' is the opposite of 'in'
- Case-sensitive for strings
- For dicts, checks keys by default
- Works with any iterable object

---
## 25. List Comprehensions 📃
**Syntax:**
```python
# Basic syntax: [expression for item in iterable]
squares = [x**2 for x in range(1, 6)]  # [1, 4, 9, 16, 25]

# With condition: [expression for item in iterable if condition]
evens = [x for x in range(1, 11) if x % 2 == 0]  # [2, 4, 6, 8, 10]

# With string manipulation
words = ["hello", "world", "python"]
upper_words = [word.upper() for word in words]

# Nested comprehensions
matrix = [[j for j in range(3)] for i in range(3)]

# Dictionary comprehension
squares_dict = {x: x**2 for x in range(1, 6)}

# Set comprehension
unique_lengths = {len(word) for word in words}
```

**Bullet Points to Remember:**
- More concise than traditional loops
- Creates new list, doesn't modify original
- Can include conditions for filtering
- Works with dictionaries and sets too
- Don't overuse - readability matters

---
## 26. Match-Case Statements 📆
**Syntax (Python 3.10+):**
```python
def handle_response(status):
    match status:
        case 200:
            return "Success"
        case 404:
            return "Not Found"
        case 500:
            return "Server Error"
        case _:  # Default case
            return "Unknown Status"

# Pattern matching with values
def describe_animal(animal):
    match animal:
        case "dog" | "cat":
            return "Domestic pet"
        case "lion" | "tiger":
            return "Wild cat"
        case _:
            return "Unknown animal"

# With conditions
def categorize_number(x):
    match x:
        case n if n < 0:
            return "Negative"
        case 0:
            return "Zero"
        case n if n > 0:
            return "Positive"
```

**Bullet Points to Remember:**
- Python 3.10+ feature (alternative to if-elif)
- Use _ for default case (wildcard)
- Can match multiple values with |
- Supports pattern matching and guards
- More powerful than traditional switch statements

---
## 27. Modules 📨
**Creating and Using Modules:**
```python
# math_operations.py (custom module)
def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

PI = 3.14159

# main.py
import math_operations
from math_operations import add, PI
import math_operations as math_ops

# Usage
result1 = math_operations.add(5, 3)
result2 = add(5, 3)  # Direct import
result3 = math_ops.multiply(4, 7)

# Built-in modules
import math, random, datetime
import os, sys
```

**Bullet Points to Remember:**
- Modules are .py files containing code
- import brings entire module
- from...import brings specific items
- Use 'as' for aliases
- Python has many built-in modules

---
## 28. Scope Resolution 🔬
**LEGB Rule:**
```python
x = "global"  # Global scope

def outer():
    x = "enclosing"  # Enclosing scope
    
    def inner():
        x = "local"  # Local scope
        print(f"Inner: {x}")
    
    inner()
    print(f"Outer: {x}")

outer()
print(f"Global: {x}")

# global and nonlocal keywords
count = 0

def increment():
    global count
    count += 1

def outer_func():
    x = 10
    
    def inner_func():
        nonlocal x
        x += 1
    
    inner_func()
    return x
```

**Bullet Points to Remember:**
- LEGB: Local → Enclosing → Global → Built-in
- Use 'global' to modify global variables
- Use 'nonlocal' to modify enclosing scope variables
- Variables are searched in LEGB order
- Avoid global variables when possible

---
## 29. if __name__ == '__main__': 📥
**Purpose and Usage:**
```python
# utilities.py
def helper_function():
    return "This is a helper function"

def main():
    print("Running utilities.py directly")
    print(helper_function())

if __name__ == "__main__":
    main()

# main_program.py
import utilities

# This will import utilities but won't run main()
result = utilities.helper_function()
print(result)
```

**Bullet Points to Remember:**
- Allows modules to be both imported and run directly
- Code under if __name__ == "__main__": only runs when script is executed directly
- Prevents code from running during imports
- Good practice for all Python modules
- Enables module testing

---
## 30. Python Object-Oriented Programming 🚗
**Classes and Objects:**
```python
class Car:
    def __init__(self, make, model, year, color):
        self.make = make
        self.model = model
        self.year = year
        self.color = color
        self.odometer = 0
    
    def drive(self, distance):
        if distance >= 0:
            self.odometer += distance
        else:
            print("Distance cannot be negative")
    
    def get_info(self):
        return f"{self.year} {self.make} {self.model} ({self.color})"

# Creating objects
car1 = Car("Toyota", "Camry", 2022, "Blue")
car2 = Car("Honda", "Civic", 2021, "Red")

# Using methods
print(car1.get_info())
car1.drive(100)
print(f"Odometer: {car1.odometer}")
```

**Bullet Points to Remember:**
- Classes are blueprints for creating objects
- __init__ method initializes object attributes
- self refers to the current instance
- Methods are functions defined inside classes
- Objects are instances of classes

---
## 31. Class Variables 🎓
**Class vs Instance Variables:**
```python
class Student:
    school_name = "Python University"  # Class variable
    num_students = 0                   # Class variable
    
    def __init__(self, name, age):
        self.name = name               # Instance variable
        self.age = age                 # Instance variable
        Student.num_students += 1      # Access class variable
    
    @classmethod
    def get_school_name(cls):
        return cls.school_name
    
    @classmethod
    def get_num_students(cls):
        return cls.num_students

# Usage
student1 = Student("Alice", 20)
student2 = Student("Bob", 21)

print(Student.school_name)        # Class variable
print(student1.name)              # Instance variable
print(Student.get_num_students()) # 2
```

**Bullet Points to Remember:**
- Class variables are shared by all instances
- Instance variables are unique to each object
- Use ClassName.variable to access class variables
- @classmethod decorator for class methods
- cls parameter refers to the class itself

---
## 32. Inheritance 👨‍👦‍👦
**Parent and Child Classes:**
```python
class Animal:
    def __init__(self, name):
        self.name = name
        self.is_alive = True
    
    def eat(self):
        print(f"{self.name} is eating")
    
    def sleep(self):
        print(f"{self.name} is sleeping")

class Dog(Animal):  # Dog inherits from Animal
    def __init__(self, name, breed):
        super().__init__(name)  # Call parent constructor
        self.breed = breed
    
    def bark(self):
        print(f"{self.name} is barking")

class Cat(Animal):
    def __init__(self, name, indoor):
        super().__init__(name)
        self.indoor = indoor
    
    def meow(self):
        print(f"{self.name} is meowing")

# Usage
dog = Dog("Buddy", "Golden Retriever")
cat = Cat("Whiskers", True)

dog.eat()   # Inherited method
dog.bark()  # Child method
cat.sleep() # Inherited method
cat.meow()  # Child method
```

**Bullet Points to Remember:**
- Child classes inherit attributes and methods from parent
- Use super() to call parent class methods
- Child classes can override parent methods
- Child classes can add their own methods
- Promotes code reusability
---
## 33. Polymorphism 🎭
**Same Interface, Different Implementation:**
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass
    
    @abstractmethod
    def perimeter(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    
    def area(self):
        return 3.14159 * self.radius ** 2
    
    def perimeter(self):
        return 2 * 3.14159 * self.radius

class Square(Shape):
    def __init__(self, side):
        self.side = side
    
    def area(self):
        return self.side ** 2
    
    def perimeter(self):
        return 4 * self.side

class Triangle(Shape):
    def __init__(self, a, b, c):
        self.a = a
        self.b = b
        self.c = c
    
    def area(self):
        s = (self.a + self.b + self.c) / 2
        return (s * (s - self.a) * (s - self.b) * (s - self.c)) ** 0.5
    
    def perimeter(self):
        return self.a + self.b + self.c

# Polymorphism in action
shapes = [Circle(5), Square(4), Triangle(3, 4, 5)]

for shape in shapes:
    print(f"Area: {shape.area():.2f}")
    print(f"Perimeter: {shape.perimeter():.2f}")
    print("-" * 20)
```

**Bullet Points to Remember:**
- Same method name, different implementations
- Abstract base classes define common interface
- Enables treating different objects uniformly
- @abstractmethod forces implementation in child classes
- Powerful for building flexible systems

---
## 34. Exception Handling 🚦
**Try, Except, Else, Finally:**
```python
# Basic exception handling
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print(f"Result: {result}")
except ValueError:
    print("Invalid input! Please enter a number.")
except ZeroDivisionError:
    print("Cannot divide by zero!")
except Exception as e:
    print(f"An unexpected error occurred: {e}")
else:
    print("No exceptions occurred!")
finally:
    print("This always executes")

# Custom exceptions
class CustomError(Exception):
    def __init__(self, message):
        self.message = message
        super().__init__(self.message)

def validate_age(age):
    if age < 0:
        raise CustomError("Age cannot be negative")
    elif age > 150:
        raise CustomError("Age seems unrealistic")
    return True

# Raising exceptions
try:
    age = int(input("Enter your age: "))
    validate_age(age)
    print(f"Age {age} is valid")
except CustomError as e:
    print(f"Validation error: {e}")
except ValueError:
    print("Please enter a valid number")
```

**Bullet Points to Remember:**
- Use try-except to handle potential errors gracefully
- Specific exceptions should be caught before general ones
- else block runs only if no exceptions occur
- finally block always executes (cleanup code)
- Create custom exceptions by inheriting from Exception