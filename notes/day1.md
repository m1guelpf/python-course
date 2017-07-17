# Day 1

## `print()` function

``` python
# Print a string
print("Hello World")
# Print a variable
print(varname)
# Print can accept multiple arguments
print(var1, var2)
```

## Variables

``` python
# Add a string to a variable
varname = "String"
# Add an integer to a variable
varname = 1
# Add a boolean to a variable
varname = True
```

### Variable names

* Can't start with a number
* Whitespaces & special signs not allowed
* Case-sensitive

### Variable Types

| Python Name| Full Name | Variable format  |
| -----------| --------- | -----------------|
| bool       | Boolean   | `True`/`False`   |
| int        | Integer   | `1`,`2`,`3`...   |
| float      | Float     | `1.23`, `1.24`...|
| str        | String    | `"Hello"`        |
| []         | List      | `[1,2,3,4,5]`    |

## Operators

|Python Name           | Notes                                                                       |
|----------------------| ----------------------------------------------------------------------------|
|`(` `)`               |                                                                             |
|`**`                  | Exponent/Power                                                              |
|`*`, `/`, `//`, `%`   | `//` - integer division, `%` - modulus                                      |
|`+`, `-`              |                                                                             |
|`+=`, `-=`, `*=`, `/=`| i.e. `x+=3` is shorthand for `x=x+3`                                        |
|`>`, `<`, `>=`, `<=`  | Bigger than, smaller than, Bigger than or equal to, smaller than or equal to|

## `input()` function

``` python
# Ask the user his name and save it to a variable
name = input("What is your name?")
```
## Python Lists

``` python
# Create a list of animals
animals = ["cat", "dog", "rabbit"]
# Lists can have all types of variables
mixed = ["String", 1, True, 2.12]
# You can access an element of a list using indexes
animals[0] # returns "cat"
# Lists also have some special methods
len(animals) # returns the number of animals we have
animals.append("cheetah") # adds "cheetah" at the end of the animals list
animals.insert(i, "cheetah") # adds "cheetah" to the animals list at the given position
animals.remove("dog") # remove "dog" from the animals list
animals.pop(i) # returns animals[i] and deletes it from the list
animals.sort() # sorts the list alphanumerically
```

### Splicing

``` python
years = [2012, 2013, 2014, 2015, 2016, 2017]
some_years= years[i:i2] # returns a list with items from i to i2, inclusive
```

## Concatenation

``` python
age = "13"
print("You are " + age + " years old")
```

## Joining and Splitting
``` python
var shopping_list = ["spam", "eggs"]
var separator = ", "
joined = separator.join(shopping_list) # returns a string with the list elements concatenated with the separator. ("spam, eggs")
joined.split(separator) # returns a list with the string elements. (["spam", "eggs"])
```

## Tuples

> Tuples are immutable lists. Once you define them, you can't change them.

``` python
tuple1 = ("String", 1, True, 2.12) # tuples are defined with parentheses instead of brackets
tuple2 = "String", 1, True, 2.12 # this is the same as the above
empty = () # this is an empty tuple
tuple3 = (50,) # you still need the comma when there's only one value
tuple1[0] # returns "String"
tuple2[2:4] # you can also use splicing
```

## Placeholders

``` python
age = 13
name = "David"
sentence = "%s is %d years old" %(name,age) # assigns each placeholder a variable. (David is 13 years old)
sentence = "{name} is {age} years old".format(name = name, age = age) # same than the above. (David is 13 years old)
```

## Conditionals

``` python
if expression: # if expression evaluates to True...
  statement # do something
elif expression: # if the above evaluates to False, and this evaluates to True...
  statement # do something
else: # if neither of the above evaluate to True
  statement # do something
```