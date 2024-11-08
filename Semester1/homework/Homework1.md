# Python Practice 1 

Task 1: Code Correction

What will be the output???

```
weather = "sunny"

if weather == "sunny":
    print("Wear sunglasses!")
else:
    print("Take an umbrella!")
```

Task 2: Your Mood Today

What will be the output???

```python
mood1 = input("How do you feel today? ")
if mood1 == "happy":
    print("That's great to hear!")
else: 
    print("I hope your day gets better!")
```

Task 3: Spotting indentation Errors

What will be the output???

```py
mood = "excited"

if mood == "excited":
    print("Yay! Let's have fun.")
else:
    print("Let's find something fun to do!")
```

# Python Comments and Multi Line Practice
Objective: Practice using single-line and multi-line comments

Task 1:  How to Create a poem and using single-line command to comment it?

```
  Python, in the realm of code you shine, 

  With simplicity an dgrace, you're truly devine

  Your sipmle code is like no other

  We were meant to work with one another

  If ever Python I should leave

  Just come along and follow me
```

Task 2 How to use Multi line Poem with  quotes??

```

Python you rock
you're the cream of the crop
I know one day you'll rise to the top
with victory in hand
your enemies can eat sand
Python your victory is close at hand

```

Task 3: How to Combining Single and Multi-line comments?

```
 Python, in the realm of code you shine, 

you're the cream of the crop

 Python Naming Convention Practice
```

# Python Naming Convention Practice

Task 1: Code Correction

```
pi_value = 1              Boolean             True or Flase?
user_age = 25               Int               True or Flase?
user_location = "New York"  String            True or Flase?
MAX_LIMIT = 1000            Number            True or Flase?
```

Python Data Types and type() Function

Task 1: Code Correction Please write the output for the print

```
variable_a = "Hello, World!" 
variable_b = 23             
variable_c = 3.14            
variable_d = True            

print(type(variable_a))
print(type(variable_b))
print(type(variable_c))
print(type(variable_d))
```

# Python Dynamic Typing Practice

Arithmetic Operations in Daily Life

Task1:Grocery Store Math, please print the output result.

```
eggs = 4.25
milk = 5
steak = 12

total_cost = eggs + milk + steak

print("Your total is", total_cost)
```

Task2: Bank interest, please print the output result.

```
savings_total = 1250
interest_rate = 0.25
apy = savings_total * interest_rate
print("Your total APY is", apy)

```

Task3: Area and Perimeter,  please print the output result.

```
rectangle_length = 4 
rectangle_width = 6
rectangle_area = rectangle_length * rectangle_width
rectangle_perimeter=rectangle_length*2 + rectangle_width * 2

print("The area of the rectangle is", rectangle_area)
print("The perimeter of the rectangle is", rectangle_perimeter)
```

# Understanding Assignments and Comparisons

Value Swapping

```
dragon_teeth = 460
dragon_teeth -=20
print(dragon_teeth)

dragon_scales = 500
dragon_scales += 50
print (dragon_scales)

are_teeth_and_scales_equal = dragon_teeth == dragon_scales
print(are_teeth_and_scales_equal)
```

# Perfect Square Checker

Give me an example and tell me the answer and output.

```
import math

def is_perfect_square(num):
    if num < 0:
        return False
    sqrt_num = math.isqrt(num)
    return sqrt_num * sqrt_num == num

num = int(input("Enter a number to see if it is a perfect square: "))
if is_perfect_square(num):
    print(num, "is a perfect square.")
else:
    print(num, "is not a perfect square."
```

# Exploring Logical Operations and Precedence

Task 1: Simple Logic Puzzles



```
has_teeth = True
has_scales = False
can_fly = True

is_dragon = has_teeth or has_scales or can_fly
print("Is it a dragon", is_dragon)

is_cat = has_teeth and has_scales and can_fly
print("Is it a pterodactyl?", is_cat)

is_dog = has_teeth and not has_scales
print("Is it a dog?", is_dog)
```

Task 2 Validating Calculations

Tell me the result for the print output

```
math_question1 = 3 + 2 * 9
print(math_question1)

math_question2 = (3 + 2) * 9
print(math_question2)

are_answers_equal = math_question1 == math_question2
print("Are the answers to the math question equal?", are_answers_equal)
```

Task 3 Mix and Match

What is the result for the following coding ?

```
result = (10 + 5 > 8) and (3 * 2 == 6) or (7 % 3 != 0)
"""
First, (10 + 5 > 8) evaluates to True because 10 + 5 equals 15, which is greater than 8.
Next, (3 * 2 == 6) evaluates to True because 3 * 2 equals 6.
Then, (7 % 3 != 0) evaluates to True because 7 % 3 equals 1, which is not equal to 0.
Finally, (True and True) or True evaluates to True because both conditions True and True and True are satisfied.
"""
print("Result:", result)
```