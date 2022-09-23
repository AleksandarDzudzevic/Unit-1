# Quiz 4
### Edit the code so the user manual is better, code is simpler...
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz004text.png)
These are the following changes:
1) Clear messages explaining process
2) instead of having d1=number%10 and d2=>tens number we can just combine it all in one if and get rid of 3 variables and make our program much faster
So to conclude, what I did is i added user messages to make the program and the instructions clearer, and then I simplified the code to one if function and added ainput counter which closes the program after 5 unsuccessful inputs 5xnot an intiger)
3) Write accurate message as a return because program doesn't check if the number is perfect
4) Do a flow diagram which accuratly represents the updated code
```.py
counter=0
int1=(input("Enter an integer"))
#The while under, is sed as a counter, which after 5 unsuccessful inputs, exits the program
while not int1.isdigit() and counter<=5:
    int1=input(f"Error, you have {5-1-counter} chancs left, please enter an intiger ")
    counter+=1
if counter>5:
    exit()
print("Entering an intiger was a success")
#This part is the code that replaces the comlicated and unclear one from the flow diagram given in the first picture
int1=int(int1) #This is neccesary because of str input that we used in order to have input checker
if int1<10 and int1>0:
    print("Number is a single digit number")
else:
    print("Number is not a single digit number")
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz004flowdiagram.png)
#### In the test it says number is not perfect but message should say number is/isn't a single digit number like in the code 
![Successful test](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz004test.png)
