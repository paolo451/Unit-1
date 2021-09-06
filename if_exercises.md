## If Exercises
Paolo Díaz

### 1. Minimum of two numbers
Given two integers, print the smaller value.

![](minimum.png)

```.py
N1 = int(input("Number 01"))
N2 = int(input("Number 02"))

if N1 > N2:
    print(N2)
else:
    print(N1)
```

### 2. Sign Function
For the given integer X print 1 if it's positive, -1 if it's negative, or 0 if it's equal to zero.
Try to use the cascade if-elif-else for it.

![](sign.png)

```.py
x = int(input("Input a number "))

if x > 0:
    print("1")
elif x == 0:
    print("0")
else:
    print("-1")
```

### 3. Minimum of Three Numbers
Given three integers, print the smallest value.

![](minimum3.png)

```.py
a = int(input("Input one number: "))
b = int(input("Input another number: "))
c = int(input("Input anoooother number: "))

if a>b:
    if b>c:
        print(c)
    else:
        print(b)
else:
    if a>c:
        print(c)
    else:
        print(a)
```

### 4. Equal Numbers
Given three integers, determine how many of them are equal to each other. The program must print one of these numbers: 3 (if all are the same), 2 (if two of them are equal to each other and the third is different) or 0 (if all numbers are different).

![](equals.png)

```.py
a = int(input("Input one number: "))
b = int(input("Input another number: "))
c = int(input("Input anoooother number: "))

if a == b:
    if b == c:
        print(3)
    else:
        print(2)
else:
    if a == c:
        print(2)
    elif b == c:
        print(2)
    else:
        print(0)
```

### 5. Rook Move

Chess rook moves horizontally or vertically. Given two different cells of the chessboard, determine whether a rook can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. The program should output YES if a rook can go from the first cell to the second in one move, or NO otherwise.

![](rookmove.png)

```.py
OY = int(input("From 1 to 8, input the Original column of the rook"))
OX = int(input("From 1 to 8, input the Original row of the rook"))

NY = int(input("From 1 to 8, input the New column of the rook"))
NX = int(input("From 1 to 8, input the New row of the rook"))

if OX == NX:
    print("YES")
elif OY == NY:
    print("YES")
else:
    print("NO")
```

### 6. Chess board - same color

Given two cells of a chessboard. If they are painted in one color, print the word YES, and if in a different color - NO.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell.

![](boardcolor.png)

```.py
Y1 = int(input("From 1 to 8, input the first column"))
X1 = int(input("From 1 to 8, input the first row"))

Y2 = int(input("From 1 to 8, input the second column"))
X2 = int(input("From 1 to 8, input the second row"))

SUM1 = X1 + Y1
SUM2 = X2 + Y2

# Here we see that the sum of the coordinates of every black tile will always be even, while the sum of the coordinates of 
# every white tile will always be odd, so that to know if they're the same color, we examine if both results are odd or 
# even by dividing them by 2 and obtaining the result.

if SUM1 % 2 == SUM2 % 2:
    print("YES")
else:
    print("NO")
```

### 7. King move

Chess king moves horizontally, vertically or diagonally to any adjacent cell. Given two different cells of the chessboard, determine whether a king can go from the first cell to the second in one move.
The program receives the input of four numbers from 1 to 8, each specifying the column and row number, first two - for the first cell, and then the last two - for the second cell. The program should output YES if a king can go from the first cell to the second in one move, or NO otherwise.

![](JESUCRISTOPORFIN.png)

```.py
OY = int(input("From 1 to 8, input the Original column of the rook"))
OX = int(input("From 1 to 8, input the Original row of the rook"))

NY = int(input("From 1 to 8, input the New column of the rook"))
NX = int(input("From 1 to 8, input the New row of the rook"))

if NY == OY + 1 or NY == OY - 1 or NY == OY: 
    if NX == OX + 1 or NX == OX - 1 or NX == OX:
        print("YES")
    else:
        print("NO")
else:
    print("NO")
```
