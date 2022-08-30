#####  tuples 
Tuples -> are order and unchangeable allow duplicates , access by indexing
use () brackets 

```python 
thistuple = ("banana", "banana", "cherry", "apple", "cherry",True,23,23.0)
print(thistuple) #output -> ('banana','banana', 'cherry', 'apple', 'cherry', True, 23, 23.0)
print(type(thistuple)) #output -> <class 'tuple'>
print(len(thistuple)) #output -> 8
```
#####  constructor tuples 
```python 
thistuple = tuple(("apple", "banana", "cherry")) # note the double round-brackets
print(thistuple) #output -> ('apple', 'banana', 'cherry')
```
##### access by indexing 
```python 
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
 print(thistuple[1])  #output ->  banana
 print(thistuple[2:5]) #output -> ('cherry', 'orange', 'kiwi')
 print(thistuple[:4]) #output ->  ('apple', 'banana', 'cherry', 'orange')
 print(thistuple[2:]) #output ->  ('cherry', 'orange', 'kiwi', 'melon', 'mango'
    
#### negative indexing 
 print(thistuple[-1])    #output -> mango
 print(thistuple[-4:-1]) #output -> ('orange', 'kiwi', 'melon')
 print(thistuple[:-4])   #output -> ('apple', 'banana', 'cherry')
 print(thistuple[-2:])   #output -> ('melon', 'mango')
```
##### check if apple is present in the tuples
```python 
thistuple = ("apple", "banana", "cherry")
if "apple" in thistuple:
  print("Yes, 'apple' is in the fruits tuple") #output ->  Yes, 'apple' is in the fruits tuple
```
##### adding items in tuples 
```python 
x = ("apple", "banana", "cherry")
x[1] = "213wqwd"
print(x) #output -> 'tuple' object does not support item assignment
```
convert to list then change 
```python 
x = ("apple", "banana", "cherry")
y = list(x)
y[1] = "kiwi"
x = tuple(y)
print(x)
```
 #####  add items to the tuples first convert to list then add items using .append(item)
 ```python 
 thistuple = ("apple", "banana", "cherry")
 y = list(thistuple)
 y.append("orange")
 thistuple = tuple(y)
 print(thistuple) #output -> ('apple', 'banana', 'cherry', 'orange')
```
##### add tuples to a tuple (which is legal)
```python 
thistuple = ("apple", "banana", "cherry")
y = ("orange","yewdd2")
thistuple = thistuple + y  #thistuple += y

print(thistuple) #output -> ('apple', 'banana', 'cherry', 'orange', 'yewdd2')
```

##### Convert the tuple into a list, remove "apple", and convert it back into a tuple
```python 
thistuple = ("apple", "banana", "cherry")
y = list(thistuple)
y.remove("apple")
thistuple = tuple(y)
print(thistuple) #output -> ('banana', 'cherry')
```
##### delete tuple complete
```python 
thistuple = ("apple", "banana", "cherry")
del thistuple
print(thistuple) #this will raise an error because the tuple no longer exists 
```
'tuple' object doesn't support item deletion
```python 
thistuple = ("apple", "banana", "cherry")
del thistuple[1]
print(thistuple) #output -> tuple' object doesn't support item deletion
```
##### unpack tuples extracting values to variable 
```python 
fruits = ("apple", "banana", "cherry")

x, y, z = fruits

print(x) #apple
print(y) #banana
print(z) #cherry
```
(*) use to add extra value to that particular values inside a list format
```python 
fruits = ("apple", "banana", "cherry","213213",True)

x, y, *z = fruits

print(x) #output -> apple
print(y) #output -> banana
print(z) #output -> ['cherry', '213213', True]
```
##### Loops tuples 
normal
```python
thistuple = ("apple", "banana", "cherry")
for x in thistuple:
  print(x) 
```
```output 
apple
banana
cherry
```

index Numbers
```python 
thistuple = ("apple", "banana", "cherry")
for i in range(len(thistuple)):
  print(thistuple[i])
```
```output 
apple
banana
cherry
```

while loop 
 ```python 
thistuple = ("apple", "banana", "cherry")
i = 0
while i < len(thistuple):
  print(thistuple[i])
  i = i + 1 
```
```
apple
banana
cherry
```
##### Join Two Tuples
```python 
tuple1 = ("a", "b" , "c")
tuple2 = (1, 2, 3)

tuple3 = tuple1 + tuple2
print(tuple3) #output -> ('a', 'b', 'c', 1, 2, 3)
```
##### Multiply Tuples
```python 
fruits = ("apple", "banana", "cherry")
myt = fruits * 2

print(myt) #output -> ('apple', 'banana', 'cherry', 'apple', 'banana', 'cherry')

```
https://www.w3schools.com/python/python_tuples_methods.asp
