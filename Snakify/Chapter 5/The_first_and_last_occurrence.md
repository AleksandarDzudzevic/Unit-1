# Unit 5 problem 5
```.py
s=input()
if s.find('f')>=0:
    print(s.find('f'))
    if s.find('f')!=len(s)-1-s[::-1].find('f'):
        print((len(s)-1-s[::-1].find('f')))
```
