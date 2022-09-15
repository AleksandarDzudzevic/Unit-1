# Unit 5 Problem 6
```.py
string=input()
a=string.find('f')+1+string[string.find('f')+1:].find('f')
if string.find('f')<0:
    print("-2")
elif string[string.find('f')+1:].find('f')<0:
    print("-1")
else:
    print(a)
```
