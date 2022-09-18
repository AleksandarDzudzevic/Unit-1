# Unit 6 problem 15
```.py
num=int(input())
i=1
a1=0
a2=1
a3=0
while num>a3:
    a3=a1+a2
    a1=a2
    a2=a3
    i+=1
if num==a3:
    print(i)
else:
    print(-1)
```
