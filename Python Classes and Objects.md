##### class and objects 
everything in python  is an object with its properties and method 
A class is a blue print for creating objects 

defining a class 
```python 
class MyClass:
  x = 5

print(MyClass)
```
```console
<class '__main__.MyClass'>
```
creating an object or the instance 
```python 
class test:
  x=3

#creating object instance 
p1 = test()
print(p1.x)

p2 = test()
print(p2.x+1)
p2.x=10
print(p2.x)

p3 = test()
print(p3.x)

```
```console
3
4
10
3
```


```python
class MyClass:
  a=101010
  aDict_1={
  "T1":"0x1",
  "T2":"0x2",
  "T3":"0x3"
  }

  def hello_test(self):
    print("hello world"+str(self.a))
    print("info_print->",self.aDict_1["T1"])

  def test_New(self,x,y):
    print(x,y)

p1 = MyClass()
p1.hello_test()
p1.test_New(10,60)
```
```console
hello world101010
info_print-> 0x1
10 60
```

The _ _init_ _() Function

All classes have a function called _ _init__(), which is always executed when the class is being initiated.

Use the _ _init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created

<b>The _ _init__() function is called automatically every time the class is being used to create a new object</b>
```python 
class test:
  def __init__(self,brand,model):
    self.brand = brand
    self.model = model

  def call_model(self):
    print(f"{self.brand} {self.model}")

	#object methods 
  def test_new(self):
    print("new->update")

  def variable_update(self,x,y):
    if x == y:
      print("sync update")
    elif(x<y):
      for i in y:
        new_var=i 
        print(new_var+1)

x = test("porsche","maserati")
x.call_model()
x.test_new()
```
```console
porsche maserati
new->update
```


<b>The _ _str__() Function</b>

The _ _str__() function controls what should be returned when the class object is represented as a string.

If the _ _str__() function is not set, the string representation of the object is returned:

```python 
class test:
  def __init__(self,model,engine):
    self.model=model
    self.engine=engine
#The string representation of an object WITH the __str__() function
  def __str__(self):
    return f"{self.model}{self.engine}"

p1 = test("test ","v12")
print(p1) #output test v12
```

##### The self Parameter
The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:

```python 
class Person:
  def __init__(mysillyobject, name, age):
    mysillyobject.name = name
    mysillyobject.age = age

  def myfunc(abc):
    print("Hello my name is " + abc.name)

p1 = Person("John", 36)
p1.myfunc()
```

```python 
class test:
  def __init__(testThis,x,y):
    testThis.x=x+1
    testThis.y=y+2
    print("x = ",x)
    print("y =", y)

    print("testThis.x = ",testThis.x)
    print("testThis y = ",testThis.y)


  def selfTest(testThis):
    return f"{testThis.x+testThis.y}"


p2 = test(4,4)

print(p2.selfTest())
```
```console
x =  4
y = 4
testThis.x =  5
testThis y =  6
11
```


##### pass Statement
class definitions cannot be empty if you dont have any statements in the class use pass statement to avoid error
```python
class Person: 
  pass
```

##### delete object Properties
```python
del ObjectName.age
```
#### delete entire object 
```python
del ObjectName 
```
