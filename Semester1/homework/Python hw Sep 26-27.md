# Homework Sep 26

#  1. Write a program that takes three numbers and prints their sum. Every number is given on a separate line.

Example input:

```
2
3
6
```

Example Output:

```
11
```

# 2. Write a program that greets the person by printing the word "Hi" and your name. See the examples below.

Example input:

```
Alice
```

Example Output:

```
Hi Alice
```

# 3.Write a program that takes a number and print its square.

Example input:

```
5
```

Example Output:

```
The Square of your input is 25
```

# 4. Write a program that reads the length of the base and the height of a right-angled triangle and prints the area. Every number is given on a separate line.

Example input:

```
179
1534
```

Example Output:

```
137293.0
```

# 5. Apple sharing

`N` students take `K` apples and distribute them among each other evenly. The remaining (the undivisible) part remains in the basket. How many apples will each single student get? How many apples will remain in the basket?

The program reads the numbers `N` and `K`. It should print the two answers for the questions above.

```
6
50
```

```
8
2
```

```
N=int(input("pls in put the number of students:"))
K=int(input("pls input the number of apples:"))
print(K//N)
print(K%N)
```

# 6.Previous and next

Write a program that reads an integer number and prints its previous and next numbers. See the examples below for the exact format your answers should take. There shouldn't be a space before the period.

Remember that you can convert the numbers to strings using the function `str`.

```
179
```

```
The next number for the number 179 is 180.
The previous number for the number 179 is 178.
```

# 7.Two timestamps

A timestamp is three numbers: a number of hours, minutes and seconds. Given two timestamps, calculate how many seconds is between them. The moment of the first timestamp occurred before the moment of the second timestamp.

```
11
7
29
11
30
29
```

```

1380
```

# 8. School desks

A school decided to replace the desks in three classrooms. Each desk sits two students. Given the number of students in each class, print the smallest possible number of desks that can be purchased.

The program should read three integers: the number of students in each of the three classes, `a`, `b` and `c` respectively.

In the first test there are three groups. The first group has 20 students and thus needs 10 desks. The second group has 21 students, so they can get by with no fewer than 11 desks. 11 desks is also enough for the third group of 22 students. So we need 32 desks in total.

```
20
21
22
```

```
32
```

