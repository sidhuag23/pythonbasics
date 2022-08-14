#### datatypes in python 
Variables can store data of different types, and different types can do different things.
<pre>
Text Type      =	str<br>
Numeric Types  = 	int, float, complex <br>
Sequence Types = 	list, tuple, range <br>
Mapping Type   =        dict <br>
Set Types      =        set, frozenset <br>
Boolean Type   =	bool <br>
Binary Types   = 	bytes, bytearray, memoryview <br>
None Type      = 	NoneType <br>
</pre>

#### Getting the Data Type
type() function:
```python
x=90;
print(type(x)) #output -> <class 'int'>
```

#### setting data types 
```python
x = "Hello World" 	              #  str 	
x = 20 	                           #     int 	
x = 20.5 	                        #float 	
x = 1j 	                               # complex 	
x = ["apple", "banana", "cherry"] 	#list 	
x = ("apple", "banana", "cherry") 	#tuple 	
x = range(6) 	                       # range 	
x = {"name" : "John", "age" : 36} 	#dict 	
x = {"apple", "banana", "cherry"} 	#set 	
x = frozenset({"apple", "banana", "cherry"})  	#frozenset 	
x = True                           	#bool 	
x = b"Hello" 	                        #bytes 	
x = bytearray(5) 	                  #bytearray 	
x = memoryview(bytes(5))           	#memoryview 	
x = None 	                          #NoneType 	
```

#### setting spefic datatype 
```python3
x = str("Hello World")                 	   # str 	
x = int(20) 	                            # int 	
x = float(20.5) 	                        #float 	
x = complex(1j) 	                        #complex 	
x = list(("apple", "banana", "cherry")) 	#list 	
x = tuple(("apple", "banana", "cherry")) 	#tuple 	
x = range(6) 	#range 	
x = dict(name="John", age=36) 	#dict 	
x = set(("apple", "banana", "cherry")) 	#set 	
x = frozenset(("apple", "banana", "cherry")) 	#frozenset 	
x = bool(5) 	#bool 	
x = bytes(5) 	#bytes 	
x = bytearray(5) 	#bytearray 	
x = memoryview(bytes(5)) #	memoryview
```
