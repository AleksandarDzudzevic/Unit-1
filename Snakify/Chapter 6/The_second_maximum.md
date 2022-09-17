# Unit 6 Problem 12
```.py
lst = []
a=int(input())
max=a
while a != 0:
    lst.append(a)
    a=int(input())
    if a>max:
        max=a
sec=0
for i in range(0,len(lst)):
    if lst[i]>sec and lst[i]!=max:
        sec=lst[i]
print(sec)
```
