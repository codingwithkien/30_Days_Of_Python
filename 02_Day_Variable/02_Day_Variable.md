<div align="center">
  <h1> 30_Days_Of_Python: 02_Day_Variable</h1>


<sub>Author:
<a href="https://www.facebook.com/duongtrungkien062003"> Duong Trung Kien</a><br>
<small>October, 2022</small>
</sub>

</div>

[<< 01_Day](../01_Day_Introduction/01_Day_Introduction.py) | [03_Day >>](../03_Day_Operators/03_Day_Operators.md)

![30DaysOfPython](https://camo.githubusercontent.com/59a720eaa51a6bbc45ba76313bf53a4f2c84dde994c947809a49b41f3c828ef2/68747470733a2f2f7374617469632e636f64696e67666f72656e7472657072656e657572732e636f6d2f6d656469612f70726f6a656374732f33302d646179732d707974686f6e2d33382f696d616765732f73686172652f33305f446179735f6f665f507974686f6e5f2d5f53686172652e6a7067)

- [📘 02_Day](#-day-2)
  - [Built in functions](#built-in-functions)
  - [Variables](#variables)
    - [Declaring Multiple Variable in a Line](#declaring-multiple-variable-in-a-line)
  - [Data Types](#data-types)
  - [Checking Data types and Casting](#checking-data-types-and-casting)
  - [Numbers](#numbers)
  - [💻 Exercises - 02_Day](#-exercises---day-2)
    - [Exercises: Level_01](#exercises-level-1)
    - [Exercises: Level_02](#exercises-level-2)

# 📘 02_Day

## Built in functions

In Python we have lots of built-in functions. Built-in functions are globally available for your use that mean you can make use of the built-in functions without importing or configuring. Some of the most commonly used Python built-in functions are the following: _print()_, _len()_, _type()_, _int()_, _float()_, _str()_, _input()_, _list()_, _dict()_, _min()_, _max()_, _sum()_, _sorted()_, _open()_, _file()_, _help()_, and _dir()_. In the following table you will see an exhaustive list of Python built-in functions taken from [python documentation](https://docs.python.org/3.9/library/functions.html).


## Variables

Variables store data in a computer memory. Mnemonic variables are recommended to use in many programming languages. A mnemonic variable is a variable name that can be easily remembered and associated. A variable refers to a memory address in which data is stored.
Number at the beginning, special character, hyphen are not allowed when naming a variable. A variable can have a short name (like x, y, z), but a more descriptive name (firstname, lastname, age, country) is highly recommended.

Python Variable Name Rules

- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and \_ )
- Variable names are case-sensitive (firstname, Firstname, FirstName and FIRSTNAME) are different variables)

Let us se valid variable names

```shell
firstname
lastname
age
country
city
first_name
last_name
capital_city
_if # if we want to use reserved word as a variable
year_2022
year2022
current_year_2022
birth_year
num1
num2
```

Invalid variables names

```shell
first-name
first@name
first$name
num-1
1num
```

We will use standard Python variable naming style which has been adopted by many Python developers. Python developers use snake case(snake_case) variable naming convention. We use underscore character after each word for a variable containing more than one word(eg. first_name, last_name, engine_rotation_speed).  The example below is an example of standard naming of variables, underscore is required when the variable name is more than one word.

When we assign a certain data type to a variable, it is called variable declaration. For instance in the example below my first name is assigned to a variable first_name. The equal sign is an assignment operator. Assigning means storing data in the variable. The equal sign in Python is not equality as in Mathematics.

_Example:_

```py
# Variables in Python
first_name = 'Duong'
middle_name = 'Trung'
last_name = 'Kien'
country = 'Quang Ngai'
city = 'Ho Chi Minh City'
age = 19
is_married = False
skills = ['HTML', 'CSS', 'JS', 'React', 'C++', 'Python']
person_info = {
   'firstname':'Duong',
   'middlename': 'Trung',
   'lastname':'Kien',
   'country':'Quang Ngai',
   'city':'Ho Chi Minh City'
   }
```

Let us use the _print()_ and _len()_ built-in functions. Print function takes unlimited number of arguments. An argument is a value which we can be passed or put inside the function parenthesis, see the example below.

**Example:**

```py
print('Hello, World!') # The text Hello, World! is an argument
print('Hello',',', 'World','!') # it can take multiple arguments, four arguments have been passed
print(len('Hello, World!')) # it takes only one argument
```

Let us print and also find the length of the variables declared at the top:

**Example:**

```py
# Printing the values stored in the variables

print('First name:', first_name)
print('First name length:', len(first_name))
print('Middle name:', middle_name)
print('Middle name length:', len(middle_name))
print('Last name: ', last_name)
print('Last name length: ', len(last_name))
print('Country: ', country)
print('City: ', city)
print('Age: ', age)
print('Married: ', is_married)
print('Skills: ', skills)
print('Person information: ', person_info)
```

### Declaring Multiple Variable in a Line

Multiple variables can also be declared in one line:

**Example:**

```py
first_name, middle_name, last_name, country, age, is_married = 'Duong', 'Trung', 'Kien', 'Quang Ngai', 19, False

print(first_name, last_name, country, age, is_married)
print('First name:', first_name)
print('Last name: ', last_name)
print('Country: ', country)
print('Age: ', age)
print('Married: ', is_married)
```

Getting user input using the _input()_ built-in function. Let us assign the data we get from a user into first_name and age variables.
**Example:**

```py
first_name = input('What is your name: ')
age = input('How old are you? ')

print(first_name)
print(age)
```

## Data Types

There are several data types in Python. To identify the data type we use the _type_ built-in function. I would like to ask you to focus on understanding different data types very well. When it comes to programming, it is all about data types. I introduced data types at the very beginning and it comes again, because every topic is related to data types. We will cover data types in more detail in their respective sections.

## Checking Data types and Casting

- Check Data types: To check the data type of certain data/variable we use the _type_
  **Example:**

```py
# Different python data types
# Let's declare variables with various data types

first_name = 'Duong'     # str
middle_name = 'Trung'
last_name = 'Kien'       # str
country = 'Quang Ngai'         # str
city= 'Ho Chi Minh City'            # str
age = 19                   # int, it is not my real age, don't worry about it

# Printing out types
print(type('Duong'))     # str
print(type(first_name))     # str
print(type(10))             # int
print(type(3.14))           # float
print(type(1 + 1j))         # complex
print(type(True))           # bool
print(type([1, 2, 3, 4]))     # list
print(type({'name':'Kien','age':19, 'is_married': False}))    # dict
print(type((1,2)))                                              # tuple
print(type(zip([1,2],[3,4])))                                   # set
```

- Casting: Converting one data type to another data type. We use _int()_, _float()_, _str()_, _list_, _set_
  When we do arithmetic operations string numbers should be first converted to int or float otherwise it will return an error. If we concatenate a number with a string, the number should be first converted to a string. We will talk about concatenation in String section.

  **Example:**

```py
# int to float
num_int = 10
print('num_int',num_int)         # 10
num_float = float(num_int)
print('num_float:', num_float)   # 10.0

# float to int
gravity = 9.81
print(int(gravity))             # 9

# int to str
num_int = 10
print(num_int)                  # 10
num_str = str(num_int)
print(num_str)                  # '10'

# str to int or float
num_str = '10.6'
print('num_int', int(num_str))      # 10
print('num_float', float(num_str))  # 10.6

# str to list
first_name = 'Duong'
print(first_name)               # 'Duong'
first_name_to_list = list(first_name)
print(first_name_to_list)            # ['D', 'u', 'o', 'n', 'g']
```

## Numbers

Number data types in Python:

1. Integers: Integer(negative, zero and positive) numbers
   Example:
   ... -3, -2, -1, 0, 1, 2, 3 ...

2. Floating Point Numbers(Decimal numbers)
   Example:
   ... -3.5, -2.25, -1.0, 0.0, 1.1, 2.2, 3.5 ...

3. Complex Numbers
   Example:
   1 + j, 2 + 4j, 1 - 1j

🌕 You are awesome. You have just completed day 2 challenges and you are two steps ahead on your way to greatness. Now do some exercises for your brain and muscles.

## 💻 Exercises - Day_02

### Exercises: Level_01


1. Write a python comment saying 'Day 2: 30 Days of python programming'
``` py
# Day2: 30 Days of python programming
print("This is comment: Day2: 30 Days of python programming")
```
2. Declare a first name variable and assign a value to it
``` py
first_name = "Duong"
```
3. Declare a last name variable and assign a value to it
``` py
last_name = "Kien"
```
4. Declare a full name variable and assign a value to it
``` py
full_name = "Duong Trung Kien"
```
5. Declare a country variable and assign a value to it
``` py
country = "Quang Ngai"
```
6. Declare a city variable and assign a value to it
``` py
city = "Ho Chi Minh City"
```
7. Declare an age variable and assign a value to it
``` py
first_name = "Duong"
```
8. Declare a year variable and assign a value to it
``` py
year = 2022
```
9. Declare a variable is_married and assign a value to it
``` py
is_married = False
```
10. Declare a variable is_true and assign a value to it
``` py
is_true = True
```
11. Declare a variable is_light_on and assign a value to it
``` py
is_light_on = False
```
12. Declare multiple variable on one line
``` py
first_name, middle_name, last_name = "Duong", "Trung", "Kien"
```

### Exercises: Level 2

1. Check the data type of all your variables using type() built-in function
```py
print(type(full_name))  
print(type(country))   
print(type(city))        
print(type(year))        
print(type(is_married))
print(type(is_light_on))
print(type(is_true))
```
2. Using the _len()_ built-in function, find the length of your first name
```py
lenght = len(first_name)
print(lenght)
```
3. Compare the length of your first name and your last name
```py
length_first_name = len(first_name)
length_last_name = len(last_name)

if length_first_name > length_last_name:
    print("length first name > length last name")
elif length_first_name == length_last_name:
    print("length first name = length last name")
else:
    print("length first name < length last name")
```
5. Declare 5 as num_one and 4 as num_two
    1. Add num_one and num_two and assign the value to a variable total
    ``` py
    num_one = 1
    num_two = 2
    total = num_one + num_two
    ```
    3. Subtract num_two from num_one and assign the value to a variable diff
     ``` py
    num_one = 10
    num_two = 2
    subtract = num_one - num_two
    ```
    5. Multiply num_two and num_one and assign the value to a variable product
     ``` py
    num_one = 1
    num_two = 2
    multipli = num_one * num_two
    ```    
    7. Divide num_one by num_two and assign the value to a variable division
     ``` py
    num_one = 1
    num_two = 2
    divide = num_one / num_two
    ```
    9. Use modulus division to find num_two divided by num_one and assign the value to a variable remainder
    ```py
    num_one = 9
    num_two = 2
    modulus_division = num_one % num_two
    ```
    11. Calculate num_one to the power of num_two and assign the value to a variable exp
    ```py
    num_one = 9
    num_two = 2
    exp = num_one**num_two
    ```
    13. Find floor division of num_one by num_two and assign the value to a variable floor_division
    ```py
    num_one  = 9
    num_two = 2
    floor_division = num_one // num_two
    ```
6. The radius of a circle is 30 meters.
    1. Calculate the area of a circle and assign the value to a variable name of _area_of_circle_
    ```py
    radius_circle = 30
    PI = 3.1415926
    area_of_circle = PI * radius * radius
    ```
    3. Calculate the circumference of a circle and assign the value to a variable name of _circum_of_circle_
    ```py
    radius_circle = 30
    PI = 3.1415926
    circum_of_circle = 2 * PI * radius
    ```
    5. Take radius as user input and calculate the area.
    ```py
    # Calculate the area of circle
    PI = 3.1415926
    radius = float(input("Enter radius of circle: "))
    area_of_circle = PI * radius * radius
    print(f"Area of circle have radius {radius} is: {area_of_circle}")
    ```
7. Use the built-in input function to get first name, last name, country and age from a user and store the value to their corresponding variable names
```py
def get_information():
    first_name = input("Enter first name: ").capitalize()
    last_name = input("Enter last name: ").capitalize()
    country = input(f"Country of {last_name} is: ").title()
    age = int(input(f"{last_name}'s age is: "))
 ```
9. Run help('keywords') in Python shell or in your file to check for the Python reserved words or keywords
```py
help("class")
```

🎉 CONGRATULATIONS ! 🎉

[<< 01_Day](../01_Day_Introduction/01_Day_Introduction.py) | [03_Day >>](../03_Day_Operators/03_Day_Operators.md)
