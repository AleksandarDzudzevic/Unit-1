![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz010text.png)
## SL
#### Function which I used in the main program
```.py
def powersTen(quantity:int)->str:
    '''
    Return the power of ten of the input
    :param quantity:
    :return: string
    '''
    out=''
    sufix=["","Kilo","Mega","Giga","Tera","mili","micro","nano","pico"]
    for power in range(4,-1,-1):
        value=f"{quantity} {('000 ')*power}".ljust(25) + sufix[power]
        out+=value + "\n"
    for power in range(0,4):
        value=f"0. {('000 ')*(power)} 00{quantity}".ljust(25) + sufix[power+5]
        out+=value + "\n"
    return out


```
### Main program
```.py
from quiz010_lib import powersTen
print(powersTen(1))
```
# ------------------------------
## HL
### Function which i used in the main program
```.py
def powersTen(quantity:int,unit:str)->str:
    '''

    :param quantity: int
    :param unit:str
    :return: str
    '''
    out=''
    sufix=[" ","Kilo","Mega","Giga","Tera","mili","micro","nano","pico"]
    for power in range(4,-1,-1):
        value=f"{quantity} {('000 ')*power}".ljust(25) + sufix[power] + unit
        out+=value + "\n"
    for power in range(0,4):
        value=f"0. {('000 ')*(power)} 00{quantity}".ljust(25) + sufix[power+5] + unit
        out+=value + "\n"
    return out
```
### Main program
```.py
from quiz010_lib import powersTen
quantity=input("Enter the quantity")
unit=input("Input the unit name")
print(powersTen(quantity,unit))
```
#### Test
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz010test.png)
#### Flow diagram
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz010flowdiagram.jpg)
