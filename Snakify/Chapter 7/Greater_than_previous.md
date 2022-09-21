# Unit 7 Problem 3
```.py
a=input().split(" ")
for i in range(1,len(a)):
    if int(a[i-1])<int(a[i]):
        print(a[i],end=" ")
```
