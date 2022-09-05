# Quiz 4
### Edit the code so the user manual is better, code is simpler...
So to conclude, what I did is i added user messages to make the program and the instructions clearer, an then I simplified the code to one if function
```.py
counter=0
int1=(input("Enter an integer"))
while not int1.isdigit() and counter<=5:
    int1=input(f"Error, you have {5-1-counter} chancs left, please enter an intiger ")
    counter+=1
if counter>5:
    exit()
print("Entering an intiger was a success")
int1=int%10+int1/10%10
if int1<10 and int1>0:
    print("number is perfect")
else:
    print("Number is not perfect")
```
