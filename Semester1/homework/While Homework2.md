# For and While

### `for` Loop
#### Characteristics:
1. **Iterative**: The `for` loop is commonly used to iterate over sequences (like lists, tuples, dictionaries, sets, strings) or generator objects.
2. **Conciseness**: The `for` loop is more concise when dealing with sequential data.
3. **Clarity**: The number of iterations is usually clear at the start, as it is based on the number of elements in the iterable.
#### Syntax:
```python
for variable in iterable:
    # do something with variable
```
#### Example:
```python
for i in range(5):
    print(i)  # Outputs 0 1 2 3 4
```
### `while` Loop
#### Characteristics:
1. **Conditional**: The `while` loop continues to execute as long as the specified condition is true (i.e., the condition evaluates to False).
2. **Flexibility**: The `while` loop is more flexible when dealing with loops of an indeterminate number of iterations because its execution depends on a condition expression.
3. **Control**: You can precisely control the execution of the loop by changing the condition within the loop body.
#### Syntax:
```python
while condition:
    # do something while the condition is True
```
#### Example:
```python
i = 0
while i < 5:
    print(i)  # Outputs 0 1 2 3 4
    i += 1
```
### Specific Differences:
1. **Control Method**:
   - The `for` loop controls the iteration process, automatically handling each element in the sequence.
   - The `while` loop controls the condition; as long as the condition is True, the loop will continue.
   
2. **Flexibility**:
   - The `for` loop is typically used when the number of iterations is known.
   - The `while` loop is more suitable for situations where the number of iterations is unknown and needs to end based on a certain condition.
   
3. **Complexity**:
   - The `for` loop is more concise when dealing with sequences and less prone to errors.
   - The `while` loop may require more code to properly control the loop's condition, making it potentially more error-prone (e.g., forgetting to update the condition within the loop body can lead to an infinite loop).
   
4. **Use Cases**:
   - When you need to traverse a collection, the `for` loop is the better choice.
   
   - When you need to repeatedly execute a code block based on a condition, the `while` loop is more appropriate.
     In summary, the choice between a `for` loop and a `while` loop depends on the specific application scenario and requirements. In some cases, they can be used interchangeably, but in others, one loop may be more suitable than the other.
   
     

#### 模拟太阳系行星运动

使用`while`循环和简单的图形库（如`turtle`）来模拟行星围绕太阳的运动。

```python
import turtle
import math

sun = turtle.Turtle()
sun.shape("circle")

def move_planet(t, distance, angle):
    t.forward(distance)
    t.right(angle)

earth = turtle.Turtle()
earth.shape("circle")
earth.color("blue")

angle = 0
while True:
    move_planet(earth, 5, angle)
    angle += 1
    if angle > 360:
        angle = 0
    turtle.update()

```

### 猜数字游戏

```
import random

# 随机生成一个1到100之间的数字
secret_number = random.randint(1, 100)
guess = None

while guess != secret_number:
    guess = int(input("猜一猜这个数字是多少（1-100）: "))
    if guess < secret_number:
        print("太小了！")
    elif guess > secret_number:
        print("太大了！")

print("恭喜你！你猜对了，数字是：", secret_number)
```

#### `for`循环特点：

1. **迭代性**：`for`循环通常用于迭代序列（如列表、元组、字典、集合、字符串）或生成器对象。
2. **简洁性**：`for`循环在处理序列数据时语法更简洁。
3. **明确性**：循环的次数通常在开始时就已经明确，因为它是基于可迭代对象中的元素数量。
#### 语法：
```python
for variable in iterable:
    # do something with variable
```
#### 示例：
```python
for i in range(5):
    print(i)  # 输出 0 1 2 3 4
```
### `while`循环
#### 特点：
1. **条件性**：`while`循环会持续执行，直到指定的条件不再满足（即条件评估为False）。
2. **灵活性**：`while`循环在处理不确定次数的循环时更为灵活，因为它的执行次数依赖于一个条件表达式。
3. **控制性**：你可以通过在循环体内改变条件来精确控制循环的执行。
#### 语法：
```python
while condition:
    # do something while the condition is True
```
#### 示例：
```python
i = 0
while i < 5:
    print(i)  # 输出 0 1 2 3 4
    i += 1
```
### 具体区别：
1. **控制方式**：
   - `for`循环控制的是迭代过程，它自动处理序列中的每个元素。
   - `while`循环控制的是条件，只要条件为True，循环就会继续。
2. **灵活性**：
   - `for`循环通常用于已知迭代次数的情况。
   - `while`循环更适用于迭代次数未知，需要根据某个条件来结束循环的情况。
3. **复杂性**：
   - `for`循环在处理序列时更简洁，不易出错。
   - `while`循环可能需要更多的代码来正确控制循环的条件，因此可能更容易出错（例如，忘记在循环体内更新条件，可能导致无限循环）。
4. **使用场景**：
   - 当你需要遍历一个集合时，`for`循环是更好的选择。
   - 当你需要基于某个条件来重复执行代码块时，`while`循环是更合适的选择。
   总的来说，选择`for`循环还是`while`循环取决于具体的应用场景和需求。在某些情况下，两者可以互换使用，但在其他情况下，一种循环可能比另一种更合适。

