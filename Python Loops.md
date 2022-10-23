##### while Loop
```python

i = 1
while i<=6:
	print(i)
	i=i+1
```
```output
1
2
3
4
5
6
```

##### break Statement
```python 
i=1
while i<6:
	print(i)
	if i == 3:
		break
	i+=1
```
```output 
1
2
3
```

##### The continue Statement
```python 
i=0
while i<=6:
	i+=1
	if i == 3:
		continue  
	print(i)
```
```output
1
2
4
5
6
7
```
##### The else Statement
```python 
i = 1
while i <=6:
	print(i)
	i+=1
else:
	print("i is no longer less than "+str(i))
```
```output 
1
2
3
4
5
6
i is no longer less than 7
```
##### Python For Loops

##### iterate through list 
```python 
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
```
```output 
apple
banana
cherry
```


##### Python For Loops
##### Looping Through a String
```python 
for x in "banana":
  print(x)
```
```output 
b
a
n
a
n
a
```

##### The break Statement
statement we can stop the loop before it has looped through all the items:
```python 
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```
```output 
apple
banana
```
```python 
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    break
  print(x)
```
```output
apple
```
####  continue Statement
statement we can stop the current iteration of the loop, and continue with 
```python 
fruits = ["apple", "banana" ,"qw1","cherry"]
for x in fruits:
  if x == "banana":
    continue 
  print(x)
```
```output
apple
qw1
cherry
```
#### range(start,stop,skip) 
```python 
for x in range(5):
  print(x)
else:
   print("Finally finished!") 
```
```output 
0
1
2
3
4
Finally finished!
```
```python 
for x in range(1,10,2):
  print(x)
```
```output
1
3
5
7
9
```
#### range(start,stop,skip) 
```python
for x in range(1,10):
   print("*")
   for j in range(x):
    print("#",end="")
else:
    print("\ndone printing ")
```
```output
*
#*
##*
###*
####*
#####*
######*
#######*
########*
#########
done printing 
```
```python
adj = ["red", "big", "tasty"]
fruits = ["apple", "banana", "cherry"]

for x in adj:
  for y in fruits:
    print(x, y)
```
```output
red apple
red banana
red cherry
big apple
big banana
big cherry
tasty apple
tasty banana
tasty cherry
```





