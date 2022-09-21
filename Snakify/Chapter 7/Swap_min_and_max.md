# Unit 7 Problem 9
```.py
a=[int(i) for i in input().split()]
min=a[0]
mini=0
max=a[0]
maxi=0
for i in range(1,len(a)):
    if a[i]<min:
        min=a[i]
        mini=i
    if a[i]>max:
        max=a[i]
        maxi=i
a[maxi],a[mini]=a[mini],a[maxi]
for x in a:
    print(x)
```
