## Peer Mystery Boxes

### Paolo's Os

```.py
def paolo_o(strin):
    ous = 0
    for char in str(strin).upper():
        if char == "O":
            ous += 1
    return ous
```

Evidence that it works:
![image](https://user-images.githubusercontent.com/88994602/136109603-d8f47107-135e-40e4-9a47-f2961ea1e211.png)

### Nisrine's Number remover

```.py
def number_remover(stringu):
    answer = []
    for char in stringu:
        if not char.isdigit():
            answer.append(char)
    return str(''.join(answer))
```

Evidence that it works:
![image](https://user-images.githubusercontent.com/88994602/136109966-c4ef44de-01f1-4e1a-a24b-99af82c702a4.png)

### Esslam's Unique Letters

```.py
def essl_rep(stringu):
    res = True
    for i in range(len(stringu)-1):
        last, now = stringu[i - 1], stringu[i]
        if last == now:
            res = False
    return res
```

Evidence that it works:
![image](https://user-images.githubusercontent.com/88994602/136110849-94586362-c36d-44e2-9316-fe194e5087a5.png)

### Ryu's Time Difference

```.py
def ryus_time(h1, m1, h2, m2):
    diff = 0
    if m1 <= m2:
        diff += m2 - m1
        diff += (h2 - h1) * 60
    elif m1 > m2:
        diff += (60 - m1) + m2
        diff += ((h2 - h1) - 1) * 60
    return diff
```

Evidence that it works:
![image](https://user-images.githubusercontent.com/88994602/136112553-9d632bdb-3f4c-40fe-b150-dd408d640ddc.png)

### Beril's 

Work in progres...

