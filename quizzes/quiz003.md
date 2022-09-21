# Quiz 3
### Given a protein that consists of A,T,C,G return a protein that changes A->T, C->G, T->A, G->C.       
### Print the changed protein.
Code for the following problem:
```.py
protein=str(input("Enter the starting protein"))
protein2=""
for i in range(0,len(protein)):
    if protein[i]=="A":
        protein2=protein2+"T"
    if protein[i]=="G":
        protein2=protein2+"C"
    if protein[i]=="T":
        protein2=protein2+"A"
    if protein[i]=="C":
        protein2=protein2+"G"
print(protein2)
```
![Successful test](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/Quiz003test.png)
### Flow diagram
![](https://github.com/AleksandarDzudzevic/Unit-1/blob/main/quiz003flowdiagram.jpg)
