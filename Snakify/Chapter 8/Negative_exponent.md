# Unit 8 Problem 2
```.py
def power(a:float,n:int):
    s=1
    if n>0:
        for i in range(n):
            s*=a
        return(s)
    else:
        for i in range(abs(n)):
            s*=a
        return(1/s)
a=float(input())
n=int(input())
print(power(a,n))
```
