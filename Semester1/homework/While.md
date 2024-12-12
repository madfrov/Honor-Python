# While Loop Exercise

Answers:AADDA BBACB BADDA

1.what will be the output of the following python code?

```
i=5
while True:
	if i%8==0:
		break
	print(i,end=" ")
	i+=1
```

A. 5 6 7                 B. 5 6 7 8           C.no output          D. 6 7 8

2.what will be the output of the following python code?

```
i=2
while True:
	if i%3==0:
		break
	print(i,end=" ")
	i+=2
```

A. 2 4                 B. Error         C.2 3          D. 2 4 6 8 10 ...

3.what will be the output of the following python code?

```
i=1
while False:
	if i%2==0:
		break
	print(i,end=" ")
	i+=2
```

A. 1                 B.1 3 5 7 ...            C.1 2 3 4 . . .         D. none of the mentioned

4.what will be the output of the following python code?

```
x=1
while True:
 	if x==5:
 	break
	x+=1
	print(x)
```

A. True                B. False          C. None        D. none of the mentioned

5.what will be the output of the following python code?

```
i=5
while True:
	if i%9==0:
		break
	print(i,end=" ")
	i+=1
```

A. 5 6 7 8               B.5 6 7 8 9          C.error         D. 5 6 7 8 9 10....

6.what will be the output of the following python code?

```
i=1
while True:
	if i%2==0:
		break
	print(i,end=" ")
	i+=2
```

A. 1               B.1 3 5 7 9 11 ...         C.1 2 3 4 5 6 ...        D.1 2 

7.what will be the output of the following python code?

```
i=1
while True:
	if i%7==0:
		break
	print(i,end=" ")
	i+=1
```

A. 1 2 3 4 5 6 7               B.1 2 3 4 5 6         C.error       D. none of the mentioned

8.what will be the output of the following python code?

```
i=1
while True:
	if i%3==0:
		break
	print(i,end=" ")
	i+=1
```

A. 1 2               B.1 2 3          C.error       D. none of the mentioned

9.what will be the output of the following python code?

```
i=1
while i<5:
	print(i)
	i+=1
	if i == 3:
		break
else:
	print(0)
```

A. 0 1 2               B.0 1 2 0          C.1 2       D. none of the mentioned



10.what will be the output of the following python code?

```
i=0
while i<3:
	print(i)
	i+=1
else:
	print(0)
```

A. 0 1 2  3 0             B.0 1 2 0          C.0 1 2       D. Error

11.what will be the output of the following python code?

```
x="abcdef"
i="a"
while i in x[1:]:
	print(i,end="")
```

A. a a a a a  a             B.no output          C.a      D. Error

12.what will be the output of the following python code?

```
x="abcdef"
i="a"
while i in x:
	x=x[:-1]
	print(i,end="")
```

A. a a a a a a             B.a a a a a          C.i i i i i i       D. none of the mentioned

13.what will be the output of the following python code?

```
x="abcdef"
i="i"
while i in x:
	print(i,end="")
```

A. a b c d e f             B.i i i i i i ...          C.abcdef     D.no output

14.what will be the output of the following python code?

```
x="abcdef"
i="a"
while i in x:
	print(i,end="")
```

A.error            B. a b c d e f        C.abcdef     D.i i i i i i . . .

15.what will be the output of the following python code?

```
x="abcdef"
while i in x:
	print(i,end="")
```

A.error            B. a b c d e f        C.abcdef     D.i i i i i i . . .

FRQ1: use of the while loop to determine the number of digits of an integer n

for example input: 100

Output should be : 3

```
n = int(input())
length = 0
while n > 0:
    n //= 10  # this is equivalent to n = n // 10
    length += 1
print(length)  # 4

```

FRQ2: List of squares

For a given integer N, print all the squares of integer numbers where the square is less than or equal to N, in ascending order.

sample input: 50     sample out: 1 4 9 16 25 36 49

sample input: 10     sample out: 1 4 9

```
N = int(input())
i = 1
while i * i <= N:
    print(i * i, end=" ")
    i += 1
```

FRQ3:Least divisor

Given an integer not less than 2.

 Print its smallest integer divisor greater than 

sample input:15     sample out: 3

sample input: 55     sample out: 5

```
n = int(input())
i = 2
while i <= n:
    if n % i == 0:
        print(i)
        break
    i += 1
```

FRQ 4:The power of two

For a given integer **N**, find the greatest integer **x** where 2^x is less than or equal to **N**. Print the exponent value and the result of the expression 2^x.

Don't use the operation `**`. 

```
N = int(input())
x = 0
power=2 
while power <= N:
    x += 1
    power*=2
x -= 1
power//=2
print(x, power)

```

Ex5.Morning jog

As a future athlete you just started your practice for an upcoming event. Given that on the first day you run *x* miles, and by the event you must be able to run *y* miles.

Calculate the number of days required for you to finally reach the required distance for the event, if you increases your distance each day by 10% from the previous day.

Print one integer representing the number of days to reach the required distance.

sample input

```
10
100
```

sample output

```
26
```

sample input2

```
1
1000
```

sample output2

```
74
```

```
x = float(input())
y = float(input())
days = 1
while x < y:
    x *= 1.10
    days += 1
print(days)
```

