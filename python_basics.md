#### basics python
```python
print("hello worlfd")
```
#### variables in python
```python
x = 5
y = "John"
z=3.0
print(x,y,z)
```
#### type casting
```python
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0 
```
#### many values to multpile variables 
```python
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```
#### one value to multiple variable
```python
x=y=z="orange"
print(x)
print(y)
print(z)
```

#### unpack values
```python
fruits = ["apple","bannan","cherry"]
x,y,z=fruits
print(x)
print(y)
print(z)
```
#### + operator (for adding and concatating )
```python
x = 5
y = 10
print(x + y)

x = "Python "
y = "is "
z = "awesome"
print(x + y + z)

x = "Python "
y = 78
z = "awesome"
print(x + str(y) + z)
```
#### global and local variable 
```python
x = "awesome" #global variable 

def myfunc():
  x = "fantastic"
  y = 78 #local variable 
  print("Python is " + x,y)

myfunc()

print("Python is " + x) 

### The global Keyword
def myfunc():
  global x
  x = "fantastic"

myfunc()


print("Python is " + x) 
```
#### comments 
```python
#single line comment
'''
multi 
   line 
      comment 
'''
```
