## QUIZ #004

```.py
# This function receives an integer N and returns all of its factors
# It also returns if the sum of the factors is the same as N 

def perfectN(n):
    factors = []
    reduced = n
    res = False

    while reduced != 1:
        for i in range(1,251):
            if reduced % i == 0:
                reduced = reduced / i
                factors.append(i)

    if sum(factors) == n:
        res = True

    return str(str(factors) + str(res))

print(perfectN(6))
print(perfectN(10))
```

#### Evidence that this works:
![stuff](https://user-images.githubusercontent.com/88994602/138989927-f4d0e652-6ad9-4919-9477-31050812c5c6.png)
