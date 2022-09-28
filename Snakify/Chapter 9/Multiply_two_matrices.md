# Unit 9 problem 8
```.py
m,n,r=[int(i) for i in input().split()]
mtr1=[[int (i) for i in input().split()]for j in range(m)]
mtr2=[[int (i) for i in input().split()]for j in range(n)]
newmtr=[[0]*r for i in range(m)]
for i in range(m):
    for j in range(r):
        for k in range(n):
            newmtr[i][j]+=mtr1[i][k]*mtr2[k][j]
print('\n'.join([" ".join([str(j) for j in row])for row in newmtr]))
```
