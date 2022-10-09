![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz012text.png)
### Function that solves the program
```.py
bold_green=green = "\033[1;32m"
end_code="\033[00m"
def mulTable(num:int)->str:
    """

    :param num: enter the number which we will multiply
    :return: table of all multiplications
    """
    table=""
    table+=(f"{bold_green}TABLE OF MULTIPLICATIONS{end_code}".center(20))
    for i in range(1,10):
        table+="\n"+(5*" ")+str(num)+" x "+str(i)+" = "+str(num*i)
    return(table)

```
### main() program
```.py
from quiz012lib import mulTable
num=int(input("Enter the number"))
print(mulTable(num))
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz012test.png)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz012flowchart.jpg)
