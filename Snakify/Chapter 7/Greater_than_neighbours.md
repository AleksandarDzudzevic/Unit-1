# Unit 7 problem 5
```.py
a = [int(i) for i in input().split()]
x=0
for i in range(1,len(a)-1):
    if a[i]>a[i-1]and a[i]>a[i+1]:
        x+=1
print(x)

```
