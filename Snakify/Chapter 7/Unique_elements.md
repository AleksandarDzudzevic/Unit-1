# Unit 7 Problem 11
```.py
a=[int(i) for i in input().split()]
cnt=1
for i in range(len(a)):
    for j in range(0,len(a)):
        if a[i]==a[j] and i!=j:
            cnt=0
    if cnt:
        print(a[i])
    cnt=1
    ```
