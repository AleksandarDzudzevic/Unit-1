# Unit 6 Problem 16
```.py
i=1
a=int(input())
b=0
max=0
while a:
    b=int(input())
    if a==b:
        i+=1
        a=b
    else:
        if max<i:
            max=i
        i=1
        a=b
print(max)
    
```
