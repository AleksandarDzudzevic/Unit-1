# Original problem was: Given the room floor and the room number on that floor, find the rooom number
```.py
num=1
while num!=100:
    if num%10!=0:
         print(f"{num}-Floor {num//10} ROOM {10}")
    else:
        print(f"{num}-Floor {num//10+1} ROOM {num%10}")
    num+=1
    #THIS IS HL PROBLEM
num=int(input("Enter the room number"))
if num%10!=0:
    print(f"{num}-Floor {num//10+1} ROOM {num%10}")
else:
    print(f"{num}-Floor {num//10} ROOM {10}")

```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz008test.png)
The first flow diagram answers the following problem.
### The 2nd flow diagram is the opposite, given the room number print the floor and the room number on that floor + print the same thing for all the rooms (100 rooms)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz008flowdiagram1.png)
2nd picture is the code for the 2nd flow diagram and instruction on how to display things in flow diagram.
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz008codeandflowchartsymbols.jpg)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz008flowdiagram2.jpg)
