#Input the starting number the steping number(amount which you add in each loop) and ending number/limit
```.py
start=int(input("Enter a starting number"))
step=int(input("Enter a step"))
end=int(input("Enter the number limit"))
print("Entering an intiger was a success")
while start<=end:
    print(start)
    start+=step
    
