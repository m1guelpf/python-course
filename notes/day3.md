# Day 3

## Python functions

``` python
def function_name(parameters): # define a new function function_name that accepts parameters. A function can take multiple, one or no parameters.
  """docstring""" # commend specifying what the class does. You can access it in the code as __doc__ if you need it.
  statements # statements to execute inside the function
  
function_name(parameters) # then, we can call the function
```

### Variable scope

``` python
variable1 = "I am a global variable" # variables defined in the "root" can be accessed anywhere

def function(input): # the input of the function is only available inside the function
  variable2 = "I am not a global variable" # variables defined inside a function can only be accessed inside the function
  print(variable1) # global variables can be accessed anywhere

variable3 = "I am another global variable" # here, take another global variable!
```

### The return statement

``` python
def filter_animals(input): # example function that accepts an input
  """Function to remove non-animals from a list"""
  animals = ["dog", "cat", "rabbit"]
  result = list(set(input).intersection(animals)) # creates a list with the items preset in both lists
  return result # returning something from a function allows as to get it as output of the function

things = ["table", "chair", "cat"]
animals = filter_animals(things) # the result will be saved into the variable because we are returning it
```

## More functions

``` python
str() # returns the input as a string. i.e. 1 => "1"
int() # returns the input as an integer. i.e. "1" => 1
list() # returns the input as a list. i.e. ("one", "two") => ["one", "two"]
tuple() # returns the input as a tuple. i.e. ["one", "two"] => ("one", "two")
len() # returns the input's length
sum() # sums the items of a list
min() # returns the smallest item of a list
max() # returns the biggest item of a list
type() # returns the type of the input. i.e. type(["one", "two"]) => <class 'list'>
```

## Modules

> Python modules are simply Python files with the `.py` extension, which implement a set of functions

``` python
import animals # This imports the module animals. You can now call its functions by doing animals.function()
from animals import rabbit # This imports ONLY the rabbit function from the animals module. You can now call it by doing rabbit()

food = "carrot"
rabbit(food) # let's give the rabbit a carrot!
```
