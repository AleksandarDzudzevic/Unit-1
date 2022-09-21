# Unit 7 problem 6
```.py
a=[int(i) for i in input().split()]
max=a[0]
ind=0
for i in range(1,len(a)):
    if a[i]>max:
        max=a[i]
        ind=i
print(max,ind)
```
