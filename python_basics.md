##### python basics 

python basics 
#### variables 
variable are way to store data 
```console
Python 3.9.2 (default, Feb 28 2021, 17:03:44)
[GCC 10.2.1 20210110] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> x = "hello world"
>>> print(x)
hello world
>>> x = "bye"
>>> print(x)
bye
```
#### strings
"strings" enclosed in quotes  
```console
>>> x = "helloworld"
>>> print(x)
helloworld
>>> type(x)
<class 'str'>
>>> type("100")
<class 'str'>
>>> "100"+"29090"
'10029090'
>>> len("hello world")
11
>>>
```
##### numbers
```
>>> a = 10
>>> type(a)
<class 'int'>
>>> type(-100)
<class 'int'>
>>> type(0)
<class 'int'>
>>> type(90.0)
<class 'float'>
>>> "100"+"100"
'100100'
>>> 100+100
200
>>>
```

#### build in function in python 
```python
# built in function 
print(type(10))

#will shows list of built in functions 
dir(__builtins__)

#to get more info about a built in function
help(len) #gets help or more details of the len function 
```
```console
>>> int(10.5)
10
>>> round(10.6)
11
>>> round(10.2)
10
>>> int("100")+100
200
>>> float("100.10")
100.1
>>> float("100.10")
100.1
>>> str(10)
'10'
>>> type(10)
<class 'int'>
>>> type(10.33)
<class 'float'>
```
#### python list and indexing
```python
listx = ["hello","world",1,2,3,4,4554]
print(listx)

listx[1] #accessing via index value 

for i in listx:
    print(i)  #printing each element using for each loop

#printing eaach element using while loop
i=0
while i<len(listx):
    print(listx[i])
    i=i+1
    
#accessing each chaacter of string using index position
"helloworld"[2]

#printing each character using for - each loop
for i in "helloworld":
    print(i)
```

To perform math operations you can use math operators. The following examples cover all basic math operators (+, -, *, /, **):


Addition
```console
>>> 1 + 3.5 
4.5 
```

Subtraction
```console
>>> 1 - 3.5 
-2.5 
```

Multiplication
```console
>>> 1 * 3.5 
3.5 
```

Division
```console
>>> 1 / 3.5 
0.2857142857142857 
```

Exponentiation (3 * 3 * 3 * 3)
```console
>>> 3 ** 4 
81 
```

Order of operations

The order of operations is (1) exponentiation, (2) multiplication, (3) division, (4) addition, and (5) subtraction.


For example, in the following expression we have exponentiation, multiplication and addition:
```console
>>> 1 + 2 * 10**2 
201 
```
You get 201 because first we get 100 from 10**2 (exponentiation), and then we get 200 from 2 * 100 (multiplication), and finally 201 from 1 + 200 (addition).

You can control what to execute first by using parenthesis:
```console
>>> (1 + 2) * 10**2 
300 
```

You get 300 because first we get 3 from 1 + 2, and then we get 100 from 10**2 and finally 300 from 3 * 100.


#### list and list slicing 
```python
address=["address",1,"Newyork",12]

#check type of each list elements 
type(address[1]) #output -> int

#we can do mathematical operations which list value 
address[1]*399/2

#gets the last element if we use the [-1] -negative indexing 
print(address[-2]); #output -> "Newyork" 
print(address[-1]); #output -> 12

#list slicing 

#returns an another list with the values between list [1] to list  [3]
address[1:3] #output -> [1, 'Newyork']

#returns everything inside the list
address[:] #output -> ['address', 1, 'Newyork', 12]

#returns all elements starting form index postion [2] 
address[2:] #output -> ['Newyork', 12]

#returns all elements up to index position [3]
address[:3] #output -> ['address', 1, 'Newyork']

#slicing elements from backwards using negative indexing 
address[:-1] #output -> ['address', 1, 'Newyork']

address[:-2] #output -> ['address', 1]

address[-3:-1] #output -> [1, 'Newyork']

address[-3:] #output -> [1, 'Newyork', 12]

address[-2:] #output -> ['Newyork', 12]

```
#### some build in list methods

```python
days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"] 

#.appends("element") adds an element to the list at the end 
days.append("funday")
print(days) #output -> ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun', 'funday']

#.removes("element") removes an element 
days.remove("Mon")
print(days) #output -> ['Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun', 'funday']

#to check the list of built in function/methods avialble for lists
dir(list)

dir(days)

```

##### lists 
starts with [0] indexing
```python
address = ['porsche','bmw','maybach','lamborghini']
print(address[2],address[1])   #output->maybach bmw

#strings can be also used with this indexing system
x="hello word"
print(x[1])  #output->e

"hello world"[3]  #output->'l'
```
we can do different operations with lists
```python
address = ['porsche','bmw','maybach','lamborghini',90,1000,200]
address[4]+address[5]+100  #output->1190 
address[0]+address[2]  #output->'porschemaybach'
```
##### to count list item backwards use (-)negative symbol in front of the index labeling 
##### eg xyz[-1] -> gets last item in the list xyz 
##### also known as negative indexing
```python
address = ['porsche','bmw','maybach','lamborghini',90,1000,200]
address[-1] #output-> 200
address[-2] #output-> 1000
address[-2] #output-> 1000
address[-0] #output->'porsche'
address[-5] #output ->'maybach'
```
##### list slicing 
#### slicing list in between return different list
```python
address = ['porsche','bmw','maybach','lamborghini',90,1000,200]
address[1:5]  #returns list elements from 1 to 5
address[5:1]  #returns nothing
address[1:] #returns list elements from index 1 to everything
address[4:] #returns list elements from index 4 to everything
address[:5] #returns list elements from the starting index up to index 5
address[:0] #returns nothing
address[0:] #returns list elements from index 0 to everything 
address[-1:-5] #returns nothing
address[-1:] #returns only the last element
address[:-1]#returns everything execpt the last one 
address[:-2] #returns -> ['porsche', 'bmw', 'maybach', 'lamborghini',90]
address[-2:]  #returns ->[1000, 200]
address[-2:-5] #returns nothing
address[-5:-2] #returns -> ['maybach', 'lamborghini', 90]
address[-6:-1] #returns -> ['bmw', 'maybach', 'lamborghini', 90, 1000]
```
Here are more examples of slicing lists if you're still not sure how slicing works.

