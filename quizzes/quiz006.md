# Given a string sum the ascii values of every char in it 
(Additional task was transforming ascii numbers of letters into their number in the alphabet and that is done by subtracting 96 from ascii code)
### Here is the code for the quiz006 problem one:
```.py
word=input()
sum=0
i=0
for i in range (len(word)):
    sum+=(ord(word[i]))
    #ord is used to get the ascii value of the character which will be useful later on
print(sum)
```
### Here is code for te second problem:
```.py
word=input("Eneter the string")
sum=0
i=0
for i in range (len(word)):
    if ord(word[i])>=97 and ord(word[i])<=122:
        sum+=(ord(word[i])-96)
    if ord(word[i])>=65 and ord(word[i])<=90:
        sum+=(ord(word[i])-64)
print("The sum of the order numbers of the letters in the string is "sum)

```
