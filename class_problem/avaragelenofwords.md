# This program returns avarage size of the word in a text that we input
```.py
text=(input)
sum=0
numwords=len(text.split())
for word in text.split(" "):
    size=len(word)
    sum+=size
print(f"avarage size of the word in this text is {int(sum/numwords)}")

```
