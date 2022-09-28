# Unit 10 Problem 4
```.py
a=input().split()
for i in range(len(a)):
    if not a[i] in a[:i]:
        print("NO")
    else:
        print("YES")
```
