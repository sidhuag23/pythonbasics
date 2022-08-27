#### basic strings
```python
print("Hello")
print('Hello')
```
#### Assign string to a variable 
```python
a="hello"
print(a)
```
#### Multiline Strings (double )
```python 
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a) 
```

#### Multiline Strings (single)
```python 
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)
```
#### Slicing
```python 
b = "Hello, World!"
print(b[2:5]) #output -> llo

b = "Hello, World!"
print(b[:5]) #output -> Hello

b = "Hello, World!"
print(b[2:]) #output -> llo, World!
```
#### Negative Indexing

From: "o" in "World!" (position -5)
To, but not included: "d" in "World!" (position -2):
```python 
b = "Hello, World!"
print(b[-5:-2]) #output -> orl
```
#### Modify Strings

#### upper() -> makes string to upper case 
```python
a="hello world"
print(a.upper()) #output ->  HELLO WORLD
```
#### lower() -> makes method returns the string in lower case 
```python
print(a.lower())  #output ->  hello world
```
#### strip() -> whitespace is the space before and/or after the actual text,
```python 
a = " Hello, World ! "
print(a.strip()) #output -> Hello, World !
```
#### replace() -> replace() method replaces a string with another string
```python
a = "Hello, World!"
print(a.replace("H", "J")) #output -> Jello, World!
```
#### split() -> split() method splits the string into substrings if it finds instances of the separator and returns a list
```python
a="hello , world!"
b =a.split(",")
print(b) #output -> ['hello ', ' world!']
```
#### string concatenation 
```python
a = "Hello"
b = "World"
c = a + " " + b
print(c) #output -> Hello World
```
#### format string / your_string.format(placeholder_variable)
```python
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price)) #output -> I want to pay 49.95 dollars for 3 pieces of item 567.
```
#### escape sequence 
```python 
txt = "We are the so-called \"Vikings\" from the north."
```
<pre>
\' 	Single Quote 	
\\ 	Backslash 	
\n 	New Line 	
\r 	Carriage Return 	
\t 	Tab 	
\b 	Backspace 	
\f 	Form Feed 	
\ooo 	Octal value 	
\xhh 	Hex value
</pre>

#### Strings are Arrays
```python
a = "Hello, World!"
print(a[1])
for i in a:
    print(i)
```
```output
e
H
e
l
l
o
,
 
W
o
r
l
d
!
```
#### len() ->  function returns the length of a string
```python 
a = "Hello, World!"
print(len(a))
```
```output 
13
```
#### in -> to check if something exist 
```python
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.") #output -> Yes, 'free' is present.
```
#### not in -> to check if something doesnt exit 
```python 
txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.") #output -> No, 'expensive' is NOT present.
```

#### String Methods
https://www.w3schools.com/python/python_strings_methods.asp
