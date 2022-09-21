# Unit 7 Problem 13
```.py
n, k = [int(i) for i in input().split()]
pins= ['I'] * n
for i in range(k):
    a,b = [int(i) for i in input().split()]
    for j in range(a- 1,b):
         pins[j] = '.'
print(''.join(pins))
```
