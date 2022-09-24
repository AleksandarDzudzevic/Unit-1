# Unit 9 Problem 1
```.py
n=[int (i) for i in input().split()]
max=-9999999999 #couldn't find min value variable in python
a,b=0,0
for i in range(n[0]):
    x=[(i) for i in input().split()]
    for j in range(n[1]):
        if float(x[j])>max:
            max=float(x[j])
            a,b=i,j
print(a,b)
```
