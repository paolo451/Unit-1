## Programming Task 3

Using the program you created in Task 2, create a program that searches automatically for strange numbers. Can you find a number that will take 10 steps or more?

```.py
rangstart = int(input("Enter the number you wish to start with in your search for a very big Strange Number"))

for z in range(rangstart, rangstart + 9999999999999999999999):

    strnum = str(z)
    steps = 0

    while len(strnum) > 1:
        newnum = 1

        for i in strnum:
            newnum *= int(i)

        strnum = str(newnum)
        steps += 1

    print(f"steps: {steps}, strnum: {z}")

    if steps > 10:
        break
        print("You found a HUGE strange number. It is {z}, and it took {steps} steps to get")
```

No, I cannot find a number that takes 10 steps or more. At least, not on a very efficient or fast way.
