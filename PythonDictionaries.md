
##### Dictionaries are used to store data values in key:value pairs.

A dictionary is a collection which is ordered*, changeable and do not allow duplicates.
```python 
 thisdict = {
   "brand": "Ford",
   "model": "Mustang",
   "year": 1964,
   1:1964,
   False:13.23,
   2.1:True,
   "colors": ["red", "white", "blue"],
   3.1: ("red", "white", "blue") ,
   4.4: {"colors","red", "white", "blue"},
   5.5:{
         "brand": "Ford",
         "model": "Mustang",
         "year": 1964,        
      },
   3+4j : 12  
}
print(thisdict)
print(type(thisdict)) #output -> <class 'dict'>
print(len(thisdict)) #output -> 11
print(thisdict["colors"]) #output -> ['red', 'white', 'blue']
```
```output 
{'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 1: 1964, False: 13.23, 2.1: True, 'colors': ['red', 'white', 'blue'], 3.1: ('red', 'white', 'blue'), 4.4: {'colors', 'red', 'blue', 'white'}, 5.5: {'brand': 'Ford', 'model': 'Mustang', 'year': 1964}, (3+4j): 12}
<class 'dict'>
11
['red', 'white', 'blue']
``` 

##### Access Dictionary Items
```python
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["model"] #output->'Mustang'
thisdict.get("model") #output-> 'Mustang'
thisdict.keys() #output-> dict_keys(['brand', 'model', 'year'])
thisdict.items() #output -> dict_items([('brand', 'Ford'), ('model', 'Mustang'), ('year', 1964)])
thisdict.values() #dict_values(['Ford', 'Mustang', 1964])
```
##### Python - Change Dictionary Items
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["year"] = 2018
print(thisdict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 2018}

```
.update()
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"year": 2020})
print(thisdict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 2020}
```

##### Python - Add Dictionary Items
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["color"] = "red"
print(thisdict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'color': 'red'}
```
.update()
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"color": "4t98054"})
print(thisdict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'color': '4t98054'}
```
##### Removing Items
#####  removes the item with the specified key name
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.pop("model")
print(thisdict) #output -> {'brand': 'Ford', 'year': 1964}
```
#####  popitem() method removes the last inserted item
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.popitem()
print(thisdict) #output -> {'brand': 'Ford', 'model': 'Mustang'}
```
##### del keyord removes the item with the specified key name
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict["model"]
print(thisdict) #output -> {'brand': 'Ford', 'year': 1964}
```
##### del keyword can also delete the dictionary completely
```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict
print(thisdict) #this will cause an error because "thisdict" no longer exists.
```
##### clear() method empties the dictionary
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.clear()
print(thisdict) #output -> {}
```
##### Python - Loop Dictionaries
```python 
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": "1964"
}
for x in thisdict:
    print(x,end=" ") #output -> brand model year 

print("\n")
for x in thisdict:
    print(thisdict[x],end=" ") #output -> Ford Mustang 1964 
    
print("\n")    
for x in thisdict.values():
    print(x,end=" ")   #output -> Ford Mustang 1964
    
print("\n")    
for x in thisdict.keys():
    print(x,end=" ")  #output -> brand model year 
    
print("\n")    
for x,y in thisdict.items():
    print(x+":"+y,end=" ")  #output -> brand:Ford model:Mustang year:1964 

```

##### Copy a Dictionary
##### copy()
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = thisdict.copy()
print(mydict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 1964}
```
##### dict()
```python 
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = dict(thisdict)
print(mydict) #output -> {'brand': 'Ford', 'model': 'Mustang', 'year': 1964}
```
##### Nested Dictionaries
```python 
child1 = {
  "name" : "Emil",
  "year" : 2004
}
child2 = {
  "name" : "Tobias",
  "year" : 2007
}
child3 = {
  "name" : "Linus",
  "year" : 2011
}

myfamily = {
  "child1" : child1,
  "child2" : child2,
  "child3" : child3
}
print(myfamily) #output -> {'child1': {'name': 'Emil', 'year': 2004}, 'child2': {'name': 'Tobias', 'year': 2007}, 'child3': {'name': 'Linus', 'year': 2011}}

```
##### check whether something exist 
```python 
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
if "model" in thisdict:
  print("Yes, 'model' is one of the keys in the thisdict dictionary") #output -> Yes, 'model' is one of the keys in the thisdict dictionary

```
```python 
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
if "Ford" in thisdict.values():
  print("Yes, 'Ford' is one of the keys in the thisdict dictionary") #output -> Yes, 'Ford' is one of the keys in the thisdict dictionary

```
