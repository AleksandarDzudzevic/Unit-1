# Quiz 5
## Print all the dividers of the number (not number itself) and see if their sum is equal to the number
![](quiz005.jpg)
Here is the code:
```.py
num=int(input())
i=1
sum=0
list=[]
while i<=num//2:
    if num%i==0:
        list.append(i)
        sum+=i
    i+=1
print(list)
if sum==num:
    print("True")
else:
    print("False")
```
