

# Data Conversion

Understanding the significance and use of the various binary systems can help us to apply them better:

### Decimal
- **Use**: Everyday counting and calculation by human beings.
- **Significance**: The most intuitive numbering system, based on 10 digits (0-9).

### Binary
- **Use**: The basis of computer systems.
- **Significance** : Simple hardware implementation, suitable for electronic circuits (on/off).

### Octal 
- **Use**: Early computer systems and certain programming scenarios.
- **Significance** : Simplified binary representation, three binary bits are synthesized into one octal bit.

### Hexadecimal 
- **Use**: memory addresses, color coding, machine codes.
- **Significance**: Simplified binary representation, four binary bits are synthesized into one hexadecimal bit, easy to read and use.

Each hexadecimal system has its own unique advantages and significance in specific application scenarios.

# Q：What is  2 to the power of 0?

## Meaning of binary:

The representation of data in a computer, ultimately in binary form

## Advantage:
The main reason for this is related to the hardware of the computer, the logic circuits that make up the computer system have only two states, (on and off), and only two possibilities of occurrence.

When our computers are disturbed, the state of the logic circuits (on and off) can still be clearly recognized.

Therefore, in specific system implementations, the binary representation of data has the advantage of being highly resistant to interference.

In contrast, the decimal design of the state circuit has ten states of the circuit, the specific system implementation will become very responsible, in the judgment of the possibility of errors in the chances will be greatly increased.

## Disadvantage:
Lengthy to write, inconvenient to express when interacting with human beings (to be precise, human beings are prone to recording errors)

For example, the int type takes up 4 bytes and is 32-bit. For example, 100, expressed as a binary number of type int would be: 　　

0000 0000 0000 0000 0000 0110 0100 　　

No one likes to think or manipulate with such long numbers.

Therefore, C and C++ do not provide a way to write binary numbers directly in code.

Therefore, hexadecimal and octal were introduced. Because, the larger the number, the shorter the length of the number.
# The meaning of decimal:
One of the designations of high-level languages is that they can be read better. So in the use of high-level language, for programming, we commonly used or decimal system. After all, it is a high-level language. 　　

For example: int a = 100,b = 99.

Drawbacks - prone to computational problems
The application of number division and inexhaustibility is of great significance, and the advantage of a number system with a high rate of division is undoubtedly higher. Research in number theory has shown that division and inexhaustibility are related to the number of divisors and the number of progressions.

Among the current decimal numbers, those whose divisors can be written as 2^p×5^q are all divisible by all decimal integers and finite decimals.

The higher the number of divisors, the higher the rate of division is not inevitable, there are also special characteristics, for example, in the civilian use of numbers within 100, the hexadecimal number of the rate of division is higher, all can be written as 2 ^ p × 3 ^ q hexadecimal number, can be divided by all the hexadecimal integer and finite fractional numbers.

This means that civilian numbers are actually hexadecimal numbers are more advantageous.

Flaw - With decimal, why develop octal and hexadecimal for computers?
Because computers use binary at the bottom, and converting binary to decimal is cumbersome and not intuitive enough.

However, it is very easy to convert binary to octal or hexadecimal. 3-bit binary can be converted to 1-bit octal, and 4-bit binary can be converted to 1-bit hexadecimal.

# The significance of octal:
Why 16 or 8 and not others, such as 9 or 20?
2, 8, and 16 are the 1st, 3rd, and 4th power of 2, respectively. This makes it very straightforward to convert between the three systems.

The octal or hexadecimal systems shorten the binary numbers, but maintain the expressive characteristics of the binary numbers.

Advantages:
Two advantages of octal:

Easy parse from character (direct char minus 0x30 is the single digit value when using ASCII), easy conversion to string (single digit value plus 0x30 is the ASCII value of the corresponding character).

easy to parse from string (just shift and add...)

For example, you encounter an octal number, to convert it to, say, int type, constantly read the character, minus 0x30, plus the result of the existing results of the left shift of 3-bit results on the line, the bold font here than the use of the results of the decimal faster...

Binary data is too large, decimal calculation is too troublesome, hexadecimal parsing is too troublesome, octal is just right here.

Applications:
Linux file permissions (e.g. this number in chmod 644) (of course this has to do with how file permissions are constructed, not so much with parse as mentioned above)

The way data is stored in certain file structures (e.g. the size and time of a file is recorded in octal when tarballing).

## Commonly used ranges of the progression and their symbolic modifiers:

### Binary (B) ---->0 ~ 1

### Octal (O) ---->0 ~ 7

### Decimal (D) ---->0 ~ 9

## In hexadecimal, letters are used to represent values greater than 9:

A = 10
B = 11
C = 12
D = 13
E = 14
F = 15

# I. Decimal conversion to binary

Integer conversion
1, decimal to binary
Divide by 2 to take the balance of the reverse output
(1) decimal to binary conversion principle: divided by 2, take the remainder in reverse, until the quotient is 0 termination

(2) specific method:
A decimal number divided by 2 to get the integer part of the retention, as the second divided by 2 when the divisor, get the remainder of the sequential note, repeat the above steps until the integer part of the end of 0, the remainder of all the final reverse order output, the decimal corresponding to the binary number.

## Example 1: 9 (decimal) → 1001 (binary)

![image-20240905155234791](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240905155234791.png)

The final result is: 9 (10) = 1001 (2)

## Example 2: 42 (decimal) → 101010 (binary)