Let's suppose we have the following list in our Python shell:
```python
>>> days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"] 
```
Here is how to access the first three items (from first to third):
```python
>>> days[0:3] 

Output:
['Mon', 'Tue', 'Wed'] 
```
Access items from first to fourth:
```python
>>> days[0:4] 
['Mon', 'Tue', 'Wed', 'Thu'] 
```
Exactly the same as above
```python
>>> days[:4] 
['Mon', 'Tue', 'Wed', 'Thu'] 
```
No boundaries
```python
>>> days[:] 
['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'] 
```
From first to second-to-last
```python
>>> days[0:-1] 
['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'] 
```
From first to third-to-last
```python
>>> days[:-2] 
['Mon', 'Tue', 'Wed', 'Thu', 'Fri'] 
```
From third-to-last to second-to-last
```python
>>> days[-3:-1] 
['Fri', 'Sat'] 
```
From third-to-last to last
```python
>>> days[-3:] 
['Fri', 'Sat', 'Sun'] 
```

#### list method (method a function that applies to the data object)
```python
x=["porsche","maybach","lamborghii",903,3,3444]
dir(x) #show all method you can apply to that particular list

dir(list) #show all method you can apply to that particular list

x.append("USA") #adds new element to the list at last position
print(x)

x.remove("porsche") #removes an element inside the list
print(x)

x.pop(2) #removes the 2second element
print(x)
```
##### tuples 
There's another datatype in Python called a tuple :
```python
mytuple = (1, 2, "Three") 
```
It's exactly like a list  except:

1. You use parenthesis instead of square brackets to define the tuple.

2. A tuple is not mutable which means you can't append or remove items from tuples, like you can with lists. Trying add an append method to a tuple would throw an error:

```python
>>> mytuple = (1, 2, "Three") 
>>> mytuple.append("Four")
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'tuple' object has no attribute 'append'
```

Tuples are rarely used. However, if you ever need a list that you really don't want to be changed, using a tuple instead of a list is a good idea.

#### dictionary key:value pair
```python
test={ 
    "bmw":6 , 
    "porsche":90 , 
    "lamborghini":90440 
    }


test["bmw"]  #accessing via key 
type(test["bmw"]) #output -> <class 'int'>

test.keys() #output -> dict_keys(['bmw', 'porsche', 'lamborghini'])

test.values() #output -> dict_values([6, 90, 90440])
```
Here are more operations you can do with dictionaries

Let's say we have the following dictionary:
```python
>>> person97 = {"name":"Jack", "surname":"Smith", "age":"29"} 
```
Removing pair "name":"Jack"
```python
>>> person97.pop("name") 
'Jack' 
>>> person97 
{'surname': 'Smith', 'age': '29'} 
```
Adding new pair "name":"Jack"
```python
>>> person97["name"] = "Jack" 
>>> person97 
{'surname': 'Smith', 'age': '29', 'name': 'Jack'} 
```
Changing an existing value
```python
>>> person97["age"] = 30 
>>> person97 
{'surname': 'Smith', 'age': 30, 'name': 'Jack'} 
```
Mapping two lists to a dictionary:
```python
>>> keys = ["a", "b", "c"] 
>>> values = [1, 2, 3] 
>>> mydict = dict(zip(keys, values)) 
>>> mydict 
{'a': 1, 'b': 2, 'c': 3} 
```
##### input() takes input
##### input() generally input() always converts to string so we wanna do sometype convertion
```python
user_input=int(input("enter your number"))
print(user_input**2)

#### some comparsion operator
"1234"==1234  #false
"1234"=="1234" #true



1234==1234  #true
1234<=1234  #true
1234<1234 #false
3>4 #false
23<9090 #true
```
#### conditionals 

```python
dict_test={ "mike":1234,"joe":1111,"jack":2333 } 
dict_test.values() #output -> dict_values([1234, 1111, 2333])
test1=1111 
#use (in) to check stuff is inside 
test1 in dict_test.values() #output -> True
```
#### if elif statement 
```python
x=2
if x==1:
    print("1")
elif x>1:
    print("2")
else:
    print("sprry")
```

#### functions 

##### built in function
```python 
len("hdejkhdkj") #output -> 9
```
##### custom function 
```python
def test(year): #parameter (in function definition)
    age = 2018-year
    return age 

x = test(1945) #passing arguments (in function call)
print(x)
type(test(1885)) #output -> int (function returns a integer)
```

#### custom function (without return type)
```python 
def sayhi(t,z=10):  #more than one parameter
    print("test thsisdnjk "+str(t),str(z))

#NoneType (function returns a None) 
type(sayhi(5)) #output ->test thsisdnjk5 10 
type(sayhi(23,90)) #output -> test thsisdnjk 23 90

```
##### function example 

```python 
def string_length(mystring):
     if type(mystring) == int:
         return "Sorry, integers don't have length"
     elif type(mystring) == float:
         return "Sorry, floats don't have length"
     else:
         return len(mystring)
    
string_length("helllo") #output -> 6
string_length(4) #output -> "Sorry, integers don't have length"
string_length(8.0) #output -> "Sorry, floats don't have length"

int==type(3) #true 
type(3)==type(3.0) #False 
```


