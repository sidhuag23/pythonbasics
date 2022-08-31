A set is a collection which is unordered, unchangeable*, unindexed ,do not allow duplicate values.
 Set items are unchangeable, but you can remove items and add new items.
```python 
thisset = {1,"apple", "banana", "cherry",232,True,0,"p",2}
print(thisset) #output -> {0, 1, 2, 'p', 'cherry', 232, 'apple', 'banana'}
print(type(thisset)) #output -> <class 'set'>
print(len(thisset)) #output -> 8
```
#####  The set() Constructor
```python 
thisset = set(("apple", "banana", "cherry")) # note the double round-brackets
print(thisset) 
```
#####  loop through sets 
```python 
thisset = {"apple", "banana", "cherry"}
for x in thisset:
  print(x) 
```
```output 
banana
apple
cherry
```
##### check if something exist
```python 
thisset = {"apple", "banana", "cherry"}
print("banana" in thisset) #output -> True
```

##### add items using add()
```python 
thisset = {"apple", "banana", "cherry"}
thisset.add("orange")
print(thisset) #output -> {'orange', 'banana', 'apple', 'cherry'}
```
##### Add Any Iterable(tuples, lists, dictionaries etc.) to a set
```python 
thisset = {"apple", "banana", "cherry"}
tropical = {"pineapple", "mango", "papaya"}
mylist = ["kiwi", "orange",67]

thisset.update(tropical)
thisset.update(mylist)
print(thisset)  #output -> {67, 'orange', 'cherry', 'pineapple', 'mango', 'apple', 'kiwi', 'banana', 'papaya'}
```
##### Remove Item  using the remove()
```python 
thisset = {"apple", "banana", "cherry"}
thisset.remove("banana")
print(thisset) #output -> {'apple', 'cherry'}
```
##### Remove Item using the discard() method:
```python 
thisset = {"apple", "banana", "cherry"}
thisset.discard("banana")
print(thisset) #output -> {'apple', 'cherry'}
```
##### Remove the last item by using the pop() method
```python 
thisset = {"apple", "banana", "cherry"}
x = thisset.pop()
print(x) #output -> banana
print(thisset)#output -> {'apple', 'cherry'}
```
##### clear() entire set
```python 
thisset = {"apple", "banana", "cherry"}
thisset.clear()
print(thisset)  #output -> set()
```
##### del -> keyword will delete the set completely
```python 
thisset = {"apple", "banana", "cherry"}
del thisset
```
#####  union() method that returns a new set containing all items from both sets
```python 
set1 = {"a", "b" , "c"}
set2 = {1, 2, 3,4}

set3 = set1.union(set2)
print(set3) #output -> {'a', 1, 2, 3, 'b', 4, 'c'}
```
##### update() method inserts the items in set2 into set1:
```python 
set1 = {"a", "b" , "c"}
set2 = {1, 2, 3,9090}

set1.update(set2)
print(set1) #output -> {'a', 1, 2, 3, 'b', 9090, 'c'}
```
###### intersection_update() -> method will keep only the items that are present in both sets.
```python 
x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

x.intersection_update(y)

print(x) #output -> {'apple'}
```
##### intersection() method will return a new set, that only contains the items that are present in both sets
```python 
x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

z = x.intersection(y)

print(z) #output -> {'apple'}
```
###### symmetric_difference_update() method will keep only the elements that are NOT present in both sets.
```python 
x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

x.symmetric_difference_update(y)

print(x) #output -> {'cherry', 'microsoft', 'banana', 'google'}
```
##### symmetric_difference() method will return a new set, that contains only the elements that are NOT present in both sets
```python 
x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

z = x.symmetric_difference(y)

print(z) #output -> {'cherry', 'microsoft', 'banana', 'google'}
```
Python - Set Methods
https://www.w3schools.com/python/python_sets_methods.asp
