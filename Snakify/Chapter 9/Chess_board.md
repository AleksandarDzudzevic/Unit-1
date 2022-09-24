# Unit 9 Problem 3
```.py
n=[int(i) for i in input().split()]
for i in range(n[0]):
    for j in range(n[1]):
        if i%2==0:
            if j%2==0:
                print('.',end=' ')
            else:
                print('*',end=' ')
        else:
            if j%2==0:
                print('*',end=" ")
            else:
                print('.',end=" ")
    print("\n")
```
