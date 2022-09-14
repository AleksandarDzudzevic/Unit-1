# Given a number of passwords and password size, make a random passowrd +if you can, color it as well
Here is the code which not only coolors, but also randomizes background and text color.
```.py
from colorama import init, Fore, Back, Style
import math
# essential for Windows environment
init()
# all available foreground colors
FORES = [ Fore.MAGENTA,Fore.LIGHTBLUE_EX ,Fore.RED,Fore.GREEN,Fore.LIGHTYELLOW_EX,Fore.CYAN]
# all available background colors
BACKS = [Back.BLACK]

def print_with_color(s, color=Fore.WHITE,brightness=Style.NORMAL, **kwargs):
    """Utility function wrapping the regular `print()` function
    but with colors and brightness"""
    print(f"{color}{brightness}{s}", **kwargs)
import random
passnum=int(input("How many passwords do you need"))
charnum=int(input("Enter how many characters should the password have"))
a=''
num=32
print("Your passwords are:".upper())
for j in range(0,passnum-1):
    for i in range(0,charnum):
        num=random.randint(33,126)
        a+=chr(num)
    print_with_color(a,FORES[random.randint(0,len(FORES)-1)],BACKS[random.randint(0,len(BACKS)-1)])
    a=''

```
