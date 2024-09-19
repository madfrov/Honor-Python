# IF statement

![image-20240918152739202](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918152739202.png)

![image-20240918153012769](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918153012769.png)

![image-20240918153119792](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918153119792.png)

# Question 1: Write a program that prompts the user for an integer and outputs “This is an even number” If the number entered is even, otherwise outputs “This is an odd number”.

Answers
```python
num = 10
if num % 2 == 0:
    print("This is an even number.")
else:
    print("This is an odd number")
```

# Question 2: Write a program that prompts the user for an age and outputs “You are an adult” if the age is greater than or equal to 18, otherwise outputs “You are underage”.

Answers:
```python
age = int(input("Please enter your age:"))
if age >= 18:
    print("You are an adult")
else:
    print("You are underage")
```

![image-20240918153448412](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918153448412.png)

![image-20240918153914365](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918153914365.png)

![image-20240918154859265](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918154859265.png)

![image-20240918154927308](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918154927308.png)

![image-20240918155013610](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918155013610.png)

![image-20240918155433152](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918155433152.png)

![image-20240918220436266](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918220436266.png)

![image-20240918220536288](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918220536288.png)

![image-20240918220627981](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918220627981.png)

![image-20240918220706600](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918220706600.png)

![image-20240918221009536](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918221009536.png)

![image-20240918221147596](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240918221147596.png)

# Question 3: Write a program that prompts the user to enter two integers and outputs the larger of the two numbers.

Answer three:

```python
num1 = int(input("Please enter the first integer:"))
num2 = int(input("Please enter the second integer:"))
if num1 > num2:
    print("The larger number is:",num1)
elif num2 > num1:
    print("The larger number is:",num2)
else: 
    print("The two numbers are equal.")
```

HW：

Question 1: Write a program that outputs the corresponding grade based on the user's input score. A score of 90 and above is 'A', 80-89 is 'B', 70-79 is 'C', 60-69 is 'D', and below 60 is 'E'.

Question 2: Write a program that prompts the user to enter a year and determines if it is a leap year. The leap year rule is: divisible by 4 but not by 100, or divisible by 400.

Question 3: Write a program that accepts three integers from the user and outputs the maximum of the three numbers.

**Question 4: FizzBuzz** Write a program that prints numbers from 1 to 100. But for multiples of 3, print "Fizz" instead of numbers, for multiples of 5, print "Buzz" instead of numbers, and for numbers that are multiples of both 3 and 5, print "FizzBuzz".