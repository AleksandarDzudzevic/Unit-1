# Unit 5 Problem 8
```.py
s=input()
a=s.find('h')
b=len(s)-s[::-1].find('h')
s2=s[a:b]
print(s[0:a]+s2[::-1]+s[b:])
```
