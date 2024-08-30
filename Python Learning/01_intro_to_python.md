### Python Introductory Lesson

Welcome to your introduction to Python! In this lesson, we will cover essential programming concepts using Python, including values and data types, variables, operators, and more. These are the building blocks that will help you write basic Python programs.

### 1. Values & Data Types

In Python, **values** are the fundamental units of data. Every value has a **type**, which defines what operations can be performed on it.

**Basic Data Types**:
- **Integers** (`int`): Whole numbers, e.g., `5`, `100`
- **Floating-point numbers** (`float`): Numbers with decimals, e.g., `3.14`, `9.81`
- **Strings** (`str`): Sequences of characters, e.g., `"Hello"`, `"Python3"`, `"The toy costs $1.50!"`
- **Booleans** (`bool`): Logical values `True` or `False`
- **NoneType** (`None`): Unique type for `None` value, used to indicate absence of data

#### Example:
```python
x = 42              # Integer
pi = 3.14159        # Float
message = "Hi"      # String
is_active = True    # Boolean
missing_data = None # NoneType
```

### 2. Type Conversion Functions

Python allows you to convert data from one type to another using **type conversion functions**.

- `int()`: Converts to integer (rounds floats down)
- `float()`: Converts to float
- `str()`: Converts to string
- `bool()`: Converts to boolean*

_*Note: `bool()` treats emptiness as False (eg `0`, `0.0`, `""`, `None`, etc...) and everything else as True (eg `1`, `5.2`, `"shirt"`, etc...)._

#### Example:
```python
num_str = "123"
num_int = int(num_str)      # Converts numerical string to integer
pi_str = str(3.14159)       # Converts float 3.14159 to string "3.14159"
bool(0)                     # Converts a non-bool to bool
```

### Practice: Convert a float value to an integer and a string to a float.

### 3. Variables

**Variables** store data values. You assign values to variables using the `=` operator.

**Naming Rules**:
- Variable names must start with a letter or underscore (`_`), followed by letters, digits, or underscores.
- Variable names are case-sensitive (e.g., `name` and `Name` are different).

#### Example:
```python
age = 25            # Valid variable name
_name = "Alice"     # Valid variable name
1st_place = "Tom"   # Invalid (cannot start with a number)
```

**Printing Variables**:
Use the `print()` function to display a value in the terminal. This is a good way to check your variables and expressions! We represent terminal outputs with `>>> ` in our examples.

#### Example:
```python
my_num = 12
print(my_num)           # prints the value of my_num in the terminal

>>> 12

name = "John"
print("Hello, " + name) # evaluates this string concatination and prints the result in the terminal

>>> Hello, John
```

_Note: The `+` operator is normally used with numeric (int and float) values, but it can also be used to concatinate two strings as in the above example._

_You can also use `*` on a string and integer pair to repeat the string, eg `"go" * 3` == `"gogogo"`_

### 4. Statements & Expressions

A **statement** is a line of code that performs an action. For example, assigning a value to a variable is a statement.

An **expression** is a combination of values, variables, and operators that produce a new value.

#### Example:
```python
x = 5       # This is a statement
y = x + 10  # This is also a statement containing an expression, x + 10

```

### 5. Operators and Operands

**Operators** perform operations on values and variables (known as **operands**). Common types of operators include:

- **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%` (modulus), `**` (exponentiation), `//` (floor division)
- **Comparison Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical Operators**: `and`, `or`, `not`

Arithmetic operators can be used on two numeric operands (int or float). 

Generally speaking, arithmetic operators return an int if and only if both operands are ints. The exceptions are division `/` which always returns a float and floor division `//` which always returns an int, rounding down as needed.

#### Example:
```python
# Arithmetic operations
print(3 + 4.0)          # Arithmatic operation
>>> 7.0

print(10 == 10.0)       # Comparison operation
>>> True

print(True and False)   # Logical operation
>>> False
```

### Practice: Write a simple arithmetic expression that combines addition and multiplication and evaluates as an integer.

### 6. Input

Use the `input()` function to get input from the user. The function always returns the input as a string, so you may need to convert it to the appropriate data type.

#### Example:
```python
user_name = input("Enter your name: ")
age = int(input("Enter your age: "))  # Converts the input to an integer
```

### 7. Order of Operations

Python follows the standard mathematical order of operations (PEMDAS: Parentheses, Exponents, Multiplication & Division, Addition & Subtraction).

#### Example:
```python
result = 3 + 5 * 2  # Result is 13, because multiplication is done first
result = (3 + 5) * 2  # Result is 16, because parentheses override the usual order
```

### 8. Reassignment

You can **reassign** a variable by giving it a new value. You can also **update** a variable by performing an operation on its current value.

**Incrementing** is a common operation where you add to a variable’s current value using the `+=` operator.

#### Example:
```python
name = "John"       # Initial assignment
name = "Kyle"       # Reassigning the variable

count = 0           # Initial assignment
count = count + 1   # Reassigning the variable by updating it
count += 1          # Incrementing with += (same as count = count + 1)
```

This is also applicable for other arithmetic operations: `-=`, `*=`, `/=`, etc.

### Summary

In this lesson, you've learned:
1. Values and basic data types (integers, floats, strings, booleans)
2. Type conversion functions to switch between data types
3. How to name and assign values to variables, and print their values
4. Statements and expressions, and how they interact
5. Operators (arithmetic, comparison, and logical) and their operands
6. How to take user input using the `input()` function
7. The order of operations in Python
8. Reassigning and updating variables

### Practice Problems Recap:
1. Convert a float value to an integer and a string to a float.
2. Write a simple arithmetic expression using multiple operators.
3. Create a script that takes user input, performs an arithmetic operation, and prints the result.

Good luck, and happy coding! Feel free to reach out with any questions or clarifications.