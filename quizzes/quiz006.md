# Given a string sum the ascii values of every char in it 
(Additional task was transforming ascii numbers of letters into their number in the alphabet and that is done by subtracting 96 from ascii code)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz006text.png)
### Here is the code for the quiz006 problem one:
```.py
word=input("Enter the string")
sum=0
i=0
for i in range (len(word)):
    sum+=(ord(word[i])) #summing ascii value of all chars in the string
    #ord is used to get the ascii value of the character which will be useful later on
print(sum)
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz006test1.png)
### Flow diagram for 1) and 2)
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz006flowdiagram1and2.jpg)
### Here is code for te second problem:
```.py
word=input("Enter the string")
sum=0
i=0
for i in range (len(word)):
    if ord(word[i])>=97 and ord(word[i])<=122: # Both if functions sum the order number in alphabet of every char by translating ascii value to order number in alphabet (-96/-64)
        sum+=(ord(word[i])-96)
    if ord(word[i])>=65 and ord(word[i])<=90:
        sum+=(ord(word[i])-64)
print("The sum of the order numbers of the letters in the string is "sum) 

```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz006test2.png)
