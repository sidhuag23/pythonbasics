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


