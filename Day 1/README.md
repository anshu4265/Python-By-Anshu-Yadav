# 🐍 Python Programming — Complete Beginner Notes

> **Learning setup:** Jupyter Notebook (`.ipynb`)  
> **Style:** Beginner-friendly notes with examples, outputs, and Hinglish explanations.

---

## Table of Contents

1. [Introduction to Python](#1-introduction-to-python)
2. [History of Python](#2-history-of-python)
3. [Features and Applications](#3-features-and-applications)
4. [Advantages and Disadvantages](#4-advantages-and-disadvantages)
5. [Python Versions](#5-python-versions)
6. [Python Development Environment: Jupyter Notebook](#6-python-development-environment-jupyter-notebook)
7. [Basic Syntax Rules](#7-basic-syntax-rules)
8. [Variables](#8-variables)
9. [Data Types](#9-data-types)
10. [Type Conversion / Type Casting](#10-type-conversion--type-casting)
11. [Input and Output](#11-input-and-output)
12. [Operators in Python](#12-operators-in-python)
13. [Operator Precedence](#13-operator-precedence)
14. [Common Mistakes](#14-common-mistakes)
15. [Practice Questions](#15-practice-questions)
16. [College Viva Questions](#16-college-viva-questions)
17. [Quick Revision](#17-quick-revision)
18. [Next Topic](#18-next-topic)

---

## 1. Introduction to Python

**Definition:** Python is a high-level, general-purpose programming language known for its readable syntax. It is commonly described as an interpreted language because Python code is processed and executed by a Python implementation at runtime.

Hinglish: Python ek programming language hai jiske through hum computer ko instructions dete hain. Iska syntax beginner-friendly aur readable hota hai.

### First Python Program

```python
print("Hello World")
```

**Output**
```text
Hello World
```

**Explanation**
- `print()` is a built-in function used to display output.
- `"Hello World"` is a string (text enclosed in quotation marks).
- Parentheses `()` contain the value passed to the function.

---

## 2. History of Python

Python was created by **Guido van Rossum**, a Dutch programmer.

- **December 1989:** Python development began.
- **1991:** Python's first public release became available.
- **2000:** Python 2.0 was released.
- **2008:** Python 3.0 was released with significant improvements and some backward-incompatible changes.
- **Today:** Python is widely used in AI, machine learning, web development, automation, data analysis, and scientific computing.

### Why is it called Python?

The name *Python* was inspired by the British comedy television show **Monty Python's Flying Circus**, not by the snake.

---

## 3. Features and Applications

### Main Features

1. **High-level:** Syntax is relatively easy for humans to read.
2. **Easy to learn:** Its syntax is simple and readable.
3. **Interpreted:** Code is processed by a Python implementation at runtime.
4. **General-purpose:** It can be used to build different kinds of applications.
5. **Dynamically typed:** You generally do not need to declare a variable's type explicitly.
6. **Cross-platform:** Programs can run on different operating systems, subject to compatibility.
7. **Open-source:** Python is freely available and its source code can be accessed.
8. **Large standard library:** Many useful modules are included with Python.

### Applications

- Artificial Intelligence (AI)
- Machine Learning (ML)
- Web development
- Data science and data analysis
- Automation and scripting
- Scientific computing
- Software development
- Cybersecurity tools and testing

---

## 4. Advantages and Disadvantages

### Advantages

- Simple and readable syntax.
- Suitable for beginners.
- Supports procedural and object-oriented programming, among other styles.
- Large community and ecosystem of libraries.
- Useful for developing many applications quickly.
- Cross-platform support.

### Disadvantages

- Can be slower than compiled languages such as C and C++ for some CPU-intensive tasks.
- May use more memory than some lower-level languages.
- Less commonly used than platform-specific tools for native Android and iOS development.
- Some type-related errors may only appear when the program runs.
- In standard GIL-enabled CPython builds, the Global Interpreter Lock can limit parallel execution of Python bytecode across threads for CPU-bound work.
- Python's high-level abstractions may be less suitable when direct hardware control or precise low-level memory management is needed.

**Note:** These limitations do not make Python a bad language. Its suitability depends on the application's requirements. Database performance, for example, depends on the database, driver, queries, and application design.

---

## 5. Python Versions

### Python 2
- Released in 2000.
- Introduced several useful language features.
- Official support ended on **January 1, 2020**.

### Python 3
- Released in 2008.
- Improved language design and consistency.
- **Recommended for new Python projects.**

---

## 6. Python Development Environment: Jupyter Notebook

Jupyter Notebook is an interactive environment where you write and execute Python code in separate cells.

### Features

- **Code cells:** Write and execute Python code.
- **Output display:** Results appear below the cell.
- **Interactive execution:** Run one cell at a time.
- **Shared kernel:** Variables can be reused across cells while the kernel session remains active.

### Running code

```python
print("Hello World")
```

**Output**
```text
Hello World
```

### Useful shortcut

- **`Shift + Enter`** — runs the current cell and selects the next cell.

**Important:** You can execute Python directly in a Jupyter Notebook without creating a separate `.py` file. A `.py` file is a Python script; `.ipynb` is a Jupyter Notebook file.

---

## 7. Basic Syntax Rules

- Python is **case-sensitive**: `name` and `Name` are different identifiers.
- **Indentation** is important for defining code blocks.
- Strings can use single or double quotation marks.
- A semicolon is generally not required at the end of a statement.
- Comments begin with `#`.

### Example

```python
# This is a comment
print("Hello Python")
print('I am learning Python')
```

**Output**
```text
Hello Python
I am learning Python
```

---

## 8. Variables

### What is a variable?

A variable is a name used to store and access a value in a program.

Hinglish: Variable ko ek labelled box ki tarah samjho. Box ka naam `age` hai aur usmein `18` value rakhi hai.

```python
age = 18
print(age)
```

**Output**
```text
18
```

### Line-by-line explanation

- `age` — variable ka naam.
- `=` — assignment operator; right-side value ko left-side variable mein assign karta hai.
- `18` — integer value.
- `print(age)` — variable ki stored value display karta hai.

**Important:** `age = 18` mein `=` assignment hai, comparison nahi. Equality compare karne ke liye `==` use hota hai.

### Variable examples

```python
name = "Anshu"
age = 18
marks = 85.5
is_student = True

print(name)
print(age)
print(marks)
print(is_student)
```

**Output**
```text
Anshu
18
85.5
True
```

### Variable naming rules

1. A variable name must start with a letter or underscore (`_`).
2. It cannot start with a number.
3. Spaces are not allowed.
4. Python is case-sensitive: `age` and `Age` are different.
5. Reserved keywords such as `if`, `for`, and `class` cannot be used as variable names.

**Valid:** `age`, `student_name`, `_count`, `marks2`  
**Invalid:** `2marks`, `student name`, `class`

---

## 9. Data Types

A data type tells us what kind of value a variable holds.

| Data type | Meaning | Examples |
|---|---|---|
| `int` | Integer numbers | `10`, `-5`, `100` |
| `float` | Decimal numbers | `3.14`, `85.5` |
| `str` | Text/string | `"Hello"`, `'Python'` |
| `bool` | Boolean value | `True`, `False` |

### Check a data type using `type()`

```python
age = 18
marks = 85.5
name = "Anshu"
is_student = True

print(type(age))
print(type(marks))
print(type(name))
print(type(is_student))
```

**Output**
```text
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```

Remember: `True` and `False` start with capital letters in Python.

---

## 10. Type Conversion / Type Casting

**Definition:** Type casting is the process of converting a value from one data type to another.

Hinglish: Jab hum kisi value ka data type change karte hain, jaise `int` se `float` ya `str` se `int`, use type conversion/type casting kehte hain.

### Important conversion functions

| Function | Purpose | Example | Result |
|---|---|---|---|
| `int()` | Convert to integer | `int(4.9)` | `4` |
| `float()` | Convert to float | `float(5)` | `5.0` |
| `str()` | Convert to string | `str(100)` | `"100"` |
| `bool()` | Convert to Boolean | `bool(1)` | `True` |
| `list()` | Convert an iterable to a list | `list("abc")` | `['a', 'b', 'c']` |
| `tuple()` | Convert an iterable to a tuple | `tuple([1, 2])` | `(1, 2)` |

**Important:** `int(4.9)` gives `4`, not `5`. `int()` removes the decimal part; it does not round to the nearest integer.

### Example: integer to float

```python
a = 10
b = float(a)

print(a)
print(b)
print(type(a))
print(type(b))
```

**Output**
```text
10
10.0
<class 'int'>
<class 'float'>
```

### Two types of conversion

#### 1. Implicit type conversion (automatic)

Python automatically converts compatible values during some operations.

```python
a = 5
b = 2.0
c = a + b

print(c)
print(type(c))
```

**Output**
```text
7.0
<class 'float'>
```

Here, the integer participates in the calculation as a float, so the result is `7.0`.

#### 2. Explicit type casting (manual)

The programmer uses a function such as `int()`, `float()`, or `str()`.

```python
x = "25"
y = int(x)

print(y)
print(type(y))
```

**Output**
```text
25
<class 'int'>
```

The value `"25"` was a string; `int(x)` converted it to an integer.

---

## 11. Input and Output

### Display output with `print()`

```python
print("Hello Python")
print(10)
```

### Take input with `input()`

The `input()` function receives information from the user through the keyboard.

```python
name = input("Enter your name: ")
print("Hello", name)
```

### Important: `input()` returns a string

```python
age = input("Enter your age: ")
print(type(age))
```

Even if the user types `18`, `input()` returns `"18"` as a string by default.

### Convert input for calculations

```python
age = int(input("Enter your age: "))
print("Next year your age will be", age + 1)
```

**Example output**
```text
Enter your age: 18
Next year your age will be 19
```

If the input cannot be converted to an integer (for example, the user types `"hello"`), `int()` raises a `ValueError`.

---

## 12. Operators in Python

### What is an operator?

An operator is a symbol or keyword that performs an operation on one or more values or variables.

Hinglish: Operator ek symbol/keyword hota hai jo values par operation karta hai, jaise addition, comparison ya logical checking.

### Main types of operators

1. Arithmetic operators
2. Comparison operators
3. Logical operators
4. Assignment operators
5. Membership operators
6. Identity operators
7. Bitwise operators

### 12.1 Arithmetic operators

Used for mathematical calculations.

| Operator | Name | Example | Result |
|---|---|---|---:|
| `+` | Addition | `10 + 3` | `13` |
| `-` | Subtraction | `10 - 3` | `7` |
| `*` | Multiplication | `10 * 3` | `30` |
| `/` | Division | `10 / 3` | `3.333...` |
| `//` | Floor division | `10 // 3` | `3` |
| `%` | Modulus (remainder) | `10 % 3` | `1` |
| `**` | Exponentiation (power) | `2 ** 3` | `8` |

Example:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a // b)
print(a % b)
print(2 ** 3)
```

**Note:** `%` is useful for checking divisibility and finding even/odd numbers.

```python
number = 8
print(number % 2)
```

Output: `0`

If `number % 2 == 0`, the number is even; otherwise, it is odd.

### 12.2 Comparison operators

Compare two values and return `True` or `False`.

| Operator | Meaning | Example | Result |
|---|---|---|---|
| `==` | Equal to | `5 == 5` | `True` |
| `!=` | Not equal to | `5 != 3` | `True` |
| `>` | Greater than | `8 > 5` | `True` |
| `<` | Less than | `2 < 5` | `True` |
| `>=` | Greater than or equal to | `5 >= 5` | `True` |
| `<=` | Less than or equal to | `3 <= 5` | `True` |

```python
a = 10
b = 5

print(a > b)
print(a == b)
print(a != b)
```

**Output**
```text
True
False
True
```

### 12.3 Logical operators

Used to combine or reverse conditions.

| Operator | Meaning | Example |
|---|---|---|
| `and` | True when both conditions are true | `age >= 18 and has_id` |
| `or` | True when at least one condition is true | `is_weekend or is_holiday` |
| `not` | Reverses a Boolean result | `not is_raining` |

```python
age = 20
has_id = True

print(age >= 18 and has_id)
print(age < 18 or has_id)
print(not has_id)
```

**Output**
```text
True
True
False
```

### 12.4 Assignment operators

Used to assign or update a variable's value.

| Operator | Example | Equivalent idea |
|---|---|---|
| `=` | `x = 5` | Assign `5` to `x` |
| `+=` | `x += 2` | `x = x + 2` |
| `-=` | `x -= 2` | `x = x - 2` |
| `*=` | `x *= 2` | `x = x * 2` |
| `/=` | `x /= 2` | `x = x / 2` |
| `//=` | `x //= 2` | `x = x // 2` |
| `%=` | `x %= 2` | `x = x % 2` |
| `**=` | `x **= 2` | `x = x ** 2` |

```python
x = 10
x += 5
print(x)
```

Output: `15`

### 12.5 Membership operators

Check whether a value exists in a sequence or collection.

| Operator | Meaning |
|---|---|
| `in` | Value is present |
| `not in` | Value is not present |

```python
name = "Python"

print("P" in name)
print("z" not in name)
```

**Output**
```text
True
True
```

### 12.6 Identity operators

Check whether two references point to the same object, not merely whether their values are equal.

| Operator | Meaning |
|---|---|
| `is` | Both references point to the same object |
| `is not` | References point to different objects |

Use `==` to compare values. Use `is` especially for identity checks such as `value is None`.

```python
x = None
print(x is None)
```

Output: `True`

### 12.7 Bitwise operators

Bitwise operators work on the binary representation of integers.

| Operator | Name |
|---|---|
| `&` | Bitwise AND |
| `\|` | Bitwise OR |
| `^` | Bitwise XOR |
| `~` | Bitwise NOT |
| `<<` | Left shift |
| `>>` | Right shift |

Example:

```python
a = 5   # binary: 0101
b = 3   # binary: 0011

print(a & b)
print(a | b)
print(a ^ b)
print(a << 1)
print(a >> 1)
```

**Output**
```text
1
7
6
10
2
```

Bitwise operators are useful in some low-level, binary, and performance-related tasks. Learn the basic arithmetic and comparison operators first.

---

## 13. Operator Precedence

Operator precedence determines which operation is evaluated first in an expression.

A simplified order for common operators, from higher to lower precedence:

1. Parentheses: `()`
2. Exponentiation: `**`
3. Unary operators: `+x`, `-x`, `not`
4. Multiplication/division/floor division/modulus: `*`, `/`, `//`, `%`
5. Addition/subtraction: `+`, `-`
6. Comparisons: `==`, `!=`, `>`, `<`, `>=`, `<=`
7. Logical `and`
8. Logical `or`

When unsure, use parentheses to make the intended order clear.

```python
print(2 + 3 * 4)
print((2 + 3) * 4)
```

**Output**
```text
14
20
```

In the first expression, multiplication happens before addition. In the second, parentheses make addition happen first.

---

## 14. Common Mistakes

- Using `=` when you mean to compare values. Use `==` for equality comparison.
- Forgetting that `input()` returns a string.
- Writing `True` or `False` in lowercase; Python uses `True` and `False`.
- Using a variable before assigning it a value.
- Using inconsistent indentation in code blocks.
- Expecting `int(4.9)` to round to `5`; it returns `4`.
- Using `is` to compare ordinary values; generally use `==` for value comparison.
- Forgetting that `/` performs true division, while `//` performs floor division.

---

## 15. Practice Questions

Try these in separate Jupyter Notebook cells. Attempt them before checking a solution.

### Variables and data types
1. Create variables for your name, age, percentage, and student status. Print each value.
2. Use `type()` to display the data type of `25`, `4.5`, `"Hello"`, and `False`.

### Type casting and input
3. Ask the user for their age and print how old they will be next year.
4. Convert the string `"123"` to an integer and print its type.
5. Convert `7` to a float and print the result.

### Operators
6. Find the quotient and remainder when `29` is divided by `4`.
7. Take a number as input and check whether it is even or odd.
8. Ask the user for two numbers and print their sum, difference, product, and division result.
9. Predict the output of `2 + 3 * 4` and `(2 + 3) * 4`.
10. Given `x = 10`, use `+=` to add `5` and print the updated value.
11. Check whether the letter `"y"` exists in the string `"Python"`.
12. Use comparison operators to check whether one input number is greater than another.

### Mini challenge: Can the person vote?

Use a conditional statement to check whether a person's age is at least 18.

```python
age = int(input("Enter your age: "))

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
```

**How it works**
- `input()` gets the age from the user.
- `int()` converts the input string to an integer.
- `if age >= 18` checks the condition.
- If the condition is true, the first message is printed; otherwise, the `else` message is printed.

This is an introductory example of the next topic: **conditional statements**. Actual voting eligibility depends on the applicable election laws and registration requirements; this example only demonstrates the basic age condition.

---

## 16. College Viva Questions

1. What is Python?
2. Who developed Python?
3. When did Python development begin?
4. When was Python first publicly released?
5. Why is Python called Python?
6. What are the main features of Python?
7. What is the difference between Python 2 and Python 3?
8. What are the applications of Python?
9. What is an interpreted language?
10. What is dynamic typing?
11. What is a variable?
12. What are `int`, `float`, `str`, and `bool`?
13. What does the `type()` function do?
14. What is type casting?
15. What is the difference between implicit and explicit type conversion?
16. What does `input()` return by default?
17. What is the difference between `=` and `==`?
18. What is the difference between `/` and `//`?
19. What does the modulus operator `%` do?
20. What is the difference between `and`, `or`, and `not`?
21. What are membership operators?
22. What are identity operators?
23. Why is indentation important in Python?
24. What is operator precedence?

---

## 17. Quick Revision

| Topic | Key point |
|---|---|
| Creator | Guido van Rossum |
| Development began | December 1989 |
| First public release | 1991 |
| Python 2.0 | 2000 |
| Python 3.0 | 2008 |
| Name inspiration | *Monty Python's Flying Circus* |
| Recommended version | Python 3 |
| Python script extension | `.py` |
| Jupyter Notebook extension | `.ipynb` |
| Output function | `print()` |
| Input function | `input()` |
| Comment symbol | `#` |
| Check data type | `type()` |
| Assignment | `=` |
| Equality comparison | `==` |
| Integer conversion | `int()` |
| Float conversion | `float()` |
| String conversion | `str()` |
| Boolean values | `True`, `False` |
| Remainder | `%` |
| Floor division | `//` |
| Power | `**` |
| Logical operators | `and`, `or`, `not` |
| Membership operators | `in`, `not in` |
| Identity operators | `is`, `is not` |

---

## 18. Next Topic

**Conditional Statements in Python**
- `if`
- `if-else`
- `if-elif-else`
- Nested `if`
- Practical examples and practice questions

**Study tip:** Run every code example in Jupyter Notebook, predict its output before running it, and then change the values to see what happens.
