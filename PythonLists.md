##### List is a collection which is ordered and changeable. Allows duplicate members.
```python
thislist = ["apple", "banana", "cherry",3,90.0,True]
print(thislist) #output -> ['apple', 'banana', 'cherry']
print(thislist[1]) #output -> banana
len(thislist) #output -> 3
print(type(thislist)) #output -> <class 'list'>
```
##### access the item
```python
thislist1 = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
#normal index 
print(thislist1[1]) #output -> banana

#Range of Indexes
print(thislist1[2:5]) #output -> ['cherry', 'orange', 'kiwi']

#negative indexing 
print(thislist1[-1]) #output -> mango
print(thislist1[-5:-2]) #output -> ['cherry', 'orange', 'kiwi']

print(thislist1[:-1]) #output -> ['apple', 'banana', 'cherry', 'orange', 'kiwi', 'melon']
print(thislist1[-5:]) #output -> ['cherry', 'orange', 'kiwi', 'melon', 'mango']

print(thislist1[3:]) #output -> ['orange', 'kiwi', 'melon', 'mango']
print(thislist1[:5]) #output -> ['apple', 'banana', 'cherry', 'orange', 'kiwi']
```

##### list constructor
```python 
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
```

##### change list items
```python 
thislistnew= ["apple", "banana", "cherry","orange", "kiwi", "mango"]
thislistnew[1]=True
thislistnew[0]=9.0
thislistnew[-1]="blackcurrant"
thislistnew[2:4]=["watermelon",9090]
print(thislistnew) #output -> [9.0, True, 'watermelon', 9090, 'kiwi', 'blackcurrant']
```

##### insert items .insert()
```python
thislist2=["apple", "banana", "cherry"]
thislist2.insert(3,"watermelon")
print(thislist2) #output -> ['apple', 'banana', 'cherry', 'watermelon']
```
##### .append() add an item to the end of the list 
```python 
thislist21=["apple","bannana","cherry"]
thislist21.append("orange")
print(thislist21) #output -> ['apple', 'bannana', 'cherry', 'orange']
```
##### .extend(list_name) to extend a existing  list tuples dictionary sets etc
```python 
thislistx = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislistx.extend(tropical)
print(thislistx) #output -> ['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya']
```
##### Remove List Items
 remove(items) removes specified elements
 ```python 
thislist3=["apple","bannana","cherry"]
thislist3.remove("bannana")
print(thislist3) #output -> ['apple', 'cherry']
```
##### pop(index_value) removes the specified index
```python 
thislist3_1=["apple1","bannana1","cherry1"]
thislist3_1.pop(2)
print(thislist3_1) #output -> ['apple1', 'bannana1']
```
##### del ->  keyword also removes the specified index
```python 
thislist4_1=["apple","bannana","cherry"]
del thislist4_1[0]
print(thislist4_1) #output -> ['bannana', 'cherry'] 
```
##### also delete the entire list 
```python 
thislist4_1=["apple","bannana","cherry"]
del thislist4_1
```
##### clear() method empties the list.
```python 
thislistx1= ["apple", "banana", "cherry"]
thislistx1.clear()
print(thislistx1) #output -> []
```
##### looping through lists
```python 
thisList_x1 = ["apple", "banana", "cherry"]
for i in thisList_x1:
    print(i)
```
```
apple
banana
cherry
```   
##### looping through index
```python
thisList_x2=["apple1", "banana1", "cherry1"]
i=0
for i in range(len(thisList_x2)):
    print(thisList_x2[i])
```
```
apple1
banana1
cherry1
```     
##### while loop
```python 
thislist_x3=["apple2", "banana2", "cherry2",True,4.5,9090]
i=0
while i<len(thislist_x3):
    print(thislist_x3[i])
    i=i+1
```
```
 apple2
 banana2
 cherry2
 True
 4.5
 9090
```
##### checking something inside the list 
```python 
thislist2 = ["apple", "banana", "cherry"]
if "apple" in thislist:
    print("Yes, 'apple' is in the fruits list")  #output -> Yes, 'apple' is in the fruits list
```
##### Python - Sort Lists
##### .sort()
```python 
thislist1 = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist1.sort()
print(thislist1) #output -> ['banana', 'kiwi', 'mango', 'orange', 'pineapple']
```
```python 
thislist1 = [1,4,5,8,3,7,3,4,7,8]
thislist1.sort()
print(thislist1) #output -> [1, 3, 3, 4, 4, 5, 7, 7, 8, 8]
```
##### sorting in descending order 
```python 
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort(reverse = True)
print(thislist) #output -> ['pineapple', 'orange', 'mango', 'kiwi', 'banana']
```
##### customise sortimg using key = function
```python 
def myfunc(n):
  return abs(n - 50)

thislist = [100, 50, 65, 82, 23]
thislist.sort(key = myfunc)
print(thislist)   #output -> [50, 65, 23, 82, 100]
```
##### sort() method is case senstive 
```python 
thislist = ["banana", "Orange", "Kiwi", "cherry"]
thislist.sort(key = str.lower)
print(thislist) #output -> ['banana', 'cherry', 'Kiwi', 'Orange']
```
##### reverse() method reverses the current sorting order of the elements.
```python 
thislist = ["banana", "Orange", "kiwi", "cherry"]
thislist.reverse()
print(thislist) #output -> ['cherry', 'kiwi', 'Orange', 'banana']
```
##### here testList1[] is actually a reference to  test_List[]
####$ so changes made in test_List[] also affect testList1[] 
```python 
test_List=[47889734879,234234]
testList1=testList
test_List.append(232)
print(testList1) #output -> [47889734879, 234234, 232]
```
##### in order to copy list we wanna use some methods 
##### .copy()
```python 
thisList =["apple", "banana", "cherry"]
thisListnew = thisList.copy()
thisList.append('dwq')
print(thisListnew) # output -> ['apple', 'banana', 'cherry']
```
##### copy list using list()
```python 
thislist = ["apple", "banana", "cherry"]
mylist = list(thislist)
thisList.append('dwq')
print(mylist) #output -> ['apple', 'banana', 'cherry']
```

###### join two list 
##### + using concatenate 
```python 
list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3) #output -> ['a', 'b', 'c', 1, 2, 3]
```
##### for loop with .append() 
```python 
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

print(list1) #output -> ['a', 'b', 'c', 1, 2, 3]
```
##### using extends 
```python 
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list1.extend(list2)
print(list1) #output -> ['a', 'b', 'c', 1, 2, 3]
```

##### List comprehension 

##### list comprehension
```python 
thisislist_x3 = ["apple3","bannana3","cherry3"]
[print(x1)for x1 in thisislist_x3 ]
```
```output 
apple3
bannana3
cherry3
```
```python 
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)
print(newlist)  #output -> ['apple', 'banana', 'mango']
```
```python
fruits1 = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist1 = [x.upper() for x in fruits1 if "e" in x]
print(newlist1) #output -> ['APPLE', 'CHERRY']
```
```python
Qw1=[i for i in range(10) if i > 5]
print(Qw1) #output -> [6, 7, 8, 9]
```

##### list methods 
https://www.w3schools.com/python/python_lists_methods.asp
##### more about arrays     
https://www.w3schools.com/python/python_arrays.asp

