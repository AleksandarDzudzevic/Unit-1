# Task 2 done on September 20th 2022
At the bottom is the code of my_library from which I used the functions that I needed
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task2text.png)
```.py
from my_library import validate_int_input,end_code,red,green,bold_green
welcome_msg="Welcome to the EV calculator".center(50,"+")
prompt_msg="Please enter an option [1-4]"
print(f"{green}{welcome_msg}{end_code}")
print(f"{green}Options{end_code}".center(50))
menu="""1. Avarage time per kWh
2.Total kWh
3.Total charge time
4. Show all data
"""
print(menu)
option= validate_int_input(prompt_msg)
while option>4 or option<1:
    option=validate_int_input((f"{red}Invalid option.{prompt.msg}{end_code}"))
#option 4 all data
with open("charging_log.csv","r") as file:
    ev_logs = file.readlines()

index=0
if option==4:
    for log in ev_logs:
         if index>0:
            print(f"{bold_green}No.{index}:  {log.strip()}{end_code}")#strip removes all \n -> no more empty rows
         index+=1
#option 3 total charge time
if option==3:
    index=0
    total_time=0
    for log in ev_logs:
        if index>0:
            values=log.split(",")
            date=values[0]
            energy=values[1]
            time=values[2].split(":")
            total_time+=(int(time[0])*3600+int(time[1])*60+int(time[2]))
        index+=1
    print(f"{green}The total time charged is {total_time//3600}Hours, {total_time%3600//60}minutes, {total_time%60} seconds")
#option 2 Total kWh
if option==2:
    index=0
    total_energy=0
    for log in ev_logs:
        if index>0:
            values=log.split(",")
            date=values[0]
            energy=values[1]
            time=values[2]
            total_energy+=float(energy[0:5])
        index+=1
    print(f"{green}The total energy charged is {total_energy}kWh")
#option 1 Avarege time per kWh
if option==1:
    index=0
    total_energy=0
    total_time=0
    for log in ev_logs:
        if index>0:
            values=log.split(",")
            date=values[0]
            energy=values[1]
            time=values[2]
            total_energy+=float(energy[0:5])
            time=values[2].split(":")
            total_time+=(int(time[0])*3600+int(time[1])*60+int(time[2]))
        index+=1
    print(f"{green}The avarage time per kWh is {int(total_time/total_energy//3600)}Hours, {int(total_time/total_energy%3600//60)}minutes, {int(total_time/total_energy%60)} seconds")
```
# LIBRARY
```.py
# I will put all the code that i want to reuse in this file
# NAME
end_code="\033[00m"
red="\33[0;31m"
green = "\033[0;32m"
bold_green=green = "\033[1;32m"

#colors=
def author():
    return "Dr.Aleksandar Dzudzevic"
#MAX OF TWO NUMBERS
def maximum(a:int,b:int)->int:
    if a>b:
        out=a
    else:
        out=b
    return out
#This validates if user's input is intiger
def validate_int_input(msg:str)->int:
    end_code="\033[00m"
    red="\33[0;31m"

    number=input(msg)
    while not number.isdigit():
        number=input(f"{red}Error.{msg}{end_code}")
    return int(number)
#This prints the error in red
```
## Option 1 test
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task2option1test.png)
## Option 2 test
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task2option2test.png)
## Option 3 test
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task2option3test.png)
## Option 4 test
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task2option4test.png)
