# Python Review 3

1. Binary to Decimal Convert the binary number 1101 to its decimal equivalent. 

   A. 13     B. 25     C. 29     D. 30

2. Decimal to Binary Convert the decimal number 23 to its binary equivalent. 

   A. 10111     B. 11011     C. 11101     D. 10011

3. Hexadecimal to Decimal Convert the hexadecimal number 2F to its decimal equivalent. 

   A. 47     B. 55     C. 63     D. 46

4. Decimal to Hexadecimal Convert the decimal number 255 to its hexadecimal equivalent.

    A. FF     B. FE    C. FD     D. FC

5. Binary to Hexadecimal Convert the binary number 11011101 to its hexadecimal equivalent. 

   A. D5     B. CD     C. DD     D. DC

6. Hexadecimal to Binary Convert the hexadecimal number 7A to its binary equivalent.

    A. 1111010     B. 1110101     C. 1101011     D. 1101101

   7.Which of the following is NOT a Python reserved word?

​                 A. def B. class C. function D. return

​                 8. Which of the following is NOT a Python reserved word?

​                 A. while B. for C. loop D. break

9. Which of the following is NOT a Python-reserved word?

​                A. import B. from C. include D. as

10. What happens when '3' == 3 is executed?

​        A. False 	B. True 	C. ValueError occurs  D. TypeError occurs

11.What is the output of the following code :

```
a = False
b = False
c = True

if not a or b:
    print("a")
elif not a or not b and c:
    print("b")
elif not a or b or not b and a:
    print("c")
else:
    print("d")
```

A. a  	B.  b  		C. c 		 D. d

12.What is the output of the following code :

```
x = 15
y = 3
if x % y > 0:
    print("Remainder")
elif x // y == 0:
    print("Division Zero")
else:
    print("No Remainder")
```

A. Remainder     B. Division Zero     C. No Remainder     D. The 

13.What is the output of the following code :

```
m = 20
n = 4
if m % n == 0:
    print("Divisible")
elif m > n * 5:
    print("Five Times")
elif m < n:
    print("Less Than")
else:
    print("Other Cases")
```

A. Divisible     B. Five Times     C. Less Than     D. Other Cases

14.What will be the execution result of the above code? 

```
p = 10
q = 3
flag1 = False
flag2 = False
if p > q:
    if p % q >= 2:
        flag1 = True
        p -= q
    else:
        p += q
if p < q:
    if q % p >= 2:
        flag2 = True
        p -= q
    else:
        p += q
```

A. flag1=True, flag2=True, p=1     B. flag1=False, flag2=False, p=13 

C. flag1=False, flag2=True, p=1     D. flag1=False, flag2=False, p=13

15.What will be the execution result of the above code? 

```
r = 8
s = 2
flag3 = False
flag4 = False
if r > s:
    if r % s == 0:
        flag3 = True
        r -= s
    else:
        r += s
if r < s:
    if s % r == 0:
        flag4 = True
        r -= s
    else:
        r += s
```

A. flag3=True, flag4=True, r=0      B. flag3=True, flag4=False, r=6 

C. flag3=False, flag4=True, r=0     D. flag3=False, flag4=False, r=10

16.What will be the execution result of the above code? 

```
if (5 > 3) and not (2 > 1):
     print("first")
elif (4 < 1) or (3 > 2):
     print("second")
else:
     print("third")
```

A. first     B. second     C. third     D. no output

17.What will be the execution result of the above code? 

```
 if (10 == 10) and (10 != 11):
     print("hello")
 elif (False or True) and not (5 > 10):
     print("world")
 else:
     print("!")
```

 A. hello     B. world     C. !     D. 无输出

1.Please output a three-digit integer, the number reversed.

For example: integer 123, the reverse is 321, integer 118, the reverse is 811, integer 700, the reverse is 7.

Sample：

Input:

169

Output:

961





