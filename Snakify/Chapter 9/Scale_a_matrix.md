# Unit 9 Problem 7 
```.py
n=[int(i) for i in input().split()]
a=[[int(x) for x in input().split() ]for i in range(n[0])]
c=int(input())
for i in range(n[0]):
    for j in range(n[1]):
        a[i][j]*=c
print('\n'.join([" ".join([str(i) for i in row])for row in a]))
```
