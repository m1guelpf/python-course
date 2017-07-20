# Day 4

## Dictionaries

> A dictionary is similar to a list, but you access values by looking up a key instead of an index. A key can be any string or number.

``` python
numbers = {'one' : 1, 'two' : 2, 'three' : 3} # create a numbers dictionary
numbers['one'] # acces the one value. This will return the value (1)
```

### Changing a dictionary

``` python
numbers = {'one' : 1, 'two' : 2, 'three' : 3}
numbers['four'] = 4 # add a new key to the numbers dictionary
del numbers['one'] # delete a key from the numbers dictionary
```

### Dictionary methods

``` python
user_balance = {'user1' : 200, 'user2' : 12, 'user3' : 3600}
user_balance.values() # returns a list containing the dictionary values. [3600, 12, 200]
user_balance.items() # returns a list with a tuple for each key-value. [('user3', 3600), ('user2', 12), ('user1', 200)]
user_balance.keys() # returns a list containing the dictionary keys. ['user3', 'user2', 'user1']
```

## Iterables

> Iterables are objects you can iterate. Lists, tuples & dictionaries are iterables

``` python
animals = ["cat", "dog", "rabbit"]
for animal in animals: # for every key our list has
  print animal # print the value
animals = ("cat", "dog", "rabbit")
for animal in animals: # this also works for tuples
  print animal # print the value
animals = {"cat" : "Meow!", "dog" : "Woof!", "rabbit" : "..."}
for animal in animals:
  print animals[animal] # here it's a little different, because you access dictionary values in a different way
```