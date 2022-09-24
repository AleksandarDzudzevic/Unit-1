# Unit 9 Problem 5
```.py
n=int(input())
for i in range(n):
    for j in range(n):
        if i+j<n-1:
            print('0',end=' ')
        elif i+j==n-1:
            print('1',end=' ')
        else:
            print('2',end=' ')
    print('\n')
```
