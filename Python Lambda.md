##### Python Lambda
lambda function is a small anonymous function.
lambda function can take any number of arguments, but can only have one expression
```
lambda arguments : expression
```

```python
x = lambda a : a+20*10
print(x(5)) 
```

```console 
 205
```

```python
y = lambda e,n: e*n 
print(y(10,11))
```
```console 
110
```
 
Lambda Functions inside basic functions 
```python
def xtest(n):
  return lambda a : a * n

double1=xtest(2)
tripler2=xtest(3)

print(double1(11))
print(tripler2(11))
```
```console 
22
33
```

