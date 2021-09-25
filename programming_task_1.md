## Programming Task #01

Ask the user for  2 numbers, A and B, Output TRUE if one of them is 10 or if their sum is 10.

Examples: 
Makes10(9, 10) → TRUE;
Makes10(9, 9) → FALSE;
Makes10(1, 9) → TRUE

```.py
a = int(input("Enter your first number: "))
b = int(input("Enter your second number: "))

if a == 10 or b == 10 or a + b == 10:
    print("TRUE")
else:
    print("FALSE")
```
