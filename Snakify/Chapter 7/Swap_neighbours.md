# Unit 7 Problem 8
```.py
a=[int(i) for i in input().split()]
for i in range(0,len(a)-1,2):
    a[i],a[i+1]=a[i+1],a[i]
for i in range(0,len(a)):
    print(a[i])
```
