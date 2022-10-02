<pre>

    Equals: a == b
    Not Equals: a != b
    Less than: a < b
    Less than or equal to: a <= b
    Greater than: a > b
    Greater than or equal to: a >= b


</pre>
#### normal if statements 
```python

a = 33
b = 200
if b>a:
    print("b is big")
elif a==b:
    print("a and b equal ")
else:
    print("a is big ")  
    
#output -> b is big

```
#### short hand else if 
```python
a=20
b=330
print("A") if a > b  else print("B")
#output -> B
```

#### short hand syntax only useful if you use one statement 
```python
a = 33
b = 200
if b>a: print("b is big")
elif a==b: print("a and b equal ")
else: print("a is big ")
#output -> b is big
```

#### nested if statements 
```python
a=33
b=200
c=500
if b>a and c>b:
    print("b is good")
    if not(a==b) and not(a>b):
        print("great")
    else:
        print("ok")
else:
    print("buy")
    
#output -> b is good
#           great
```
#### logical operations 
```python
not(1==9) and not(3==9 or 3==3) #output -> False
```
#### pass if no statements 
```python
if 5==5:
    pass
else:
    print("no")
```
