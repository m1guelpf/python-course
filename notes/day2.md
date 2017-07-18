# Day 2

## Python Comparisor Operators

| Python Symbol | Meaning                                     |
| ------------- | ------------------------------------------- |
| `==`, `!=`    | Equals, Not Equals                          |
| `>`, `<`      | Greater than, Less than                     |
| `>=`, `<=`    | Greater than or equals, Less than or equals |

## Python Logical Operators

| Python Symbol | Meaning                                         |
| ------------- | ------------------------------------------------|
| `and`         | Both `statement` `and` `statement` must be true |
| `or`          | Either `statement` `or` `statement` must be true|

## For Loops

![Flowchart](https://www.programiz.com/sites/tutorial2program/files/forLoop.jpg)
``` python
animals = ["dog", "cat", "rabbit"]
for animal in animals: # for each item in our animals list...
  print (animal) # print the animal name
```

## `range()` function

``` python
range(stop) # returns an iterable object containig numbers from 0 to stop
range(start, stop) # you can specify a number to start at
range(start, stop, step) # you can also specify steps, i.e. "let's count from start to stop moving step by step"
```

## While Loops

![Flowchart](https://upload.wikimedia.org/wikipedia/commons/4/43/While-loop-diagram.svg)
``` python
animals = ["cat", "dog", "rabbit"]
while len(animals) > 0: # while this condition is true
  print(animals.pop(0)) # print the first animal name and remove it from the list
```