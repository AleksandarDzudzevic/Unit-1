# Unit 5 Problem 11
```.py
s=input()
a=s.find('h')
b=s.rfind('h')
s=s.replace('h','H')
print(s[0:a]+'h'+s[a+1:b]+'h'+s[b+1:])
```