### **题目 1：打印 1 到 N 的数字**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter a number (N): "))
for i in range(1, N + 1):
    print(i, end=" ")
print()
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter a number (N): "))
i = 1
while i <= N:
    print(i, end=" ")
    i += 1
print()
```

---

### **题目 2：计算 1 到 N 的累加和**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter a number (N): "))
sum = 0
for i in range(1, N + 1):
    sum += i
print("Sum:", sum)
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter a number (N): "))
sum = 0
i = 1
while i <= N:
    sum += i
    i += 1
print("Sum:", sum)
```

---

### **题目 3：打印偶数**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter a number (N): "))
for i in range(2, N + 1, 2):
    print(i, end=" ")
print()
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter a number (N): "))
i = 2
while i <= N:
    print(i, end=" ")
    i += 2
print()
```

---

### **题目 4：计算 N 的阶乘**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter a number (N): "))
factorial = 1
for i in range(1, N + 1):
    factorial *= i
print("Factorial:", factorial)
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter a number (N): "))
factorial = 1
i = 1
while i <= N:
    factorial *= i
    i += 1
print("Factorial:", factorial)
```

---

### **题目 5：数字逆序**

#### **代码实现：`for` 循环**
```python
num = int(input("Enter a number: "))
reversed_num = 0
for digit in str(num):
    reversed_num = int(str(digit) + str(reversed_num))
print("Reversed:", reversed_num)
```

#### **代码实现：`while` 循环**
```python
num = int(input("Enter a number: "))
reversed_num = 0
while num > 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num //= 10
print("Reversed:", reversed_num)
```

---

### **题目 6：判断质数**

#### **代码实现：`for` 循环**
```python
num = int(input("Enter a number: "))
is_prime = True
if num < 2:
    is_prime = False
else:
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break

print(f"{num} is prime: {is_prime}")
```

#### **代码实现：`while` 循环**
```python
num = int(input("Enter a number: "))
is_prime = True
if num < 2:
    is_prime = False
else:
    i = 2
    while i <= int(num ** 0.5):
        if num % i == 0:
            is_prime = False
            break
        i += 1

print(f"{num} is prime: {is_prime}")
```

---

### **题目 7：打印乘法表**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter a number (N): "))
for i in range(1, N + 1):
    for j in range(1, N + 1):
        print(f"{i} x {j} = {i * j}", end="\t")
    print()
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter a number (N): "))
i = 1
while i <= N:
    j = 1
    while j <= N:
        print(f"{i} x {j} = {i * j}", end="\t")
        j += 1
    print()
    i += 1
```

---

### **题目 8：斐波那契数列**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter the number of terms (N): "))
a, b = 0, 1
for _ in range(N):
    print(a, end=" ")
    a, b = b, a + b
print()
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter the number of terms (N): "))
a, b = 0, 1
count = 0
while count < N:
    print(a, end=" ")
    a, b = b, a + b
    count += 1
print()
```

---

### **题目 9：统计数字的位数**

#### **代码实现：`for` 循环**
```python
num = int(input("Enter a number: "))
digits = 0
for _ in str(num):
    digits += 1
print("Number of digits:", digits)
```

#### **代码实现：`while` 循环**
```python
num = int(input("Enter a number: "))
digits = 0
while num > 0:
    num //= 10
    digits += 1
print("Number of digits:", digits)
```

---

### **题目 10：打印简单的星号图形**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter the number of rows (N): "))
for i in range(1, N + 1):
    print("*" * i)
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter the number of rows (N): "))
i = 1
while i <= N:
    print("*" * i)
    i += 1
```

---

### **题目 11：找出 1 到 N 的所有倍数**

#### **代码实现：`for` 循环**
```python
N = int(input("Enter the range (N): "))
X = int(input("Enter the divisor (X): "))
for i in range(1, N + 1):
    if i % X == 0:
        print(i, end=" ")
print()
```

#### **代码实现：`while` 循环**
```python
N = int(input("Enter the range (N): "))
X = int(input("Enter the divisor (X): "))
i = 1
while i <= N:
    if i % X == 0:
        print(i, end=" ")
    i += 1
print()
```

---

### **题目 12：数字猜测游戏**

#### **代码实现：`while` 循环**
```python
target = 50
guess = -1
while guess != target:
    guess = int(input("Guess the number: "))
    if guess < target:
        print("Too low!")
    elif guess > target:
        print("Too high!")
print("Correct! The number is 50.")
```

#### **代码实现：`for` 循环**  
```python
target = 50
for _ in iter(int, 1):  # Infinite loop using `for`
    guess = int(input("Guess the number: "))
    if guess < target:
        print("Too low!")
    elif guess > target:
        print("Too high!")
    else:
        print("Correct! The number is 50.")
        break
```

---

完整实现涵盖了所有题目，使用了 `for` 和 `while` 两种循环方式。如果有进一步需求，请随时告诉我！ 😊