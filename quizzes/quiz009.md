
```.py

'''
word=str(input("Enter the string"))
newword=""
for i in range(len(word)):
     if ord(word[i])>=97 and ord(word[i])<=122:
        newword+=chr(((ord(word[i])-96+13)%26+96))
     if ord(word[i])>=65 and ord(word[i])<=90:
        newword+=chr(((ord(word[i])-64+13)%26+64))
print(newword)
'''
word=str(input("Enter the string"))
shft=int(input("enter the shift size"))
newword=""
for i in range(len(word)):
     if ord(word[i])>=97 and ord(word[i])<=122:
        newword+=chr(((ord(word[i])-96+shft)%26+96))
     if ord(word[i])>=65 and ord(word[i])<=90:
        newword+=chr(((ord(word[i])-64+shft)%26+64))
print(newword)
```
