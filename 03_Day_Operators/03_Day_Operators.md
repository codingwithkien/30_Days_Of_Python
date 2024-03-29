<div align="center">
  <h1> 30_Days_Of_Python: 03_Day_Operators</h1>




<sub>Author:
<a href="https://www.facebook.com/duongtrungkien062003"> Duong Trung Kien</a><br>
<small>October, 2022</small>
</sub>
  
 
</div>

[<< 02_Day](../02_Day_Variable/02_Day_Variable.md) | [04_Day >>](../04_Day_Strings/04_Day_Strings.md)

![30DaysOfPython](https://camo.githubusercontent.com/59a720eaa51a6bbc45ba76313bf53a4f2c84dde994c947809a49b41f3c828ef2/68747470733a2f2f7374617469632e636f64696e67666f72656e7472657072656e657572732e636f6d2f6d656469612f70726f6a656374732f33302d646179732d707974686f6e2d33382f696d616765732f73686172652f33305f446179735f6f665f507974686f6e5f2d5f53686172652e6a7067)
- [📘 03_Day](#-day-3)
  - [Boolean](#boolean)
  - [Operators](#operators)
    - [Assignment Operators](#assignment-operators)
    - [Arithmetic Operators:](#arithmetic-operators)
    - [Comparison Operators](#comparison-operators)
    - [Logical Operators](#logical-operators)
  - [💻 Exercises - Day_03](#-exercises---day-3)

# 📘 03_Day

## Boolean

A boolean data type represents one of the two values: _True_ or _False_. The use of these data types will be clear once we start using the comparison operator. The first letter **T** for True and **F** for False should be capital unlike JavaScript.
**Example: Boolean Values**

```py
print(True)
print(False)
```

## Operators

Python language supports several types of operators. In this section, we will focus on few of them.

### Assignment Operators

Assignment operators are used to assign values to variables. Let us take = as an example. Equal sign in mathematics shows that two values are equal, however in Python it means we are storing a value in a certain variable and we call it assignment or a assigning value to a variable. The table below shows the different types of python assignment operators, taken from [w3school](https://www.w3schools.com/python/python_operators.asp).

![Assignment Operators](https://i.postimg.cc/wTLQJWRv/Capture-Assignment.png)

### Arithmetic Operators:

- Addition (+): a + b
- Subtraction (-): a - b
- Multiplication (*): a * b
- Division (/): a / b
- Modulus (%): a % b
- Floor division (//): a // b
- Exponentiation (**): a ** b

![Arithmetic Operators](https://github.com/Asabeneh/30-Days-Of-Python/raw/master/images/arithmetic_operators.png)

**Example: Integers**

```py
# Arithmetic Operations in Python
# Integers

print('Addition: ', 1 + 2)        # 3
print('Subtraction: ', 2 - 1)     # 1
print('Multiplication: ', 2 * 3)  # 6
print ('Division: ', 4 / 2)       # 2.0  Division in Python gives floating number
print('Division: ', 6 / 2)        # 3.0         
print('Division: ', 7 / 2)        # 3.5
print('Division without the remainder: ', 7 // 2)   # 3,  Gives without the floating number or without the remaining
print ('Division without the remainder: ',7 // 3)   # 2
print('Modulus: ', 3 % 2)         # 1, Gives the remainder
print('Exponentiation: ', 2 ** 3) # 9 it means 2 * 2 * 2
```

**Example: Floats**

```py
# Floating numbers
print('Floating Point Number, PI', 3.14)
print('Floating Point Number, gravity', 9.81)
```

**Example: Complex numbers**

```py
# Complex numbers
print('Complex number: ', 1 + 1j)
print('Multiplying complex numbers: ',(1 + 1j) * (1 - 1j))
```

Let's declare a variable and assign a number data type. I am going to use single character variable but remember do not develop a habit of declaring such types of variables. Variable names should be all the time mnemonic.

**Example:**

```python
# Declaring the variable at the top first

a = 3 # a is a variable name and 3 is an integer data type
b = 2 # b is a variable name and 3 is an integer data type

# Arithmetic operations and assigning the result to a variable
total = a + b
diff = a - b
product = a * b
division = a / b
remainder = a % b
floor_division = a // b
exponential = a ** b

# I should have used sum instead of total but sum is a built-in function - try to avoid overriding built-in functions
print(total) # if you do not label your print with some string, you never know where the result is coming from
print('a + b = ', total)
print('a - b = ', diff)
print('a * b = ', product)
print('a / b = ', division)
print('a % b = ', remainder)
print('a // b = ', floor_division)
print('a ** b = ', exponential)
```

**Example:**

```py
print('== Addition, Subtraction, Multiplication, Division, Modulus ==')

# Declaring values and organizing them together
num_one = 3
num_two = 4

# Arithmetic operations
total = num_one + num_two
diff = num_two - num_one
product = num_one * num_two
div = num_two / num_one
remainder = num_two % num_one

# Printing values with label
print('total: ', total)
print('difference: ', diff)
print('product: ', product)
print('division: ', div)
print('remainder: ', remainder)
```

Let us start start connecting the dots and start making use of what we already know to calculate (area, volume,density,  weight, perimeter, distance, force).

**Example:**

```py
# Calculating area of a circle
radius = 10                                 # radius of a circle
area_of_circle = 3.14 * radius ** 2         # two * sign means exponent or power
print('Area of a circle:', area_of_circle)

# Calculating area of a rectangle
length = 10
width = 20
area_of_rectangle = length * width
print('Area of rectangle:', area_of_rectangle)

# Calculating a weight of an object
mass = 75
gravity = 9.81
weight = mass * gravity
print(weight, 'N')                         # Adding unit to the weight

# Calculate the density of a liquid
mass = 75 # in Kg
volume = 0.075 # in cubic meter
density = mass / volume # 1000 Kg/m^3

```

### Comparison Operators

In programming we compare values, we use comparison operators to compare two values. We check if a value is greater or less or equal to other value. The following table shows Python comparison operators which was taken from [w3shool](https://www.w3schools.com/python/python_operators.asp).

<table class="ws-table-all notranslate">
<tbody><tr>
<th style="width:100%">Operator</th>
<th style="width:100%">Name</th>
<th style="width:100%">Example</th>
</tr>
<tr>
<td>==</td>
<td>Equal</td>
<td>x == y</td>
</tr>
<tr>
<td>!=</td>
<td>Not equal</td>
<td>x != y</td>
</tr>
<tr>
<td>&gt;</td>
<td>Greater than</td>
<td>x &gt; y</td>
</tr>
<tr>
<td>&lt;</td>
<td>Less than</td>
<td>x &lt; y</td>
</tr>
  <tr>
<td>&gt;=</td>
<td>Greater than or equal to</td>
<td>x &gt;= y</td>
  </tr>
<tr>
<td>&lt;=</td>
<td>Less than or equal to</td>
<td>x &lt;= y</td>
</tr>
</tbody></table>

**Example: Comparison Operators**

```py
print(3 > 2)     # True, because 3 is greater than 2
print(3 >= 2)    # True, because 3 is greater than 2
print(3 < 2)     # False,  because 3 is greater than 2
print(2 < 3)     # True, because 2 is less than 3
print(2 <= 3)    # True, because 2 is less than 3
print(3 == 2)    # False, because 3 is not equal to 2
print(3 != 2)    # True, because 3 is not equal to 2
print(len('mango') == len('avocado'))  # False
print(len('mango') != len('avocado'))  # True
print(len('mango') < len('avocado'))   # True
print(len('milk') != len('meat'))      # False
print(len('milk') == len('meat'))      # True
print(len('tomato') == len('potato'))  # True
print(len('python') > len('dragon'))   # False


# Comparing something gives either a True or False

print('True == True: ', True == True)
print('True == False: ', True == False)
print('False == False:', False == False)
```

In addition to the above comparison operator Python uses:

- _is_: Returns true if both variables are the same object(x is y)
- _is not_: Returns true if both variables are not the same object(x is not y)
- _in_: Returns True if the queried list contains a certain item(x in y)
- _not in_: Returns True if the queried list doesn't have a certain item(x in y)

```py
print('1 is 1', 1 is 1)                   # True - because the data values are the same
print('1 is not 2', 1 is not 2)           # True - because 1 is not 2
print('A in Asabeneh', 'A' in 'Asabeneh') # True - A found in the string
print('B in Asabeneh', 'B' in 'Asabeneh') # False - there is no uppercase B
print('coding' in 'coding for all') # True - because coding for all has the word coding
print('a in an:', 'a' in 'an')      # True
print('4 is 2 ** 2:', 4 is 2 ** 2)   # True
```

### Logical Operators

Unlike other programming languages python uses keywords _and_, _or_ and _not_ for logical operators. Logical operators are used to combine conditional statements:

![Logical Operators](https://github.com/Asabeneh/30-Days-Of-Python/raw/master/images/comparison_operators.png)

```py
print(3 > 2 and 4 > 3) # True - because both statements are true
print(3 > 2 and 4 < 3) # False - because the second statement is false
print(3 < 2 and 4 < 3) # False - because both statements are false
print('True and True: ', True and True)
print(3 > 2 or 4 > 3)  # True - because both statements are true
print(3 > 2 or 4 < 3)  # True - because one of the statements is true
print(3 < 2 or 4 < 3)  # False - because both statements are false
print('True or False:', True or False)
print(not 3 > 2)     # False - because 3 > 2 is true, then not True gives False
print(not True)      # False - Negation, the not operator turns true to false
print(not False)     # True
print(not not True)  # True
print(not not False) # False

```

🌕 You have boundless energy. You have just completed day 3 challenges and you are three steps ahead on your way to greatness. Now do some exercises for your brain and your muscles.

## 💻 Exercises - Day_03

1. Declare your age as integer variable
```py
age = 19
```
2. Declare your height as a float variable
```py
height = 1.69
```
3. Declare a variable that store a complex number
```py
complex = 1 + 2j
```
4. Write a script that prompts the user to enter base and height of the triangle and calculate an area of this triangle (area = 0.5 x b x h).

```py
while True:
    enter_base = float(input("Enter base of the triangle: "))
    enter_height = float(input("Enter height of the triangle: "))
    area_triangle = 0.5 * enter_base * enter_height
    print(f"Area of the triangle is {area_triangle}")
        
    print("-----------------")
    exit_calculus = input("Do you want to exit? (Y / N)" )
    print("-----------------")

    if exit_calculus == "Y":
        break
```

5. Write a script that prompts the user to enter side a, side b, and side c of the triangle. Calculate the perimeter of the triangle (perimeter = a + b + c).

```py
# Enter side a: 5
# Enter side b: 4
# Enter side c: 3
# The perimeter of the triangle is 12

side_a = int(input("Enter side a: "))
side_b = int(input("Enter side b: "))
side_c = int(input("Enter side c: "))

triangle = side_a + side_b + size_c
print(f"The perimeter of the triangle is {triangle}")
```

6. Get length and width of a rectangle using prompt. Calculate its area (area = length x width) and perimeter (perimeter = 2 x (length + width))
```py
length_rectangle = int(input("Enter length of a recangle: "))
width_rectangle = int(input("Enter width of a recangle: "))

area_of_rectangle = length_rectangle * width_of_rectangle
print(f"Area of rectangle is {area_of_rectangle}")

perimeter_of_rectangle = (length_rectangle + width_of_rectangle) * 2
print(f"Perimeter of rectangle is {perimeter_of_rectangle}")

```
8. Get radius of a circle using prompt. Calculate the area (area = pi x r x r) and circumference (c = 2 x pi x r) where pi = 3.14.
```py
PI = 3.14
radius = float(input("Enter the radius of the circle: "))

area_circle = PI * radius ** 2
circumference = 2 * PI * radius

print("Area of the circle is: {}".format(area_circle))
print("Circumference is: {}".format(circumference))
```
10. Calculate the slope, x-intercept and y-intercept of y = 2x -2
11. Slope is (m = y2-y1/x2-x1). Find the slope and [Euclidean distance](https://en.wikipedia.org/wiki/Euclidean_distance#:~:text=In%20mathematics%2C%20the%20Euclidean%20distance,being%20called%20the%20Pythagorean%20distance.) between point (2, 2) and point (6,10) 
12. Compare the slopes in tasks 8 and 9.
13. Calculate the value of y (y = x^2 + 6x + 9). Try to use different x values and figure out at what x value y is going to be 0.
14. Find the length of 'python' and 'dragon' and make a falsy comparison statement.
15. Use _and_ operator to check if 'on' is found in both 'python' and 'dragon'
16. _I hope this course is not full of jargon_. Use _in_ operator to check if _jargon_ is in the sentence.
17. There is no 'on' in both dragon and python
18. Find the length of the text _python_ and convert the value to float and convert it to string
19. Even numbers are divisible by 2 and the remainder is zero. How do you check if a number is even or not using python?
20. Check if the floor division of 7 by 3 is equal to the int converted value of 2.7.
21. Check if type of '10' is equal to type of 10
22. Check if int('9.8') is equal to 10
23. Writ a script that prompts the user to enter hours and rate per hour. Calculate pay of the person?

```py
Enter hours: 40
Enter rate per hour: 28
Your weekly earning is 1120
```

22. Write a script that prompts the user to enter number of years. Calculate the number of seconds a person can live. Assume a person can live hundred years

```py
Enter number of years you have lived: 100
You have lived for 3153600000 seconds.
```

23. Write a Python script that displays the following table

```py
1 1 1 1 1
2 1 2 4 8
3 1 3 9 27
4 1 4 16 64
5 1 5 25 125
```

🎉 CONGRATULATIONS ! 🎉

[<< 02_Day](../02_Day_Variable/02_Day_Variable.md) | [04_Day >>](../04_Day_Strings/04_Day_Strings.md)
