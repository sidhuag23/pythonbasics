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

