# Email generator 
## Make isak email
### Given the first name, last name and gradutaion year print isak email address
```.py
year=input()
name=input()
lastname=input()
print(f"{year}.{name}.{lastname}@uwcisak.jp")
```
## Make a menu that shows 5 different email ideas
### Given the first name, last name and gradutaion year print isak email address
```.py
year=input()
name=input()
lastname=input()
print(f"The email {year}.{name}.{lastname}@uwcisak.jp is not available choose one of these insted:")
print("Click the number in front of the option that you like the most")
print("1. gradyear.lastname.firstname@uwcisak.jp ")
print("2. lastname.firstname.gradyear@uwcisak.jp ")
print("3. firstname.gradyear.lastname@uwcisak.jp ")
print("4. firstname.lastname.gradyear@uwcisak.jp ")
print("5. lastname.gradyear.firstname@uwcisak.jp ")
x=int(input())
print("YOUR NEW EMAIL IS:")
if x==1:
    print(f"{year}.{lastname}.{name}@uwcisak.jp")
if x==2:
    print(f"{lastname}.{name}.{year}@uwcisak.jp")
if x==3:
    print(f"{name}.{year}.{lastname}@uwcisak.jp")
if x==4:
    print(f"{name}.{lastname}.{year}@uwcisak.jp")
if x==5:
    print(f"{lastname}.{year}.{name}@uwcisak.jp")
```
