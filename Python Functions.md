##### Normal functions 
```python 
def my_function():
  print("hello world")

my_function()
```
```console
 hello world
```

#### parameters and arguments 
```python 
def testAutoInfo(car_name,car_engine,car_price): #parameters
  
  list_details = [car_name,car_engine,car_price]
  print("\nyour car details")
  for x in list_details:
    print(x,end=" ")
  

testAutoInfo("BMW","v12","1234") #arguments 
testAutoInfo("Audi","v8","12Lakhs")
```
```console
your car details
BMW v12 1234 
your car details
Audi v8 12Lakhs 
```
#### Arbitrary Arguments, *args
If you do not know how many arguments that will be passed into your function, add a * before the parameter name in the function definition.
function will receive a tuple of arguments, and can access the items accordingly

```python 
def my_function(*x):
  print(x) #function will receive a tuple of arguments
  for i in x:
    print(i)

my_function(1,"1we",3j,4,5)
my_function(23,"12wqa",334,2j)
```
```console
(1, '1we', 3j, 4, 5)
1
1we
3j
4
5
(23, '12wqa', 334, 2j)
23
12wqa
334
2j

```

##### keyword arguments 
#### key = value syntax
```python 
def my_function(T1,T2,T3,T4):
  print("fn = "+T1)
  print("fn2 = "+ str(T4))

my_function(T1="@we",T2="12",T3=12330,T4=12+1j)
```
```console
fn =@we
fn2 =(12+1j)
```

##### Arbitrary Keyword Arguments, **kwargs
#### key = value pair format 
If you do not know how many keyword arguments that will be passed into your function, add two asterisk: ** before the parameter name in the function definition
```python 
def test(**test1):
  print(type(test1))
  for i,y in test1.items():
    print(i+" "+str(y))

test(BrandName="Audi",CarName="A8L",Engine="v12")
test(BrandName="BMW",CarName="780li",Engine="v8")
```
```console
<class 'dict'>
BrandName Audi
CarName A8L
Engine v12
<class 'dict'>
BrandName BMW
CarName 780li
Engine v8
```
##### default parameter  and return value 
```python 
#we can also set default value for our paramaters 
def my_function(x=5):
  return 5*x  # will return some value 

print(my_function(3))
print(my_function())
```
```console
15
25
```
##### pass statement 
 if no statement just put pass in there
```python
def test_this():
  pass

test_this()
```

##### Recursion
function calls itself
based on stack 
with no base condition causes something called stack overflow
```python
def testQ(n):
  print(n)
  if n>1:
   testQ(n-1)

testQ(5)
```
```console
5
4
3
2
1
```
```python
def testA(i):
  print(i)
  if i<10:
    testA(i+1)

testA(1)
```
```console
1
2
3
4
5
6
7
8
9
10
```
```python
def Test1(k):
  if k>0:
    val=k+Test1(k-1)
    print(val)
  else:
    val=0
  return val

Test1(6)
```
```console
1
3
6
10
15
21
```

