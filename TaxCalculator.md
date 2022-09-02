# Tax calculator program done on September 2nd 2022
## Calculate total taxes of ISAK BANK user based on their salary
```.py
print("WELCOME TO ISAK BANK, TO PROCED PLEASE ENtER YOUR CURRENT SALARY IN USD")
salary=int(input())
if salary<=10000:
    tax=int(salary/20)
elif salary<=50000:
    tax=int(salary/10)
elif salary<=100000:
    tax=int(salary*0.15)
elif salary>100000:
    tax=int(salary/4)
print(f"Your tax is {tax}USD, please pay as soon as you can")
```
