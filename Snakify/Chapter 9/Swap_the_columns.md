# Unit 9 Problem 6
```.py
def swap_columns(a,i,j):
    for row in a:
        row[i],row[j]=row[j],row[i]
    return a
n=[int(i) for i in input().split()]
a=[[int(x) for x in input().split() ]for i in range(n[0])]
i,j=[int(i) for i in input().split()]
for row in swap_columns(a,i,j):
    print(' '.join([str(i) for i in row]))
```
