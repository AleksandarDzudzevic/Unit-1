# Unit 8 Problem 3
```.py
def caps(word):
    firstchr=word[0]
    newfirstchr=chr(ord(firstchr)-32)
    return newfirstchr+word[1:]
string=input().split()
newstr=[]
for word in string:
    newstr.append(caps(word))
print(' '.join(newstr))
```
