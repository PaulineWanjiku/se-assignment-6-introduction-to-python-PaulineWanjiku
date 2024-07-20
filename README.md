[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15406932&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   .Python is an interpreted, object-oriented, high-level programming language that can be used to create applications for different uses.

Some of its features include

Object-Oriented

Has Lots of Libraries

Has Built-in Data Structures

Widely Applicable

It Increases Speed and Productivity

Easy to Learn

It can run on various platforms like windows, linux and macOS 

Cases where python is particularly effective

In web development to build dynamic web applications with frameworks like Django and flask.

Python is also used in data science and analytics for data manipulation, analysis and visualization using libraries like pandas.

It is used in automating file operations and web scraping.

Used to implement network protocols and SSH connections.

Python is also used in creation of simple 2D games.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Steps of installing python on my operating system

Windows

1.	Go to https://www.python.org/downloads/

2.	Select the python version to download

3.	Install then click on the downloaded file.

4.	Customize your installation by adding path, desired location and features etc.

5.	Then lastly start the installation

6.	Try and run python on cmd and to verify the installation just use python -v or python --version on cmd.


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   Python syntax to print hello world

print ("hello world!")

This prints Hello world! In the console after inputting python then file name with a .py extension on the console or terminal.

Basic syntax elements in python 
•	Print function ()
like in the example above the print function is used to output text to the console.
The text to be displayed is placed in the brackets.

•	String
it is characterized by quotation marks and it is just a sequence of characters. 



•	Brackets or parentheses ()
they are used to enclose arguments that are passed to functions as in the example above.


•	Quotation marks “”
used to define a string.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Data Types in Python 
•	List: Represents an ordered collection of items that can be of different types.

fruits = ["apple", "banana", "cherry"]

print ("fruits:", fruits)


•	Integer:

Represents whole numbers.

age = 25

print("Age:", age)


•	String data type: It is a sequence of characters.

name = "Alice"

print ("name:", name)


•	Boolean: has only True or False values.

is_student = True
 
print("is_student:", is_student)



•	Set: Unordered collection of unique items.

unique_numbers = {1, 2, 3, 4, 5}

print("\nUnique numbers:", unique_numbers)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional Statements and loops
They are used to run different blocks of code based on specific conditions.

Examples are if, else if, and else

e.g.,

if age >=18:

print(“You are an adult”)

else:

print(“You are a minor”)

This checks whether the first condition is true, if it is true, it returns the statement “you are an adult”
If the condition is false and age is not equal to or greater than 18 then the second statement is printed on the console.


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Functions in Python 

These are blocks of code that can be re used and are used to perform specific tasks.

They are defined by the keyword def then the function name and parameters enclosed in brackets.

Importance of functions

They allow the programmer to write a piece of code only once but can use it multiple times.

They break down complex problems into small pieces.

They make code more organized hence more readable

Updating and maintaining code is easier since changes are in one place.

Example of python function

Def add_numbers(a, b):
" This function takes two arguments, a and b, and returns their sum. "

Return a + b

#calling the function 

Result = add_numbers(3, 5)

#printing the result

Print (“the sum is:”, result)



7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists and dictionaries

Differences Between Lists and Dictionaries in Python

Lists:

Ordered collection of items.

Indexed by position, starting from 0.

Allow duplicate elements.

Elements can be of any data type.

Created using square brackets [].

Dictionaries:

Unordered collections of key-value pairs.

Indexed by unique keys. 

Keys must be unique and immutable; examples include strings, numbers, or tuples.

Values may be of any type.

Created using curly braces {}.


<!-- # Create a list of numbers -->

numbers = [1, 2, 3, 4, 5]

<!-- # Create a dictionary with key-value pairs -->

person = {
    "name": "John",
    "age": 30,
    "city": "New York"
}

<!-- # Basic operations on the list -->
print("Original list:", numbers)

<!-- # Append an item to the list -->
numbers.append(6)
print("After appending 6:", numbers)

<!-- # Access an item by index -->
print("Item at index 2:", numbers[2])

<!-- # Remove an item from the list -->
numbers.remove(3)
print("After removing 3:", numbers)

<!-- # Basic operations on the dictionary -->
print("Original dictionary:", person)

<!-- # Access a value by key -->
print("Name:", person["name"])

<!-- # Add a new key-value pair -->
person["email"] = "john@example.com"
print("After adding email:", person)

<!-- # Remove a key-value pair -->
del person["age"]
print("After removing age:", person)


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   . Exception Handling in Python
Exception handling can be defined as a mechanism in Python to 'catch' and 'handle' an exception or error when the program is executed. It lets the program continue executing or stop with a nice message without crashing. The key words used for exception handling are try, except, else, and finally.

try block: It contains that part of the code that might probably raise an exception.

Except block: This block contains code to be executed in case of an exception in the try block.

 Finally block: It is optional, but it always executes, whether an exception occurred or not.

Example
def divide_numbers(a, b):
    try:
        # Code that may raise an exception

        result = a / b

    except ZeroDivisionError as e:

        # Code to handle the exception

        print("Error: Cannot divide by zero.")

        print(f"Exception message: {e}")
    except TypeError as e:

        # Code to handle a different exception
        print("Error: Invalid input type. Please enter numbers.")

        print(f"Exception message: {e}")

    finally:
        # Code that always executes

        print("Execution completed.")

# Test cases

divide_numbers(10, 2)

divide_numbers(10, 0)

divide_numbers(10, 'a')


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Modules and Packages

 Modules:

A module is a file containing Python definitions and statements. It helps in organizing code by grouping related functionalities together.

Modules may define functions, classes, and variables. Moreover, it can include runnable code.

Packages:

A package is a way of organizing related modules into a directory hierarchy; it contains a special file called __init__.py that may even remain empty, informing Python that the directory must be treated as a package.

Packages enable a hierarchical structuring of the module namespace using dot notation.

Importing and using modules

The import statement is used to import modules.  An example using tge math module is

import math

result = math.sqrt(16)

print(result)  # Output: 4.0


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    .Reading and Writing to a file

In Python, reading from and writing to files is done using the built-in open() function along with several methods for manipulating files. Here are some examples on how to do this.

Read a File
Reading from a file involves the following steps:

Open the file using open() in read mode ('r').

Read the content using read(), readline(), or readlines() methods.

Close the file, or preferably use a context manager which will automatically handle the file.

Script for reading a file

<!-- # read_file.py

# Using a context manager to ensure the file is properly closed after reading -->

with open('example.txt', 'r') as file:

    content = file.read()  # Reads the entire content of the file

    print(content)  # Prints the content to the console

Writing to a File

 open the file in write, append, or write binary mode with the open().

Write the contents using write() or writelines() methods.

Also either close the file or use a context manager, as this does it automatically.

Script for writing to a file
<!-- # write_file.py -->

lines_to_write = ["First line\n", "Second line\n", "Third line\n"]

<!-- # Using a context manager to ensure the file is properly closed after writing -->

with open('output.txt', 'w') as file:

    file.writelines(lines_to_write)  # Writes the list of strings to the file


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


