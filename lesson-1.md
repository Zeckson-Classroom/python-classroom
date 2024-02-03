# Python basics

## Variables

In Python, variables are used to store data values. Unlike some other programming languages, Python does not require you
to explicitly declare the data type of a variable. The interpreter automatically identifies the type based on the value
assigned to it. Here's how you define and use variables in Python:

### Variable Naming Rules:

- Variable names can contain letters (a-z, A-Z), digits (0-9), and underscores (_).
- Variable names cannot start with a digit.
- Variable names are case-sensitive.
- Variable names cannot be reserved words (e.g., `if`, `else`, `for`, `while`, `def`, `class`, etc.).

### Assigning Values to Variables:

You can assign values to variables using the assignment operator (=).

```python
x = 5  # x is assigned the value 5 (an integer)
name = "John"  # name is assigned the value "John" (a string)
pi = 3.14  # pi is assigned the value 3.14 (a float)
```

### Variable Reassignment:

You can change the value of a variable by assigning it a new value.

```python
x = 5  # x is assigned the value 5
x = 10  # x is reassigned the value 10
```

### Multiple Assignment:

You can assign values to multiple variables in a single line.

```python
a, b, c = 5, 10, 15
```

### Variable Concatenation:

You can concatenate variables of the same type using the `+` operator (for strings) or perform arithmetic operations
with numeric variables.

```python
first_name = "John"
last_name = "Doe"
full_name = first_name + " " + last_name  # Concatenating strings

x = 5
y = 3
z = x + y  # Performing arithmetic operation
```

### Print Variables:

You can print the value of a variable using the `print()` function.

```python
age = 30
print("My age is", age)
```

Variables are a fundamental concept in programming and are used extensively to store and manipulate data in Python
programs. Understanding how to use variables effectively is crucial for writing readable and maintainable code.

## Data Types

### Number type

In Python, there are several numeric data types that you can use to represent numbers in your programs. The primary
numeric data types in Python include:

#### 1. Integer (int):

Integers represent whole numbers, both positive and negative, without any decimal point. They can be of unlimited size,
subject to available memory.

Example:

```python
x = 5
y = -10
```

#### 2. Float (float):

Floats represent real numbers, including both integer and fractional parts. They are represented with a decimal point.

Example:

```python
pi = 3.14
temperature = -20.5
```

#### 3. Complex (complex):

Complex numbers consist of a real part and an imaginary part, represented as `a + bj`, where `a` is the real part
and `b` is the imaginary part.

Example:

```python
z = 2 + 3j
```

#### Numeric Operations:

Python supports various arithmetic operations on numeric data types, including addition (+), subtraction (-),
multiplication (*), division (/), modulus (%), exponentiation (**), and floor division (//).

Example:

```python
x = 10
y = 3

print(x + y)  # Output: 13
print(x - y)  # Output: 7
print(x * y)  # Output: 30
print(x / y)  # Output: 3.3333333333333335
print(x % y)  # Output: 1
print(x ** y)  # Output: 1000
print(x // y)  # Output: 3
```

Understanding the different numeric data types and their operations is crucial for performing calculations, representing
quantities, and making decisions in Python programs.

### String type

In Python, strings are sequences of characters, and they are one of the most commonly used data types. Strings in Python
are immutable, meaning once they are created, they cannot be changed.

Here's how you define strings in Python:

```python
my_string = "Hello, World!"
```

Strings can be enclosed in single quotes (' '), double quotes (" "), or triple quotes (''' ''' or """ """). The choice
of quotation style depends on your preference and the specific requirements of your string.

#### Basic String Operations:

Python provides a variety of operations that you can perform on strings:

1. **Concatenation:**
You can concatenate (join) two or more strings using the `+` operator.

Example:
```python
greeting = "Hello"
name = "John"
message = greeting + ", " + name + "!"
print(message)  # Output: Hello, John!
```

2. **Repetition:**
You can repeat a string multiple times using the `*` operator.

Example:
```python
word = "Python "
repeated_word = word * 3
print(repeated_word)  # Output: Python Python Python 
```

## `input()` function

In Python, the `input()` function is used to accept user input from the keyboard. It allows the program to pause and wait for the user to enter some data, which is then read as a string. Here's how you use the `input()` function:

```python
user_input = input("Enter your name: ")
```

In this example, the string "Enter your name: " is passed as an argument to the `input()` function. This string serves as a prompt, providing guidance to the user about what type of input is expected. The user is then prompted to enter their name.

After the user enters their name and presses the Enter key, the `input()` function will read the input and return it as a string, which can be assigned to a variable (`user_input` in this case).

You can use the `input()` function without any arguments:

```python
user_input = input()
```

In this case, the program will simply wait for the user to input any value and press Enter. The entered value will be stored as a string in the variable `user_input`.

### Converting Input to Other Data Types:

By default, the `input()` function always returns the user's input as a string. If you expect the user to enter a different data type (e.g., integer, float), you need to explicitly convert the input using the appropriate typecasting function (`int()`, `float()`, etc.).

```python
age = input("Enter your age: ")
age = int(age)  # Convert the input string to an integer
```

### Example:

Here's a simple example of using the `input()` function to accept user input and perform an operation based on the input:

```python
# Accept user input for two numbers
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))

# Calculate the sum of the two numbers
sum = num1 + num2

# Display the result
print("The sum of", num1, "and", num2, "is", sum)
```

In this example, the user is prompted to enter two numbers. The numbers are converted to floats using the `float()` function, and then the sum is calculated and printed.