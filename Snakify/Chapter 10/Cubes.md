# Unit 10 Prolem 5
```.py
n,m=[int(j) for j in input().split()]
alice=set()
bob=set()
for i in range(n):
    alice.add(int(input()))
for i in range(m):
    bob.add(int(input()))
intrs= alice&bob
jstalice=alice-bob
jstbob=bob-alice
print(len(intrs))
print(*sorted(intrs))
print(len(jstalice))
print(*sorted(jstalice))
print(len(jstbob))
print(*sorted(jstbob))
```
