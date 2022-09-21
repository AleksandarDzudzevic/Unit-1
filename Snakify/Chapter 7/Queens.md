# Unit 7 Problem 12
```.py
a=[]
for i in range(0,7):
    a.append([int(i) for i in input().split()])
x=1
for i in range(0,6):
    for j in range(i,7):
        if i!=j and not (a[i][0]!=a[j][0] and a[i][1]!=a[j][1] and  abs(a[i][0]-a[j][0])!=abs(a[i][1]-a[j][1])):
            x=0
if x:
    print("NO")
else:
    print("YES")
    ```
