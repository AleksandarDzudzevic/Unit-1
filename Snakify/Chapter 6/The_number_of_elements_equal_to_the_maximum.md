# Unit 6 Problem 13
```.py
lst = []
a=int(input())
max=a
while a != 0:
    lst.append(a)
    a=int(input())
    if a>max:
        max=a
num=0
for i in range(0,len(lst)):
    if lst[i]==max:
        num+=1
print(num)
```
