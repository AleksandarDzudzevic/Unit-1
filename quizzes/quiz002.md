# Quiz 2
## Given 2 numbers A and B, Output TRUE if one of them is 20 or if their sum is 20.
Here is the solution code for the following problem:
```.py
a=[1,13,14,5]
b=[19,7,1,4]
for i,j in zip(a,b):
    if i+j==20 or i==20 or j==20:
        output=True
        print(f"{output} for {i} and {j}")
    else:
        output=False
        print(f"{output} for {i} and {j}")
```
