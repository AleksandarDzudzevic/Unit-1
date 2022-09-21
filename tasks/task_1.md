![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/task1questions.png)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Task1text2.2.png)
# Problems relating color of the in the school 
the first locker is red, second is white,third is yellow, fourth is blue and the colors repeat in the same order 
### Problem one is to print color of the each locker for the 2400 lockers in a school (I mad a table so the data is easier to see)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/taskk1flowchart.jpg)
```.py
#1:Just printing colors
lockers=2400
colors=["Blue","Red","White","Yellow"]
for i in range(1,lockers+1):
    print(f"Locker{i}--->{colors[i%4]}")
```
### Problem two is to answer what color will the locker be given the number of it
```.py
#2 The color of the given locker 
num=int(input("Enter the number of the locker"))
if num%4==1:
    print(f"COLOR OF LOCKER {num}:RED")
elif num%4==2:
    print(f"COLOR OF THE LOCKER {num}:WHITE")
elif num%4==3:
    print(f"COLOR OF THE LOCKER {num}:YELLOW")
else:
        print(f"COLOR OF THE LOCKER {num}:BLUE")
```
### Problem three is when given the color and number of lockers to output all the lockers in that color and use as many stroing edit functions
```.py
from colorama import init, Fore, Back, Style
import math
# essential for Windows environment
init()
# all available foreground colors
FORES = [Fore.RED, Fore.WHITE,Fore.YELLOW, Fore.BLUE]
def print_with_color(s, color=Fore.WHITE, **kwargs):
    """Utility function wrapping the regular `print()` function
    but with colors and brightness"""
    print(f"{color}{s}", **kwargs)
color=input("ENTER THE COLOR(RED,WHITE,YELLOW,BLUE)")
if not color:
    print("You didn't enter the color")
num=int(input("NUMBER OF LOCKERS:"))
if color=="RED":
    x=1
elif color=="WHITE":
    x=2
elif color=="YELLOW":
    x=3
elif color=="BLUE":
    x=4
else:
    print("ERROR")
    print("These are the lockers in that color".upper())
for i in range (0,(num//4)):
    print(f"The locker number {4*i+x} is the color".lower())
    if color.isprintable():
        print_with_color(color, color=FORES[x-1])
```
### Problem 4 Make a school email given last and first name and also assign the locker number in the mail
```.py
#4 :
num=int(input("Enter the number of the students "))
a=[""]
b=[""]
for i in range(0,num):
    a[i]=input(f"Enter the name of the student number{i+1}")
    b[i]=input(f"Enter the last name of the student number{i+1}")
    print(f"New email is {b[i]}.{a[i]}.{i}@uwcisak.jp".lower())
```
