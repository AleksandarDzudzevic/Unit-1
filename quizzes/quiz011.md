![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz011text.png)
# Sl&HL (only difference that for input in the sl one I can skip name of the month and just say that a=10 (My birthday is in October))
## function
```.py
twentyeight = ["February"]
thirty = ["April", "June", "September", "Novemeber"]
thirty_one = ["January", "March", "May", "July", "August", "October", "December"]


def month() -> str:
    '''
    prints everything needed
    :return str(calendar):
    '''
    months = ['January', 'February', 'March', 'April', 'May', 'June', 'July',
              'August', 'September', 'October', 'November', 'December']
    curmnth = input("Enter the Month:")
    x: int = 0  # x is used to get an index of the inputed month
    for check in months:
        if check == curmnth:
            a = x
            break
        else:
            x += 1
    week = ''
    count = 0
    day = 0
    date = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    spacenum = []
    for i in range(((sum(date[:a]) + 1) % 7 + 4) % 7):
        spacenum.insert(0, '  ')
    for x in range(int(date[a])):
        day += 1
        spacenum.append(str(day))
    for d in spacenum:
        if len(d) < 2:
            week += '0'
        week += d
        week += ' '
        count += 1
        if count % 7 == 0:
            week += '\n'
    print("|", months[a].center(21, '-'), "|")
    print('Mo Tu We TH Fr Sa Su')
    print(week)
    return 'a'
```
## Main
```.py
from quiz011lib import month
month()
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz011test.png)
## Flow diagram
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz011flowdiagram.jpg)
