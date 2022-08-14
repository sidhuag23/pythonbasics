#### int
```python
x=-90;   
print(x,type(x)) #output->-90 <class 'int'>
```
#### float
```python
y=2.3; 
print(y,type(y)) #output->2.3 <class 'float'>
```
#### Complex numbers are written with a "j" as the imaginary part:
```python
zz=3+1j;  
print(zz,type(zz)) #output-> (3+1j) <class 'complex'>
xz=-3j;
print(xz,type(xz)) #output -> (-0-3j) <class 'complex'>
```
#### Float can also be scientific numbers with an "e" to indicate the power of 10
```python
t=2e4
print(type(t)) #output -> <class 'float'>  
a=-20E10
print(type(a)) #output -> <class 'float'>
```
#### generates random numbers
```python
import random
print(random.randrange(1, 10))  #output -> 8
```
#### Type converson
```python
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c)) 
```
