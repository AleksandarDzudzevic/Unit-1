# Unit 8 Problem 6
```.py
def fib(n):
    if n <= 1:
       return n
    else:
       return(fib(n-1) +fib(n-2))
n=int(input())
print(fib(n))
```
