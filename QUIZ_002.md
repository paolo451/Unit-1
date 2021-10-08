## Quiz #002

```.py
def LargestDistance(a, b, c):
    listu = []
    listu.append(a)
    listu.append(b)
    listu.append(c)

    listu.sort()

    res = listu[2] - listu [0]

    return res
```
Prove that this works:
![](quiz002.png)
