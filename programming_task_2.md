## Programming Task #02

Strange Numbers: Given a number as a String N. Multiply all of its digits, and repeat the same with the product obtained till the product consists of only one digit. Output the number of steps taken to do so. 

Example: N = 39
Step 1: 3 * 9 = 27
Step 2: 2 * 7 = 14
Step 3: 1 * 4 = 4

Since it took us 3 steps to reach a number with only 1 digit, the output is 3.

```.py
steps = 0

strnum = input("Input your strange number: ")

while len(strnum) > 1:
    newnum = 1

    for i in strnum:
        newnum *= int(i)

    strnum = str(newnum)
    steps += 1

print(steps)
```

