# Quiz 5
## Print all the dividers of the number (not number itself) and see if their sum is equal to the number
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz005text.png)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz005.jpg)
Here is the code:
```.py
num=int(input("Enter the number"))
i=1
sum=0
list=[]
while i<=num//2:
    if num%i==0:
        list.append(i) #This ads the divider into a string of all dividers
        sum+=i # summing dividers
    i+=1
print(list)
if sum==num:
    print("True")
else:
    print("False")
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz005test.png)
