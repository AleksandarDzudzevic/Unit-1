```.py
protein=str(input())
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
