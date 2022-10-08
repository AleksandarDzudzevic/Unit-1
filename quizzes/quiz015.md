![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz015text.png)
```.py
def open_doors(numdoors:int,students:int)->int:
    '''

    :param doors:
    :param n:
    :return: the number of the doors open for n students
    '''
    doors=[]
    count=0
    for i in range(numdoors):
        doors.append(False)
    for std in range(1,students+1):
        for door in range(1,numdoors+1):
            if door%std==0:
                doors[door-1]=not doors[door-1]
    count = doors.count(True)
    return(count)
"""doors=int(input("Enter the number of doors"))
students=int(input("Enter the number of students"))
print(open_doors(doors,students))"""
print(open_doors(numdoors=10,students=10))
print(open_doors(numdoors=100,students=100))

```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz015test.png)
