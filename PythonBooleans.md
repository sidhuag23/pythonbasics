#### Boolean Values 
boolean values are either True or False -> 1 and 0
```python 
print(10 > 9) #output -> True
print(10 == 9) #output -> False 
print(10 < 9) #output -> False 
```
##### most will return True
```python
bool("abc")
bool(123)
bool(["apple", "cherry", "banana"]) 
```
##### will return False
```python
bool(False)
bool(None)
bool(0)
bool("")
bool(())
bool([])
bool({}) 
```
##### object always returns true
```python
class Test:
    def __init__(self,testString):
        print("hello worlf",testString )
    def testDifferentmMethod(self,tetsAcrh):
        print(tetsAcrh)
    def test(self):
        print(23)

new_ob = Test("tqwe")
new_ob.testDifferentmMethod("p")
new_ob.test()
print(bool(new_ob))
```
```output 
hello worlf tqwe
p
23
True
```
##### object with __len__ function returns false 
```python
class myclass():
  def __len__(self):
    return 0

myobj = myclass()
print(bool(myobj)) #output -> False 
```
##### functions that returns a Boolean Value
```python
def myfunction():
    return True

if myfunction():
    print("YES")
else:
    print("NO")

    #output -> YES
```
