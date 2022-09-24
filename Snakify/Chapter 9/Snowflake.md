# UNit 9 Problem 2
```.py
n=int(input())
for i in range (n):
    for j in range(n):
        if i==(n//2) or j==(n//2) or i==j or n-1-i==j:
            print('* ',end='')
        else:
            print(". ",end='')
    print("\n")

```