![image-20240905162242690](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240905162242690.png)

The final result is: 42 (10) = 101010 (2)

Here are some decimal to binary conversion topics:

### Decimal to binary.

1. 18
2. 45
3. 63
4. 100
5. 255

### Binary to decimal

1. 1010
2. 11011
3. 111111
4. 1000001
5. 11001011

```
 十进制转二进制

1. 18 → 10010
2. 45 → 101101
3. 63 → 111111
4. 100 → 1100100
5. 255 → 11111111

 二进制转十进制

1. 1010 → 10
2. 11011 → 27
3. 111111 → 63
4. 1000001 → 65
5. 11001011 → 203
```

![image-20240905195008690](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240905195008690.png)

![image-20240905195027657](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240905195027657.png)

# 2、Decimal to octal
Divide by 8 and take the remainder in reverse order output
(1) Conversion principle: divide by 8, reverse the remainder until the quotient is 0 termination.

(2) specific steps with the same binary
Example: 796 (decimal) → 1434 (octal)

![image-20240905195700565](/Users/huangzizhuang/Library/Application Support/typora-user-images/image-20240905195700565.png)

### Octal to decimal

## Binary to Octal, three-in-one method, every three binary digits synthesized into one octal number

#### Binary Number:  1011 1110

​                =(010)+(111)+(110)

​                = 2 + 7 + 6

​               = 276



## Exercise  2

## Octal to Decimal
17 → 15
45 → 37
123 → 83

## Decimal to octal
25 → 31
64 → 100
156 → 234

Here are 10 octal to decimal and decimal to octal examples and answers:

### Octal to decimal.

1. Octal:  17  
   **Decimal: ** \( 1 \times 8^1 + 7 \times 8^0 = 8 + 7 = 15 \)

2. **Octal: ** 23  
   **Decimal:** \( 2 \times 8^1 + 3 \times 8^0 = 16 + 3 = 19 \)

3. **Octal: ** 45  
   **Decimal:** \( 4 \times 8^1 + 5 \times 8^0 = 32 + 5 = 37 \)

4. **Octal: ** 61  
   **Decimal:** \( 6 \times 8^1 + 1 \times 8^0 = 48 + 1 = 49 \)

5. **Octal: ** 127  
   **Decimal:** \( 1 \times 8^2 + 2 \times 8^1 + 7 \times 8^0 = 64 + 16 + 7 = 87 \)

### Decimal to octal.

6. **Decimal: ** 15  
   **Octal: ** \( 15 \div 8 = 1 \) 余 \( 7 \) → **Results:** 17

7. **Decimal: ** 19  
   ** Octal: ** \( 19 \div 8 = 2 \) remainder \( 3 \) → **Results:** 23

8. **Decimal: ** 37  
   ** Octal: ** \( 37 \div 8 = 4 \) remainder \( 5 \) → **Results:** 45

9. **Decimal: ** 49  
   ** Octal: ** \( 49 \div 8 = 6 \) remainder \( 1 \) → **Results:** 61

10. **Decimal: ** 87  
    **Octal: ** \( 87 \div 8 = 10 \) remainder \( 7 \) → \( 10 \div 8 = 1 \) remainder \( 2 \) → **Results:** 127

### Summary
- Octal to decimal is calculated by multiplying each octal bit by the corresponding power of eight to sum.
- Decimal to octal is calculated by continually dividing by eight and recording the remainder.

### Octal to binary.

1. ** Octal: ** 12  
   **Binary:** \( 1 \ ) → `001`  
   \( 2 \) → `010`  
   **Results:** `001010`

2. **Octal: ** 27  
   **Binary:** \( 2 \) → `010`  
   \( 7 \ ) → `111`  
   **Results:** `010111`

3. **Octal: ** 34  
   **Binary:** \( 3 \) → `011`  
   \( 4 \ ) → `100`  
   **Results:** `011100`

4. **Octal: ** 56  
   **Binary:** \( 5 \) → `101`  
   \( 6 \) → `110`  
   **Results:** `101110`

5. **Octal: ** 72  
   **Binary:** \( 7 \) → `111`  
   \( 2 \) → `010`  
   **Results:** `111010`

### Binary to octal

1. **Binary: ** `101010`  
   **Octal: ** \( 101 \) → 5, \( 010 \) → 2  
   **Results:** 52

2. **Binary: ** `111111`  
   **Octal: ** \( 111 \) → 7, \( 111 \) → 7  
   **Results:** 77

3. **Binary:** `110100`  
   **Octal: ** \( 110 \) → 6, \( 100 \) → 4  
   **Results:** 64

4. **Binary:** `100110`  
   **Octal: ** \( 100 \) → 4, \( 110 \) → 6  
   **Results:** 46

5. **Binary: ** `111010`  
   **Octal: ** \( 111 \) → 7, \( 010 \) → 2  
   **Results:** 72

### Summary
- When converting from octal to binary, each octal bit is converted to three bits of binary.
- When converting binary to octal, the binary number is converted to the corresponding octal bit by grouping each three bits from right to left.

- Decimal is mainly used in everyday life, while binary, octal, and hexadecimal are mainly used in electronics.

Binary is the most direct language for digital circuits and processors, while octal and hexadecimal are used because of their convenience in conversion and recording.

Nowadays, hexadecimal is more commonly used for storage and memorization, while octal is less commonly used.

Processor registers, memory addresses, and data are all expressed in hexadecimal.