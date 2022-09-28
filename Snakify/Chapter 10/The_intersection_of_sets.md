# Unit 10 Problem 3
```.py
x=[]
string=(set(input().split()) & set(input().split()))
for a in string:
    if a.isdigit():
        x.append(int(a))
for i in range(len(x)):
    for j in range(i+1,len(x)):
        if x[j]<x[i]:
            x[i],x[j]=x[j],x[i]
    print(x[i],end=" ")
    ```
