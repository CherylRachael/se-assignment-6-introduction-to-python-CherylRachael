[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15286705&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

    Python is a high-level, interpreted programming language known for its simplicity, readability, and versatility. It was created by Guido van Rossum and first released in 1991. Python's design philosophy emphasizes code readability and simplicity, making it an excellent choice for both beginners and experienced developers.

Key Features of Python:
Readability and Simplicity:

Python's syntax is clear and easy to understand, which helps developers write code that is easy to read and maintain.
Example: Python uses indentation to define code blocks, which enforces a clean and consistent coding style.
def greet(name):
    print(f"Hello, {name}!")
Dynamically Typed:

Python does not require explicit declaration of variable types, making the code shorter and more flexible.
x = 10  # x is an integer
x = "Hello"  # now x is a string
Interpreted Language:

Python code is executed line by line, which makes debugging easier and more interactive.
Example: You can run Python scripts directly without the need for a compilation step
python script.py
Extensive Standard Library:

Python comes with a vast standard library that includes modules and packages for various tasks, from file I/O and system calls to web servers and data manipulation.
Example: Using the math library for mathematical functions.
import math
print(math.sqrt(16))  # Output: 4.0
Cross-Platform:

Python is available on multiple operating systems, including Windows, macOS, and Linux, allowing developers to write cross-platform code easily.
Large Ecosystem and Community:

Python has a rich ecosystem of third-party libraries and frameworks, such as NumPy, Pandas, Django, Flask, and TensorFlow.
import pandas as pd
df = pd.read_csv('data.csv')
print(df.head())
upport for Multiple Paradigms:

Python supports multiple programming paradigms, including procedural, object-oriented, and functional programming.
Example: Defining a class in Python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print(f"{self.name} makes a sound.")
Use Cases Where Python is Particularly Effective:
Web Development:

Python frameworks like Django and Flask are popular for building robust and scalable web applications.
Example: A simple web application using Flask
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, Flask!"

if __name__ == '__main__':
    app.run(debug=True)
Data Science and Machine Learning:
Libraries like NumPy, Pandas, Matplotlib, and scikit-learn make Python a go-to language for data analysis, visualization, and machine learning.
Example: Data manipulation using Pandas.
import pandas as pd
data = {'Name': ['Alice', 'Bob', 'Charlie'], 'Age': [25, 30, 35]}
df = pd.DataFrame(data)
print(df)
Scientific Computing:
Python, with libraries like SciPy and SymPy, is widely used in scientific computing and research.
Artificial Intelligence (AI) and Deep Learning:
Python frameworks like TensorFlow, Keras, and PyTorch are extensively used for developing AI and deep learning models.
Game Development:
Python, with libraries like Pygame, can be used for game development and prototyping.



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
  
Installing Python on Windows involves several steps. Here's a detailed guide on how to install Python, verify the installation, and set up a virtual environment.

Step 1: Download Python Installer
Visit the Python website:
Go to the official Python website: python.org.
Download the installer:
Navigate to the "Downloads" section and choose the latest stable release for Windows. The recommended version will be highlighted.
Click on the download link to get the Python installer (usually named something like python-3.x.x.exe).
Step 2: Run the Installer
Run the downloaded installer:

Locate the downloaded file and double-click it to start the installation process.
Customize Installation (optional):

The installer offers an option to "Add Python to PATH." Check this box to ensure Python is added to your system’s PATH environment variable.
Click on "Customize installation" if you want to specify installation options like installing pip (Python's package manager), documentation, or setting the installation location. Otherwise, you can go with the default settings by clicking "Install Now."
Complete the installation:

The installer will download and install Python along with its standard library and tools like pip.
Once the installation is complete, you will see a "Setup was successful" message.
Step 3: Verify the Installation
Open Command Prompt:
Press Win + R, type cmd, and press Enter to open the Command Prompt.
Check Python installation:
Type python --version and press Enter. You should see the installed Python version (e.g., Python 3.x.x).
Similarly, check pip installation by typing pip --version.

Step 4: Set Up a Virtual Environment
Navigate to your project directory:
Use the Command Prompt to navigate to the directory where you want to set up your project. For example:
cd C:\path\to\your\project
Create a virtual environment:
Run the following command to create a virtual environment named venv (you can name it anything you like):
python -m venv venv
Activate the virtual environment:
Activate the virtual environment using the following command:
venv\Scripts\activate
After activation, you will see (venv) prefixed to your command prompt, indicating that the virtual environment is active.
Deactivate the virtual environment:
To deactivate the virtual environment, simply run:
deactivate

Step 5: Installing Packages in the Virtual Environment
Ensure the virtual environment is active:
Make sure your virtual environment is activated ((venv) should be visible in your command prompt).
Install packages:
Use pip to install packages. For example, to install requests:
pip install requests
Freeze installed packages:
You can create a requirements.txt file with the list of installed packages for easier replication of the environment:
pip freeze > requirements.txt
Summary
Download and run the Python installer from the official Python website.
Choose to add Python to the system PATH during installation.
Verify the installation by checking the Python and pip versions in the Command Prompt.
Set up and activate a virtual environment using the venv module.
Install and manage packages within the virtual environment using pip


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

print("Hello, World!")
Explanation of Basic Syntax Elements
Function Call (print):

print is a built-in function in Python used to output text to the console.
In this program, print is called with the argument "Hello, World!".
String Literal ("Hello, World!"):

"Hello, World!" is a string literal, which is a sequence of characters enclosed in double quotes.
In Python, strings can be enclosed in either single quotes (') or double quotes ("), as long as they match.
Parentheses (()):
The parentheses () are used in function calls to enclose the arguments passed to the function.
Here, the string "Hello, World!" is the argument to the print function.
Additional Notes
Indentation:
Python uses indentation to define code blocks, such as those within functions, loops, and conditionals. However, for this simple program, no indentation is needed as it consists of a single line.
Comments:
Comments can be added to Python code using the # symbol. Comments are ignored by the Python interpreter and are used to add explanations or notes within the code.
No Semicolons:
Unlike some other programming languages, Python does not require semicolons to terminate statements. They can be used to separate multiple statements on a single line, but this is generally discouraged for readability.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

Python has several built-in data types that are used to store various kinds of information. Here are some of the basic data types in Python:

Integer (int):

Represents whole numbers, both positive and negative.
Example: 42, -3, 0.
Floating Point Number (float):

Represents real numbers, which can include decimal points.
Example: 3.14, -0.001, 2.0.
String (str):

Represents sequences of characters.
Example: "Hello, World!", 'Python', "123".
Boolean (bool):

Represents truth values: True or False.
Example: True, False.
List (list):

An ordered, mutable collection of items, which can be of any type.
Example: [1, 2, 3], ['apple', 'banana', 'cherry'].
Tuple (tuple):

An ordered, immutable collection of items, which can be of any type.
Example: (1, 2, 3), ('apple', 'banana', 'cherry').
Dictionary (dict):

An unordered collection of key-value pairs, where keys are unique.
Example: {'name': 'Alice', 'age': 25}, {'a': 1, 'b': 2}.
Set (set):

An unordered collection of unique items.
Example: {1, 2, 3}, {'apple', 'banana', 'cherry'}.
Short Script Demonstrating Different Data Types
Here's a Python script that demonstrates how to create and use variables of different data types:

python
Copy code
#Integer
age = 30
print("Age:", age)
print("Type of age:", type(age))

#Float
pi = 3.14159
print("Pi:", pi)
print("Type of pi:", type(pi))

#String
greeting = "Hello, World!"
print("Greeting:", greeting)
print("Type of greeting:", type(greeting))

#Boolean
is_python_fun = True
print("Is Python fun:", is_python_fun)
print("Type of is_python_fun:", type(is_python_fun))

#List
fruits = ['apple', 'banana', 'cherry']
print("Fruits:", fruits)
print("Type of fruits:", type(fruits))

#Tuple
coordinates = (10.0, 20.0)
print("Coordinates:", coordinates)
print("Type of coordinates:", type(coordinates))

#Dictionary
person = {'name': 'Alice', 'age': 25}
print("Person:", person)
print("Type of person:", type(person))

#Set
unique_numbers = {1, 2, 3, 2, 1}
print("Unique numbers:", unique_numbers)
print("Type of unique_numbers:", type(unique_numbers))
Explanation of the Script
Integer: age = 30

An integer variable age is assigned the value 30.
Float: pi = 3.14159

A float variable pi is assigned the value 3.14159.
String: greeting = "Hello, World!"

A string variable greeting is assigned the value "Hello, World!".
Boolean: is_python_fun = True

A boolean variable is_python_fun is assigned the value True.
List: fruits = ['apple', 'banana', 'cherry']

A list variable fruits is assigned a list of three fruit names.
Tuple: coordinates = (10.0, 20.0)

A tuple variable coordinates is assigned a tuple of two floating-point numbers.
Dictionary: person = {'name': 'Alice', 'age': 25}

A dictionary variable person is assigned a dictionary with two key-value pairs.
Set: unique_numbers = {1, 2, 3, 2, 1}

A set variable unique_numbers is assigned a set of numbers, demonstrating that duplicates are automatically removed.



5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

  Conditional Statements
Conditional statements allow you to execute certain blocks of code based on whether a condition is true or false. The most common conditional statements in Python are if, elif (else if), and else.

Example of an if-else Statement

age = 18

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
Explanation:

if age >= 18: checks if the value of age is 18 or greater.
If the condition is true, the block of code under the if statement is executed (print("You are an adult.")).
If the condition is false, the block of code under the else statement is executed (print("You are a minor.")).
You can also add more conditions using elif:


score = 85

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")
Explanation:

This checks multiple conditions in sequence.
Each condition is checked in order, and the corresponding block of code is executed for the first true condition.
Loops
Loops allow you to execute a block of code repeatedly. Python supports for and while loops.

Example of a for Loop

fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
Explanation:

for fruit in fruits: iterates over each item in the fruits list.
On each iteration, the variable fruit takes the value of the current item in the list.
The block of code under the for statement (print(fruit)) is executed for each item in the list.
Example of a while Loop
count = 0

while count < 5:
    print("Count:", count)
    count += 1
Explanation:

while count < 5: checks if the condition is true (count is less than 5).
If the condition is true, the block of code under the while statement is executed.
The statement count += 1 increments the value of count by 1 on each iteration.
The loop continues to execute as long as the condition is true.
Summary
Conditional statements (if-else):

Used to execute code blocks based on conditions.
Example:

if condition:
    # code block
elif another_condition:
    # another code block
else:
    # another code block
Loops (for, while):

Used to execute code blocks repeatedly.
for loop: Iterates over a sequence (like a list or a range).
for item in sequence:
    # code block
while loop: Repeats as long as a condition is true.
while condition:
    # code block
By using conditional statements and loops, you can control the flow of your Python programs and handle repetitive tasks efficiently.


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

Functions in Python are reusable blocks of code designed to perform a specific task. They help in organizing code, reducing repetition, and making code more modular and easier to maintain. Functions can take input arguments, process them, and return a result.
Key Benefits of Using Functions:
Reusability: Once a function is defined, it can be reused multiple times throughout the code.
Modularity: Functions help break down complex problems into smaller, manageable pieces.
Readability: Code with functions is generally easier to read and understand.
Maintainability: Functions make it easier to update and manage the code.

Defining a Function in Python
Here's a basic syntax for defining a function in Python:
def function_name(parameters):
    # function body
    return result
def: Keyword used to define a function.
function_name: The name of the function.
parameters: Input values that the function accepts.
function body: The block of code that runs when the function is called.
return: Keyword to return a value from the function (optional).

Example: Function to Return the Sum of Two Arguments
Here's a Python function that takes two arguments and returns their sum:


def add_numbers(a, b):
    """
    This function takes two arguments and returns their sum.
    """
    return a + b
Explanation:
def add_numbers(a, b):: Defines a function named add_numbers that takes two parameters, a and b.
return a + b: Returns the sum of a and b.
Calling the Function
To use the function, you call it with the required arguments:


# Example of calling the add_numbers function

result = add_numbers(5, 7)
print("The sum is:", result)
Explanation:
result = add_numbers(5, 7): Calls the add_numbers function with arguments 5 and 7, and stores the result in the variable result.
print("The sum is:", result): Prints the result to the console.
Complete Example
Here's the full code with function definition and an example call:


# Function definition

def add_numbers(a, b):
    """
    This function takes two arguments and returns their sum.
    """
    return a + b

# Example of calling the function

result = add_numbers(5, 7)
print("The sum is:", result)
Output:
The sum is: 12


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

Differences Between Lists and Dictionaries in Python

1. **Structure**:
   - **List**: An ordered collection of elements. Elements are accessed by their index, which is an integer starting from 0.
   - **Dictionary**: An unordered collection of key-value pairs. Elements are accessed by their keys, which can be of any immutable type (e.g., strings, numbers, tuples).

2. **Mutable**:
   - Both lists and dictionaries are mutable, meaning their contents can be changed after creation.

3. **Access Time**:
   - **List**: Access time is O(1) for indexing and O(n) for searching an element.
   - **Dictionary**: Access time is generally O(1) for key lookups.

4. **Syntax**:
   - **List**: Defined using square brackets `[]`.
     ```python
     my_list = [1, 2, 3, 4, 5]
     ```
   - **Dictionary**: Defined using curly braces `{}` with key-value pairs separated by colons.
     ```python
     my_dict = {'name': 'Alice', 'age': 25, 'city': 'New York'}
     ```

### Example Script

Here's a script that creates a list of numbers and a dictionary with some key-value pairs, and demonstrates basic operations on both.

```python
# Creating a list of numbers
numbers = [1, 2, 3, 4, 5]

# Creating a dictionary with some key-value pairs
person = {
    'name': 'Alice',
    'age': 25,
    'city': 'New York'
}

# Basic operations on the list
print("Original list:", numbers)

# Adding an element to the list
numbers.append(6)
print("List after append:", numbers)

# Removing an element from the list
numbers.remove(3)
print("List after remove:", numbers)

# Accessing an element by index
print("Element at index 2:", numbers[2])

# Basic operations on the dictionary
print("Original dictionary:", person)

# Adding a new key-value pair
person['email'] = 'alice@example.com'
print("Dictionary after adding email:", person)

# Updating the value for an existing key
person['age'] = 26
print("Dictionary after updating age:", person)

# Removing a key-value pair
del person['city']
print("Dictionary after deleting city:", person)

# Accessing a value by key
print("Name:", person['name'])
```

### Explanation of the Script

1. **Creating a List**:
   - `numbers = [1, 2, 3, 4, 5]`: Initializes a list of numbers.

2. **Creating a Dictionary**:
   - `person = {'name': 'Alice', 'age': 25, 'city': 'New York'}`: Initializes a dictionary with key-value pairs.

3. **List Operations**:
   - `numbers.append(6)`: Adds the element `6` to the end of the list.
   - `numbers.remove(3)`: Removes the first occurrence of the element `3` from the list.
   - `numbers[2]`: Accesses the element at index `2` (third element) in the list.

4. **Dictionary Operations**:
   - `person['email'] = 'alice@example.com'`: Adds a new key-value pair to the dictionary.
   - `person['age'] = 26`: Updates the value associated with the key `'age'`.
   - `del person['city']`: Deletes the key-value pair with the key `'city'`.
   - `person['name']`: Accesses the value associated with the key `'name'`.

Output

The script will produce the following output:

```
Original list: [1, 2, 3, 4, 5]
List after append: [1, 2, 3, 4, 5, 6]
List after remove: [1, 2, 4, 5, 6]
Element at index 2: 4
Original dictionary: {'name': 'Alice', 'age': 25, 'city': 'New York'}
Dictionary after adding email: {'name': 'Alice', 'age': 25, 'city': 'New York', 'email': 'alice@example.com'}
Dictionary after updating age: {'name': 'Alice', 'age': 26, 'city': 'New York', 'email': 'alice@example.com'}
Dictionary after deleting city: {'name': 'Alice', 'age': 26, 'email': 'alice@example.com'}
Name: Alice
```



8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

### Exception Handling in Python

Exception handling in Python is a way to manage errors gracefully during program execution, allowing the program to handle unexpected situations and continue running or terminate in a controlled manner. Python uses `try`, `except`, `else`, and `finally` blocks to manage exceptions.

#### Key Components of Exception Handling:

1. **`try` block**:
   - This block contains the code that might raise an exception.
2. **`except` block**:
   - This block contains the code that executes if an exception occurs in the `try` block.
3. **`else` block** (optional):
   - This block contains the code that executes if no exceptions occur in the `try` block.
4. **`finally` block** (optional):
   - This block contains the code that always executes, regardless of whether an exception occurred or not.

###Example: Using `try`, `except`, and `finally`

Here's an example of how to use `try`, `except`, and `finally` blocks in a Python script to handle errors:

```python
def read_file(file_path):
    try:
        file = open(file_path, 'r')
        content = file.read()
        print("File content:")
        print(content)
    except FileNotFoundError as e:
        print("Error: The file was not found.")
        print("Exception:", e)
    except IOError as e:
        print("Error: An I/O error occurred.")
        print("Exception:", e)
    finally:
        try:
            file.close()
        except NameError:
            print("Error: File was not opened, so it cannot be closed.")
        else:
            print("File has been closed.")

# Test cases
print("Test case 1: Valid file path")
read_file('example.txt')

print("\nTest case 2: Invalid file path")
read_file('nonexistent.txt')
```

### Explanation of the Script

1. **Function Definition**:
   - `def read_file(file_path):` defines a function to read the contents of a file specified by `file_path`.

2. **`try` Block**:
   - `try:` contains the code that might raise exceptions. In this case, it attempts to open and read the file.

3. **`except` Blocks**:
   - `except FileNotFoundError as e:` handles the case where the file does not exist. It catches the `FileNotFoundError` and prints an error message along with the exception details.
   - `except IOError as e:` handles I/O errors that might occur while opening or reading the file. It catches the `IOError` and prints an error message along with the exception details.

4. **`finally` Block**:
   - `finally:` contains code that always executes, regardless of whether an exception was raised or not. It attempts to close the file if it was successfully opened. The inner `try` block is used to catch a `NameError` if the file was never opened, ensuring the program doesn't crash when trying to close an unopened file.

### Test Cases

1. **Test Case 1: Valid File Path**:
   ```python
   read_file('example.txt')
   ```
   - This case assumes `example.txt` exists and is readable. It will open, read, and print the file's content, then close the file.

2. **Test Case 2: Invalid File Path**:
   ```python
   read_file('nonexistent.txt')
   ```
   - This case assumes `nonexistent.txt` does not exist. It will raise a `FileNotFoundError`, print an error message, and attempt to close the file, which was never opened.

### Output

The script will produce the following output:

```
Test case 1: Valid file path
Error: The file was not found.
Exception: [Errno 2] No such file or directory: 'example.txt'
Error: File was not opened, so it cannot be closed.

Test case 2: Invalid file path
Error: The file was not found.
Exception: [Errno 2] No such file or directory: 'nonexistent.txt'
Error: File was not opened, so it cannot be closed.
```

This example demonstrates how to use `try`, `except`, and `finally` blocks to handle exceptions in Python, ensuring that errors are managed gracefully and necessary cleanup (like closing a file) is always performed.



9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

In Python, modules and packages are mechanisms for organizing and reusing code. They help in maintaining clean and manageable codebases by allowing you to split your code into smaller, logical units and reuse them across multiple projects.

### Modules

A module is a Python file containing Python definitions, statements, and functions. These files have a `.py` extension and can be imported into other Python scripts. Modules allow you to logically organize your Python code into reusable units.

### Packages

A package is a collection of related modules organized in a directory structure. A package contains an `__init__.py` file (which can be empty) to indicate that the directory should be treated as a package. Packages help in hierarchical organization and prevent naming conflicts.

### Importing and Using Modules

You can import a module into your Python script using the `import` statement. Once imported, you can access functions, variables, and classes defined in the module using dot notation (`module_name.function_name`).

### Example Using the `math` Module

The `math` module provides mathematical functions and constants for performing mathematical operations in Python.

```python
import math

# Using math module functions
print("Square root of 16:", math.sqrt(16))
print("Value of pi:", math.pi)
print("Factorial of 5:", math.factorial(5))
```

### Explanation

- **`import math`**: Imports the `math` module into the current script, allowing access to its functions and constants.
- **`math.sqrt(16)`**: Calculates the square root of 16 using the `sqrt` function from the `math` module.
- **`math.pi`**: Accesses the value of pi (π) constant defined in the `math` module.
- **`math.factorial(5)`**: Calculates the factorial of 5 using the `factorial` function from the `math` module.

### Output

The script will produce the following output:

```
Square root of 16: 4.0
Value of pi: 3.141592653589793
Factorial of 5: 120
```

This example demonstrates how to import and use the `math` module in Python to perform mathematical calculations. Similarly, you can import and use other built-in or third-party modules in your Python scripts to leverage their functionality and simplify your code.



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

Reading from and writing to files in Python is straightforward using built-in functions and methods provided by the language.

### Reading from a File

You can read from a file in Python using the `open()` function to open a file object and then using methods like `read()`, `readline()`, or `readlines()` to read the content.

Here's a script that reads the content of a file and prints it to the console:

```python
# Open the file in read mode
with open('example.txt', 'r') as file:
    # Read the entire content of the file
    content = file.read()

# Print the content to the console
print("File Content:")
print(content)
```

### Writing to a File

You can write to a file in Python using the `open()` function with the appropriate mode (e.g., `'w'` for write mode) and then using methods like `write()` to write content to the file.

Here's a script that writes a list of strings to a file:

```python
# List of strings
lines = ['First line\n', 'Second line\n', 'Third line\n']

# Open the file in write mode
with open('output.txt', 'w') as file:
    # Write each line from the list to the file
    for line in lines:
        file.write(line)
```

### Explanation

- **Reading from a File**:
  - `open('example.txt', 'r')`: Opens the file named `example.txt` in read mode.
  - `file.read()`: Reads the entire content of the file.
  - The `with` statement ensures that the file is properly closed after reading.

- **Writing to a File**:
  - `open('output.txt', 'w')`: Opens (or creates if it doesn't exist) the file named `output.txt` in write mode.
  - `file.write(line)`: Writes each line from the list to the file.
  - The `with` statement ensures that the file is properly closed after writing.

### Output

Assuming the file `example.txt` contains the following content:
```
This is line 1.
This is line 2.
This is line 3.
```

After running the first script, the output will be:
```
File Content:
This is line 1.
This is line 2.
This is line 3.
```

After running the second script, the file `output.txt` will contain:
```
First line
Second line
Third line
```

These examples demonstrate how to read from and write to files in Python using built-in functions and methods, providing flexibility for file manipulation tasks.


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


