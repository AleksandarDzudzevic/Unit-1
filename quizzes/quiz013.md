![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz013text.png)
```.py
def mystery(a:int,b:int)->int:
    '''

    :param a:
    :param b:
    :return: multiplication minus the differnce between the numbers
    '''
    return(a*b-abs(a-b))
#a=int(input("Enter the first number")) if the user enters the numbers
#b=int(input("Enter the second number"))
print(mystery(a=70,b=50))
print(mystery(a=2,b=6))
print(mystery(a=4,b=10))
print(mystery(a=10,b=10))

```
