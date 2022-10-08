![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz016text.png)
```.py
def blackboxthree(given:str)->str:
    output=''
    x=[]
    for letter in given.lower():
        if letter.isalpha():
            found=False
            for element in x:
                if element[0]==letter:
                    element[1]+=1
                    found=True
                    output+=str(element[1])
            if found==False:
                x.append([letter,1])
                output+="1"
        else:
            output+=letter
    return output
print(blackboxthree("hello world"))
```
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz016test.png)
