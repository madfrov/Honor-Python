# Question 1: Write a program that prompts the user for an integer and outputs “This is an even number” If the number entered is even, otherwise outputs “This is an odd number”.

```
num = int(input("请输入一个整数："))

if num % 2 == 0:
    print("这是一个偶数")
else:
    print("这是一个奇数")
```

# Question 2: Write a program that prompts the user for an age and outputs “You are an adult” If the age is greater than or equal to 18, otherwise outputs “You are underage”.

```
age = int(input("请输入您的年龄："))

if age >= 18:
    print("您已成年")
else:
    print("您未成年")
```

# Question 3: Write a program that prompts the user to enter two integers and outputs the larger of the two numbers.

```
num1 = int(input("请输入第一个整数："))
num2 = int(input("请输入第二个整数："))

if num1 > num2:
    print("较大的数是",num1)
elif num2 > num1:
    print("较大的数是",num2)
else:
    print("两个数相等")
```

# HW： 

# Question 1: Write a program that outputs the corresponding grade based on the user's input score. A score of 90 and above is 'A', 80-89 is 'B', 70-79 is 'C', 60-69 is 'D', and below 60 is 'E'.

```
score = int(input("Enter your score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: E")
```



# Question 2: Write a program that prompts the user to enter a year and determines if it is a leap year. The leap year rule is: divisible by 4 but not by 100, or divisible by 400.

To determine if a year is a leap year, we need to follow the rules:

1. If the year is divisible by 4, it could be a leap year.
2. However, if the year is divisible by 100, it is not a leap year unless:
   - It is also divisible by 400, which is a leap year.

Let's apply these rules to the year 1000:

1. 1000 is divisible by 4 and at the same time 1000 is divisible by 100.
2. 1000 is not divisible by 400.

```
year = int(input("Enter a year: "))

if (year % 4 == 0 and year % 100 != 0) or year % 400 == 0:
    print(year,"is a leap year")
else:
    print(year, "is not a leap year")
```

# Question 3: Write a program that accepts three integers from the user and outputs the maximum of the three numbers.

```
num1 = int(input("Enter the first integer: "))
num2 = int(input("Enter the second integer: "))
num3 = int(input("Enter the third integer: "))

max_num = num1

if num2 > max_num:
    max_num = num2
if num3 > max_num:
    max_num = num3

print(f"The maximum number is: ",max_num)
```

 **Question 4: FizzBuzz** Write a program that prints numbers from 1 to 100. But for multiples of 3, print "Fizz" instead of numbers, for multiples of 5, print "Buzz" instead of numbers, and for numbers that are multiples of both 3 and 5, print "FizzBuzz".

```
for i in range(1, 101):

	if i % 3 == 0 and i % 5 == 0:

		print("FizzBuzz")

	elif i % 3 == 0:

		print("Fizz")

	elif i % 5 == 0:

		print("Buzz")

	else:

		print(i)
```







