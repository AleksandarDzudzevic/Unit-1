# Unit 6 Problem 14
```.py
size=int(input())
i=1
a1=0
a2=1
a3=0
while i!=size:
    a3=a1+a2
    a1=a2
    a2=a3
    i+=1
print(a3)
```
