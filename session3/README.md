## variable
```python
x = 12 # just a variable

# change it
x = 'hellllloo'

# another one
y = 12.2

# increment
x = x + 1

# shorter
x += 1
x += 8

# also you can do this with other operators
x -= 12
x **= 2
x %= 5
```


## functions
```python
def function_name():
    do_something

def say_hello():
    print('hello')

```

### function parameters
```python
def say_hello(name):
    print('hello', name)
```

### functions can return sth
```python
def jam(a, b):
    return a + b

def zarb(a, b):
    # this is a comment
    # you can also return a variable
    result = a * b
    return result
```

## lists
```python
names = ['saeide', 'zahra', 'gholi', 'kourush', 'ali', 'jafar']
```

### size of a list
```python
size = len(names)
```

### indexing
```python
first_item = names[0] # programmers count from zero :)
second_item = names[1]

# also negative indexes
last_item = names[-1]
```

### list to variable
```python
numbers = [1, 2, 3]
a, b, c = numbers
```

### convert string to list
```python
characters = list('amir')
``` 

### concat, append
```python
numbers = [1, 2, 3]

# wanna add 4 to numbers
numbers.append(4)

# also you can do this
numbers += [4]

numbers += [8, 6, 5]

# but what happens if you do this?
numbers.append([4])

# and this
numbers += 4 # error
```

### list of 10 zeros
```python
my_list = [0] * 10

# or a non_pythonic way
my_list = []
for i in range(10):
    mylist.append(0)
```

## for loops
```python
for variable in sequence:
    do_sth

numbers = [1, 2, 3]
for number in numbers:
    print(number)

# range based loop
for i in range(1, 12):
    print(i)

# try this one
for i in range(1, 12, 2):
    print(i)

for i in range(12, 1, -1):
    print(i)

# nested loops
for x in range(1, 20):
    for y in range(1, 10):
        print(x, y)

# this is not pythonic (but works fine!)
for i in range(len(numbers)):
    print(numbers[i])
```

## single line if statement
```python
name = 'amir'
family = 'mohamadi' if name == 'amir' else 'unknown'
```

## print tricks
```python
print('salam', end=', ') # it will print "salam, " without newline
```

## input tricks
```python
x = input() # a string input

x = input('plz give me your number ') # a string input with message

x = int(input()) # integer input
x += 1

# assume input is sth like this:
# 2 amir mohamadi
i = input()
# now i is: '2 amir mohamadi'

# you can split it
i = i.split()
# now i is ['2', 'amir', 'mohamadi']

# you can unpack
num, name, family = input().split()

# but the num is strign yet
# do this
num = int(num)


# try this to get a list of integers in one line :D
# assume the input is 1 2 3 4
a, b, c, d = map(int, input().split())
```
